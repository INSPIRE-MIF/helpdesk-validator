## v1.0.2

**Status:** merged into master

**Release date:** 07/03/2019

### Modifications in ETS and ATS for the issue #117
Some modifications are needed in the ETS code. The validations have been divided in two main blocks of code. In a first step the ETS validates that exists at least one url that is a valid service (WFS, WMS, WCS, SOS or Atom). In a second step, if one or more URL exists and is valid, there will be no 'TR.unknownXMLResource' errors. If there is not any available URL, some warning(s) will be shown.
* Repository: metadata/iso
* ETS: md-iso.c.3: Dataset linkage
* Version: v0.2.8
* ATS: ds-linkage.md
* Issue: [#117](https://github.com/inspire-eu-validation/ets-repository/issues/117)

## v1.0.1

**Status:** merged into master 

**Release date:** 01/02/2019

### Modifications in ETS and ATS for the issue community#5
Improvements in the code to call to the https secure urls instead of the http to avoid the redirection.
* Repository: data/interoperability-metadata
* ETS: md-iop.a.5: Character Encoding and md-iop.a.6: Spatial Representation Type
* Version: v0.2.4
* ATS: character-encoding.md and spatial-representation-type.md
* Issue: [community#5](https://github.com/inspire-eu-validation/community/issues/5) and [#189](https://github.com/inspire-eu-validation/ets-repository/issues/189)

### Modifications in ETS for the issue #180
The check for the text value of dateType element is removed. The assertion should only check that the codeListValue attribute is "publication".
* Repository: metadata/iso
* ETS: md-iso.f.1: Dataset keyword
* Version: v0.2.7
* Issue: [#180](https://github.com/inspire-eu-validation/ets-repository/issues/180)

### Modifications in ETS for the issue #182
Improvements in the code to check the descendant elements of wfs:FeatureCollection element for all feature types.
* Repository: data-ad/ad-gml, data-au/au-gml, data-cp/cp-gml, data-gn/gn-gml, data-hy/hy-gml, data-ps/ps-gml and data-tn/tn-gml
* ETS: ad-gml.a.1: Address feature in dataset, au-gml.a.1: Administrative Unit feature in dataset, cp-gml.a.1: CadastralParcel feature in dataset, gn-gml.a.1: Geographical Names feature in dataset, hy-gml.a.1: Hydrographic feature in dataset, ps-gml.a.1: Protected site feature in dataset and tn-gml.a.1: Transport Network feature in dataset
* Version: v0.2.2
* Issue: [#182](https://github.com/inspire-eu-validation/ets-repository/issues/182)

### Modifications in ETS for the issue #188
Modifications in the code to correct the spanish and french titles of GEMET controlled vocabulary.
* Repository: metadata/iso
* ETS: md-iso.c.4: Dataset conformity
* Version: v0.2.8
* Issue: [#188](https://github.com/inspire-eu-validation/ets-repository/issues/188)

## v1.0.0 

**Status:** deployed in reference validator

**Release date:** 09/09/2018

### Modifications in ETS and ATS for the issues #30
Improvements in the code to don´t check anymore the specification in the test.
* Repository: data/interoperability-metadata
* ETS: md-iop.a.3: Encoding
* Version: v0.2.3
* ATS: encoding.md
* Issue: [#30](https://github.com/inspire-eu-validation/ets-repository/issues/30)

### Modifications in ETS and ATS for the issues #127
Improvements in the code to relax the xPath validations for name and version.
* Repository: data/interoperability-metadata
* ETS: md-iop.a.3: Encoding
* Version: v0.2.3
* ATS: encoding.md
* Issue: [#127](https://github.com/inspire-eu-validation/ets-repository/issues/127)

### Modifications in ETS and ATS for the issue #119
Improvements in the code to accept application/atom as a media type for distribution. 
* Repository: metadata/iso
* ETS: md-iso.d.2: Service linkage
* Version: v0.2.6
* ATS: srv-linkage.md
* Issue: [#119](https://github.com/inspire-eu-validation/ets-repository/issues/119)

### Modifications in ETS and ATS for the issue #130
The vocabulary test should check that the date type is "publication" and the date is "2008-06-01" when the title of the thesaurus is "GEMET - INSPIRE themes, version 1.0". 
* Repository: metadata/iso
* ETS: md-iso.f.1: Dataset keyword
* Version: v0.2.6
* ATS: ds-keyword.md
* Issue: [#130](https://github.com/inspire-eu-validation/metadata/issues/130)

### Modifications in ETS and ATS for the issue #120. 
Improvements in the code to check if there is at least one DQ_ConformanceResult element, in case there is none the test fails. 
Other check added is whether the title of one of the CI_Citation elements is the title of the Data interoperability IRs (in different languages).
* Repository: metadata/iso
* ETS: md-iso.c.4: Dataset conformity
* Version: v0.2.6
* ATS: ds-conformity.md
* Issue: [#120](https://github.com/inspire-eu-validation/ets-repository/issues/120)

### Modifications in ETS and ATS for the issue #130 
Some improvements in the code: 
This test case only applies to records with a hierarchyLevel value 'dataset' or 'series'. 
For every DQ_ConformanceResult element, check if there is at least one specification. In case there is none, the test fails.
The DQ_ConformanceResult has an element gmd:pass that must contain a value of type gco:Boolean.
* Repository: metadata/iso
* ETS: md-iso.a.5: Specification
* Version: v0.2.6
* ATS: ds-specification.md
* Issue: [#130](https://github.com/inspire-eu-validation/ets-repository/issues/130)
