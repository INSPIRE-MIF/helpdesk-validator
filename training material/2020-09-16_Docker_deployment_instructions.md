#### Deployment instructions

```CMD
docker login docker.pkg.github.com 
#Provide Github credentials
docker run --name inspire-validator -d -p 8080:8080 -v ~/etf:/etf docker.pkg.github.com/inspire-eu-validation/community/inspire-validator:2020.3
#Launches a container with the image, exposing it port 8080 through the same port in the host machine, and uses a volume in the local file system, on the directory ~/etf
```
##### Modifying the Docker image

In the inspire-validator ZIP file you can find all the resources needed to generate the Docker image from this release. If you would like to tweak anything from it, you can modify any of its contents (Dockerfile, entrypoint file, configuration files... ), then execute the command
```
docker build -t [IMAGE_NAME]:[VERSION]
```
You can run this again using the run command
```
docker run --name inspire-validator -d -p 8080:8080 -v ~/etf:/etf [IMAGE_NAME]:[VERSION]
```
##### Deployment on production host

The Docker image is set up to run at localhost to be deployed on any machine. However, users may need to acces their validator on a dedicated host, usually with a domain name. For proper functioning of the validator, their UI and correct rendering of Test Reports, validator needs to be configured to run on a domain.

If you want to run the webapp in another host, you can change the configuration file, inside the .war file inside the inspire-validator zip file accompanying this release, at ```WEB-INF/classes/etf-config.properties```, and modify the `etf.webapp.base.url` property. Then you can proceed to the build process described in the previous point.

##### Exposing the validator through a proxy

Usually host machines are connected in a private network that access to the Internet through a proxy. The Docker client needs to be configured to make use of this proxy, in order to be able to build the image and set up running the container.

For the build process, you need to add the following arguments to the command
```
--build-arg http_proxy=[HTTP_PROXY_URL:PORT]  --build-arg https_proxy=[HTTPS_PROXY_URL:PORT]  --build-arg no_proxy=127.0.0.1,localhost,*.<my-domain>
```
For the run command, you need to add the environment variables to it
```
--env http_proxy=[HTTP_PROXY_URL:PORT]  --env https_proxy=[HTTPS_PROXY_URL:PORT]  --env no_proxy=127.0.0.1,localhost,*.<mydomain>
```
These can also be set up in the Dockerfile, using the keyword ENV

For more information please check out https://docs.docker.com/network/proxy
