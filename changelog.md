# Changelog

# Production

## v1.0.7


**Status:** deployed in [production](http://inspire.ec.europa.eu/validator/)

**Release date:** 23/07/2019


### Modifications in ETS for the issue [#89](https://github.com/inspire-eu-validation/community/issues/89)
Relaxed the validation allowing xsd:date xsd:gYearMonth xsd:gYear
* ETS Repository: [testquery-md.xq](https://github.com/inspire-eu-validation/ets-repository/tree/master/)
* ETS: [md-iso.h.1](https://github.com/inspire-eu-validation/ets-repository/commit/ece63911fd528907540f30a422efc28257905e65)
* ETS Version: v0.3.0


### Modifications in ETS for some links
Updated links refering to metadata repository because of the rebuild of branches
* ETS Repository: [metadata/](https://github.com/inspire-eu-validation/metadata/tree/master/)
* ETS: [links updated](https://github.com/inspire-eu-validation/ets-repository/commit/4d74b0c69a6621fbdbc6945e3140bcb6afe063a2)


### Modifications in ETS for the issues [#69](https://github.com/inspire-eu-validation/community/issues/69), [#70](https://github.com/inspire-eu-validation/community/issues/70), [#71](https://github.com/inspire-eu-validation/community/issues/71), [#72](https://github.com/inspire-eu-validation/community/issues/72), [#73](https://github.com/inspire-eu-validation/community/issues/73)
Metadata Dataset has been updated relaxing the CodeList validation
* ETS Repository: [metadata/2.0/common](https://github.com/inspire-eu-validation/ets-repository/tree/master/metadata/2.0/common/)
* ETS: [md common req C.15: Language Code](https://github.com/inspire-eu-validation/ets-repository/commit/5b75bc7931f9d4f4f58d2505b05f463b306c1de7)
* ETS: [md common req C.17: Language Code](https://github.com/inspire-eu-validation/ets-repository/commit/5b75bc7931f9d4f4f58d2505b05f463b306c1de7)
* ETS: [md common req C.18: Language Code](https://github.com/inspire-eu-validation/ets-repository/commit/5b75bc7931f9d4f4f58d2505b05f463b306c1de7)
* ETS Version: v0.3.0


### Modifications in ETS for the issue [#52](https://github.com/inspire-eu-validation/community/issues/52)
A CodeList value has been added
* ETS Repository: [metadata/2.0/common](https://github.com/inspire-eu-validation/ets-repository/tree/master/metadata/2.0/common/)
* ETS: [md common req C.5: Language Code](https://github.com/inspire-eu-validation/ets-repository/commit/ece63911fd528907540f30a422efc28257905e65)
* ETS Version: v0.3.0


## v1.0.6

**Status:** deployed in deployed in [production](http://inspire.ec.europa.eu/validator/)

**Release date:** 05/06/2019

### Modifications in ETS for the issue [#262](https://github.com/inspire-eu-validation/ets-repository/issues/262)
The Croatian title of the Regulation 1089/2010 has been added.
* ETS Repository: [metadata/iso](https://github.com/inspire-eu-validation/ets-repository/tree/master/metadata/iso)
* ETS: [md-iso.c.4: Dataset conformity](https://github.com/inspire-eu-validation/ets-repository/commit/5eea1ab22ccddbad45c728eb4a799adde58a0ed7)
* ETS Version: v0.3.0

## v1.0.5

**Status:** deployed in deployed in [production](http://inspire.ec.europa.eu/validator/)

**Release date:** 04/06/2019

### Modifications in ETS for the issue [#45](https://github.com/inspire-eu-validation/community/issues/45)
The XPath of Coordinate Reference System and Spatial Representation Type have been relaxed. The validation that the value of CRS is a http URI and includes one of the values from table 2 in [TG_DS_TMPL](http://inspire.ec.europa.eu/id/ats/data/3.0rc3/interoperability-metadata/README#ref_TG_DS_TMPL) is removed.
* ETS Repository: [data/interoperability-metadata](https://github.com/inspire-eu-validation/ets-repository/tree/master/data/interoperability-metadata)
* ETS: [md-iop.a.1: Coordinate Reference System](https://github.com/inspire-eu-validation/ets-repository/commit/e2eddde1bd4511c458f96be38550482356edc776) and [md-iop.a.6: Spatial Representation Type](https://github.com/inspire-eu-validation/ets-repository/pull/269/commits/8a2f45c6aadb42ecd4aa62dfbf8ca3cde2d3321a)
* ETS Version: v0.2.5
* ATS Repository: [data/interoperability-metadata](https://github.com/inspire-eu-validation/data/tree/master/interoperability-metadata)
* ATS: [coordinate-reference-system.md](https://github.com/inspire-eu-validation/data/blob/master/interoperability-metadata/coordinate-reference-system.md) and [spatial-representation-type.md](https://github.com/inspire-eu-validation/data/blob/master/interoperability-metadata/spatial-representation-type.md)

## v1.0.4

**Status:** deployed in deployed in [production](http://inspire.ec.europa.eu/validator/)

**Release date:** 13/05/2019

### Modifications in ETS for the issue [#251](https://github.com/inspire-eu-validation/ets-repository/issues/251)
The validation checks that the 'zoning' properties references a resource 'CadastralZoning' instead of 'BasicPropertyUnit'.
* ETS Repository: [data-cp/cp-ia](https://github.com/inspire-eu-validation/ets-repository/tree/master/data-cp/cp-ia)
* ETS: [cp-ia.b.4: CadastralParcel.zoning](https://github.com/inspire-eu-validation/ets-repository/commit/c2eaf40db5f515dd0db385fd7cb745f297c104cc)
* ETS Version: v0.2.2

## v1.0.3

**Status:** deployed in deployed in [production](http://inspire.ec.europa.eu/validator/)

**Release date:** 15/04/2019

### Modifications in ETS for the issue [#180](https://github.com/inspire-eu-validation/ets-repository/issues/180)
The assertion checks that there is a non-empty value of the element CI_DateTypeCode.
* ETS Repository: [metadata/iso](https://github.com/inspire-eu-validation/ets-repository/tree/master/metadata/iso)
* ETS: [md-iso.f.1: Dataset keyword](https://github.com/inspire-eu-validation/ets-repository/commit/2cdd5f60dce728c4a32ac197a1599eefbf5bbabd)
* ETS Version: v0.2.9

## v1.0.2

**Status:** deployed in deployed in [production](http://inspire.ec.europa.eu/validator/)

**Release date:** 07/03/2019

### Modifications in ETS and ATS for the issue [#117](https://github.com/inspire-eu-validation/ets-repository/issues/117)
Some modifications are needed in the ETS code. The validations have been divided in two main blocks of code. In a first step the ETS validates that exists at least one url that is a valid service (WFS, WMS, WCS, SOS or Atom). In a second step, if one or more URL exists and is valid, there will be no 'TR.unknownXMLResource' errors. If there is not any available URL, some warning(s) will be shown.
* ETS Repository: [metadata/iso](https://github.com/inspire-eu-validation/ets-repository/tree/master/metadata/iso)
* ETS: [md-iso.c.3: Dataset linkage](https://github.com/inspire-eu-validation/ets-repository/commit/08bf74c4db1935e16c358f2a9e6ca28ce448e9fa)
* ETS Version: v0.2.8
* ATS Repository: [metadata/iso](https://github.com/inspire-eu-validation/metadata/tree/master/iso-19115-19119)
* ATS: [ds-linkage.md](https://github.com/inspire-eu-validation/metadata/blob/master/iso-19115-19119/ds-linkage.md)

## v1.0.1

**Status:** deployed in deployed in [production](http://inspire.ec.europa.eu/validator/)

**Release date:** 01/02/2019

### Modifications in ETS and ATS for the issues [#5](https://github.com/inspire-eu-validation/community/issues/5) and [#189](https://github.com/inspire-eu-validation/ets-repository/issues/189) and [#257](https://github.com/inspire-eu-validation/ets-repository/issues/257)
Improvements in the code to call to the https secure urls instead of the http to avoid the redirection.
* ETS Repository: [data/interoperability-metadata](https://github.com/inspire-eu-validation/ets-repository/tree/master/data/interoperability-metadata)
* ETS: [md-iop.a.5: Character Encoding](https://github.com/inspire-eu-validation/ets-repository/pull/190/commits/7cd3252de2e100d08a82b5121534b906e575af0d) and [md-iop.a.6: Spatial Representation Type](https://github.com/inspire-eu-validation/ets-repository/pull/190/commits/7cd3252de2e100d08a82b5121534b906e575af0d)
* ETS Version: v0.2.4
* ATS Repository: [data/interoperability-metadata](https://github.com/inspire-eu-validation/data/tree/master/interoperability-metadata)
* ATS: [character-encoding.md](https://github.com/inspire-eu-validation/data/blob/master/interoperability-metadata/character-encoding.md) and [spatial-representation-type.md](https://github.com/inspire-eu-validation/data/blob/master/interoperability-metadata/spatial-representation-type.md)

### Modifications in ETS for the issue [#180](https://github.com/inspire-eu-validation/ets-repository/issues/180)
The check for the text value of dateType element is removed. The assertion should only check that the codeListValue attribute is "publication".
* ETS Repository: [metadata/iso](https://github.com/inspire-eu-validation/ets-repository/tree/master/metadata/iso)
* ETS: [md-iso.f.1: Dataset keyword](https://github.com/inspire-eu-validation/ets-repository/commit/2603836e5ce9a233020d5c12477e74c3a8e4618b)
* ETS Version: v0.2.7

### Modifications in ETS for the issue [#182](https://github.com/inspire-eu-validation/ets-repository/issues/182)
Improvements in the code to check the descendant elements of wfs:FeatureCollection element for all feature types.
* ETS Repository: [data-ad/ad-gml](https://github.com/inspire-eu-validation/ets-repository/tree/master/data-ad/ad-gml), [data-au/au-gml](https://github.com/inspire-eu-validation/ets-repository/tree/master/data-au/au-gml), [data-cp/cp-gml](https://github.com/inspire-eu-validation/ets-repository/tree/master/data-cp/cp-gml), [data-gn/gn-gml](https://github.com/inspire-eu-validation/ets-repository/tree/master/data-gn/gn-gml), [data-hy/hy-gml](https://github.com/inspire-eu-validation/ets-repository/tree/master/data-hy/hy-gml), [data-ps/ps-gml](https://github.com/inspire-eu-validation/ets-repository/tree/master/data-ps/ps-gml) and [data-tn/tn-gml](https://github.com/inspire-eu-validation/ets-repository/tree/master/data-tn/tn-gml)
* ETS: [ad-gml.a.1: Address feature in dataset](https://github.com/inspire-eu-validation/ets-repository/commit/aabe657e60e5d831c97e7a4b49a968659daa5af8), [au-gml.a.1: Administrative Unit feature in dataset](https://github.com/inspire-eu-validation/ets-repository/commit/aabe657e60e5d831c97e7a4b49a968659daa5af8), [cp-gml.a.1: CadastralParcel feature in dataset](https://github.com/inspire-eu-validation/ets-repository/commit/aabe657e60e5d831c97e7a4b49a968659daa5af8), [gn-gml.a.1: Geographical Names feature in dataset](https://github.com/inspire-eu-validation/ets-repository/commit/aabe657e60e5d831c97e7a4b49a968659daa5af8), [hy-gml.a.1: Hydrographic feature in dataset](https://github.com/inspire-eu-validation/ets-repository/commit/aabe657e60e5d831c97e7a4b49a968659daa5af8), [ps-gml.a.1: Protected site feature in dataset](https://github.com/inspire-eu-validation/ets-repository/commit/aabe657e60e5d831c97e7a4b49a968659daa5af8) and [tn-gml.a.1: Transport Network feature in dataset](https://github.com/inspire-eu-validation/ets-repository/commit/aabe657e60e5d831c97e7a4b49a968659daa5af8)
* ETS Version: v0.2.2

### Modifications in ETS for the issue [#188](https://github.com/inspire-eu-validation/ets-repository/issues/188)
Modifications in the code to correct the Spanish and French titles of GEMET controlled vocabulary.
* ETS Repository: [metadata/iso](https://github.com/inspire-eu-validation/ets-repository/tree/master/metadata/iso)
* ETS: [md-iso.c.4: Dataset conformity](https://github.com/inspire-eu-validation/ets-repository/commit/8803ede975879ec1ea484aec73a09ac15abb5480)
* ETS Version: v0.2.8

## v1.0.0 

**Status:** deployed in [production](http://inspire.ec.europa.eu/validator/)

**Release date:** 09/09/2018

### Modifications in ETS and ATS for the issue [#30](https://github.com/inspire-eu-validation/ets-repository/issues/30)
Improvements in the code in order not to check anymore the specification in the test.
* ETS Repository: [data/interoperability-metadata](https://github.com/inspire-eu-validation/ets-repository/tree/master/data/interoperability-metadata)
* ETS: [md-iop.a.3: Encoding](https://github.com/inspire-eu-validation/ets-repository/commit/fb0ce3c988226e88c25141d5e3f4d0b54b0f3d8b)
* ETS Version: v0.2.3
* ATS Repository: [data/interoperability-metadata](https://github.com/inspire-eu-validation/data/tree/master/interoperability-metadata)
* ATS: [encoding.md](https://github.com/inspire-eu-validation/data/blob/master/interoperability-metadata/encoding.md)

### Modifications in ETS and ATS for the issue [#127](https://github.com/inspire-eu-validation/ets-repository/issues/127)
Improvements in the code to relax the xPath validations for name and version.
* ETS Repository: [data/interoperability-metadata](https://github.com/inspire-eu-validation/ets-repository/tree/master/data/interoperability-metadata)
* ETS: [md-iop.a.3: Encoding](https://github.com/inspire-eu-validation/ets-repository/pull/162/commits/b9e5eeec7b930a28514108cf13cbabae5989f3af)
* ETS Version: v0.2.3
* ATS Repository: [data/interoperability-metadata](https://github.com/inspire-eu-validation/data/tree/master/interoperability-metadata)
* ATS: [encoding.md](https://github.com/inspire-eu-validation/data/blob/master/interoperability-metadata/encoding.md)

### Modifications in ETS and ATS for the issue [#119](https://github.com/inspire-eu-validation/ets-repository/issues/119)
Improvements in the code to accept application/atom as a media type for distribution. 
* ETS Repository: [metadata/iso](https://github.com/inspire-eu-validation/ets-repository/tree/master/metadata/iso)
* ETS: [md-iso.d.2: Service linkage](https://github.com/inspire-eu-validation/ets-repository/pull/162/commits/50153ba18168b9c9361ef3e8483fa776bb4c66a4)
* ETS Version: v0.2.6
* ATS Repository: [metadata/iso](https://github.com/inspire-eu-validation/metadata/tree/master/iso-19115-19119)
* ATS: [srv-linkage.md](https://github.com/inspire-eu-validation/metadata/blob/master/iso-19115-19119/srv-linkage.md)

### Modifications in ETS and ATS for the issue [#130](https://github.com/inspire-eu-validation/metadata/issues/130)
The vocabulary test should check that the date type is "publication" and the date is "2008-06-01" when the title of the thesaurus is "GEMET - INSPIRE themes, version 1.0". 
* ETS Repository: [metadata/iso](https://github.com/inspire-eu-validation/ets-repository/tree/master/metadata/iso)
* ETS: [md-iso.f.1: Dataset keyword](https://github.com/inspire-eu-validation/ets-repository/pull/162/commits/47ce651dd03adfa974777a3ffde452b483c970b4)
* ETS Version: v0.2.6
* ATS Repository: [metadata/iso](https://github.com/inspire-eu-validation/metadata/tree/master/iso-19115-19119)
* ATS: [ds-keyword.md](https://github.com/inspire-eu-validation/metadata/blob/master/iso-19115-19119/ds-keyword.md)

### Modifications in ETS and ATS for the issue [#120](https://github.com/inspire-eu-validation/ets-repository/issues/120)
Improvements in the code to check if there is at least one DQ_ConformanceResult element, in case there is none the test fails. 
Other check added is whether the title of one of the CI_Citation elements is the title of the Data interoperability IRs (in different languages).
* ETS Repository: [metadata/iso](https://github.com/inspire-eu-validation/ets-repository/tree/master/metadata/iso)
* ETS: [md-iso.c.4: Dataset conformity](https://github.com/inspire-eu-validation/ets-repository/pull/162/commits/51138055828d5a226694c055c87d69b23c6a980f)
* ETS Version: v0.2.6
* ATS Repository: [metadata/iso](https://github.com/inspire-eu-validation/metadata/tree/master/iso-19115-19119)
* ATS: [ds-conformity.md](https://github.com/inspire-eu-validation/metadata/blob/master/iso-19115-19119/ds-conformity.md)

### Modifications in ETS and ATS for the issue [#130](https://github.com/inspire-eu-validation/ets-repository/issues/130) 
Some improvements in the code: 
This test case only applies to records with a hierarchyLevel value 'dataset' or 'series'. 
For every DQ_ConformanceResult element, check if there is at least one specification. In case there is none, the test fails.
The DQ_ConformanceResult has an element gmd:pass that must contain a value of type gco:Boolean.
* ETS Repository: [metadata/iso](https://github.com/inspire-eu-validation/ets-repository/tree/master/metadata/iso)
* ETS: [md-iso.a.5: Specification](https://github.com/inspire-eu-validation/ets-repository/pull/162/commits/f9d928db15aa056125326cdca347c27a311de1f5#diff-45c8fc7d1c02631d6be2d09a7bcea1ac)
* ETS Version: v0.2.6
* ATS Repository: [metadata/iso](https://github.com/inspire-eu-validation/metadata/tree/master/iso-19115-19119)
* ATS: [ds-specification.md](https://github.com/inspire-eu-validation/metadata/blob/master/iso-19115-19119/ds-specification.md)

# Staging

## v1.0.11
**Status:** deployed in [staging](http://staging-inspire-validator.eu-west-1.elasticbeanstalk.com/etf-webapp/)

### Modifications in ETS for the issue [#106](https://github.com/inspire-eu-validation/community/issues/106) 
Relaxed md-iso.f.1: Dataset keyword test
* ETS Repository: [ets-md-common-bsxets](https://github.com/inspire-eu-validation/ets-repository/blob/master/metadata/1.3/iso/ets-md-iso-bsxets.xml)

## v1.0.10
**Status:** deployed in [staging](http://staging-inspire-validator.eu-west-1.elasticbeanstalk.com/etf-webapp/)

### Modifications in ETS for the issue [#111](https://github.com/inspire-eu-validation/community/issues/111) 
The user detected a false validation that passed the test even if it should not pass. The corrections where applied on the corresponding file.
* ETS Repository: [ets-md-common-bsxets](https://github.com/inspire-eu-validation/ets-repository/blob/master/metadata/2.0/common/ets-md-common-bsxets.xml)

### Modifications in ETS for the issue [#74](https://github.com/inspire-eu-validation/community/issues/74) 
The test has been relaxed. 
* ETS Repository: [ets-md-sds-bsxets](https://github.com/inspire-eu-validation/ets-repository/blob/master/metadata/2.0/sds/ets-md-sds-bsxets.xml)

## v1.0.9

**Status:** deployed in [staging](http://staging-inspire-validator.eu-west-1.elasticbeanstalk.com/etf-webapp/)

## Modifications in ETS for issue [#118](https://github.com/inspire-eu-validation/community/issues/118)
There was some typo errors on Metadata 2.0 Conformance Class source.
The corresponding typo errors were fixed.
* Corresponding pull: [Typo-fixed ](https://github.com/inspire-eu-validation/ets-repository/pull/336/commits/1fa74d8da6e3b3acb7c845700b550f103e9d0fa6)

## v1.0.8

**Status:** deployed in [staging](http://staging-inspire-validator.eu-west-1.elasticbeanstalk.com/etf-webapp/)

### Modifications in ETS for the issue [#101](https://github.com/inspire-eu-validation/community/issues/101) 
The validator was looking for `/Capabilities/ServiceProvider/Role` instead of `/Capabilities/ServiceProvider/ServiceContact/Role`. 
The corresponding file was modified.
* ETS Repository:  [dis-csw-core-soapui-project](https://github.com/inspire-eu-validation/ets-repository/blob/master/service/ds-wfs-direct-soapui-project.xml)

### Modifications in ETS for the requirement on [#94](https://github.com/inspire-eu-validation/community/issues/94) 
The URL error message was uncertain because it does not says which URL is wrong. The corresponding files were modified.
* ETS Repository:  [TranslationTemplateBundle-EID70a263c0-0ad7-42f2-9d4d-0d8a4ca71b52](https://github.com/inspire-eu-validation/ets-repository/blob/master/include-metadata/TranslationTemplateBundle-EID70a263c0-0ad7-42f2-9d4d-0d8a4ca71b52.xml)
* ETS Repository:  [datasets-and-series/ets-md-datasets-and-series-bsxets](https://github.com/inspire-eu-validation/ets-repository/blob/master/metadata/2.0/datasets-and-series/ets-md-datasets-and-series-bsxets.xml)

### Modifications in ETS for the requirement on [#93](https://github.com/inspire-eu-validation/community/issues/93) 
The test was checking that the value follow `let $regex_float := '^-?\d+\.\d{2,}'` which means 100 is not valid but 100.00 is.
The corresponding file was modified.
* ETS Repository:  [ets-md-datasets-and-series-bsxets](https://github.com/inspire-eu-validation/ets-repository/blob/master/metadata/2.0/datasets-and-series/ets-md-datasets-and-series-bsxets.xml)

