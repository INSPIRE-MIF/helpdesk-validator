# Changelog

# Staging

## v1.0.9
**Status:** deployed in [staging](http://staging-inspire-validator.eu-west-1.elasticbeanstalk.com/etf-webapp/)


#### 🚀 New Features


#### 🐛 Bugfixes
* [#161](https://github.com/inspire-eu-validation/community/issues/161) Add support for new schemaLocation links on MD 1.3 - [#368](https://github.com/inspire-eu-validation/ets-repository/pull/368)
* [#165](https://github.com/inspire-eu-validation/community/issues/165) Fix typo error on Download Service WCS Core - [#369](https://github.com/inspire-eu-validation/ets-repository/pull/369)
* [#100](https://github.com/inspire-eu-validation/community/issues/100) Relax test for md sds 3.1: Resource Type - [#372](https://github.com/inspire-eu-validation/ets-repository/pull/372)

#### 💅 Enhancements
* [#96](https://github.com/inspire-eu-validation/community/issues/96) Stronger test for md sds 3.1 and md sds 3.8- [#373](https://github.com/inspire-eu-validation/ets-repository/pull/373)

#### 📝 Documentation
Updated [NetworkService_WMS_metadata_2.0_example](https://github.com/inspire-eu-validation/community/blob/master/examples/NetworkService_WMS_metadata_2.0_example)

# Production

# Releases

## v1.0.8

**Status:** deployed in [production](http://inspire.ec.europa.eu/validator/)

**Release date:** 18/11/2019

#### 🚀 New Features
ATS: 
* Add [ATS for SOS v1.0](https://github.com/inspire-eu-validation/download-sos)
* Add [ATS for WCS v1.0](https://github.com/inspire-eu-validation/download-wcs)
* Add [ATS for CSW v3.1](https://github.com/inspire-eu-validation/discovery-service/tree/review-ats-csw-3.1)


ETS:
* Add [ETS for SOS v1.0](https://github.com/inspire-eu-validation/ets-repository/tree/sos-tg-1.0) - [#226](https://github.com/inspire-eu-validation/ets-repository/pull/226)
* Add [ETS for WCS v1.0](https://github.com/inspire-eu-validation/ets-repository/tree/wcs-tg-1.0) - [#225](https://github.com/inspire-eu-validation/ets-repository/pull/225)
* Add [ETS for CSW v3.1](https://github.com/inspire-eu-validation/ets-repository/tree/csw-tg-3.1) - [#297](https://github.com/inspire-eu-validation/ets-repository/pull/297)


ETF:
* Add [test for SOS v1.0](http://inspire.ec.europa.eu/validator) - [#5](https://github.com/etf-validator/etf-sui-ae/pull/5)
* Add [test for WCS v1.0](http://inspire.ec.europa.eu/validator) - [#5](https://github.com/etf-validator/etf-sui-ae/pull/5)
* Add [test for CSW v3.1](http://inspire.ec.europa.eu/validator) - [#253](https://github.com/inspire-eu-validation/ets-repository/pull/253)


#### 🐛 Bugfixes
* [#52](https://github.com/inspire-eu-validation/community/issues/52) Relax test on MD 2.0 C.5 - [#318](https://github.com/inspire-eu-validation/ets-repository/pull/318)
* [#55](https://github.com/inspire-eu-validation/community/issues/55) Rename at06 to at06-mandatory-metadata-elements - [#293](https://github.com/inspire-eu-validation/ets-repository/pull/293)
* [#63](https://github.com/inspire-eu-validation/community/issues/63) Relax test on MD 2.0 - [#308](https://github.com/inspire-eu-validation/ets-repository/pull/308)
* [#67](https://github.com/inspire-eu-validation/community/issues/67) Fix test on MD 1.3 - [#307](https://github.com/inspire-eu-validation/ets-repository/pull/307)
* [#69](https://github.com/inspire-eu-validation/community/issues/69) Relax test on MD 2.0 C.3 - [#132](https://github.com/inspire-eu-validation/ets-repository/pull/132)
* [#70](https://github.com/inspire-eu-validation/community/issues/70) Relax test on MD 2.0 C.15 - [#132](https://github.com/inspire-eu-validation/ets-repository/pull/132)
* [#71](https://github.com/inspire-eu-validation/community/issues/71) Relax test on MD 2.0 C.17 - [#132](https://github.com/inspire-eu-validation/ets-repository/pull/132)
* [#73](https://github.com/inspire-eu-validation/community/issues/73) Relax test on MD 2.0 Comon Requirements - [#313](https://github.com/inspire-eu-validation/ets-repository/pull/313)
* [#74](https://github.com/inspire-eu-validation/community/issues/74) Relax test on MD 2.0 CC 3.5 - [#338](https://github.com/inspire-eu-validation/ets-repository/pull/338)
* [#87](https://github.com/inspire-eu-validation/community/issues/87) Update HTTP/HTTPS convertion - [#341](https://github.com/inspire-eu-validation/ets-repository/pull/341)
* [#89](https://github.com/inspire-eu-validation/community/issues/89) Relax validation on testquery-md - [#314](https://github.com/inspire-eu-validation/ets-repository/pull/314)
* [#93](https://github.com/inspire-eu-validation/community/issues/93) Add support for a double number on MD 2.0 CC 1.5 - [#319](https://github.com/inspire-eu-validation/ets-repository/pull/319) / [@fxprunayre](https://github.com/fxprunayre)
* [#101](https://github.com/inspire-eu-validation/community/issues/101) Add correction for attribute Role on CSW - [#323](https://github.com/inspire-eu-validation/ets-repository/pull/323)
* [#106](https://github.com/inspire-eu-validation/community/issues/106) Relax test on Dataset keyword on MD 1.3 - [#345](https://github.com/inspire-eu-validation/ets-repository/pull/345), [#342](https://github.com/inspire-eu-validation/ets-repository/pull/342)
* [#108](https://github.com/inspire-eu-validation/community/issues/108) Relax test on Dataset keyword on MD CSW Core Discovery Service - [#360](https://github.com/inspire-eu-validation/ets-repository/pull/360), [#342](https://github.com/inspire-eu-validation/ets-repository/pull/342)
* [#111](https://github.com/inspire-eu-validation/community/issues/111) Add support for correct validation on MD 2.0 Common Requirements C.17 & C.18 - [#354](https://github.com/inspire-eu-validation/ets-repository/pull/354), [#353](https://github.com/inspire-eu-validation/ets-repository/pull/353), [#351](https://github.com/inspire-eu-validation/ets-repository/pull/351)
* [#115](https://github.com/inspire-eu-validation/community/issues/115) Relax test on MD 1.3 - [#341](https://github.com/inspire-eu-validation/ets-repository/pull/341)
* [#118](https://github.com/inspire-eu-validation/community/issues/118) Fix typo errors on MD 2.0 all Conformance Classes - [#336](https://github.com/inspire-eu-validation/ets-repository/pull/336)
* [#134](https://github.com/inspire-eu-validation/community/issues/134) Update test for MD 1.3 Validate XML documents - [#346](https://github.com/inspire-eu-validation/ets-repository/pull/346)
* [#139](https://github.com/inspire-eu-validation/community/issues/139) Use of text() instead of node() - [#350](https://github.com/inspire-eu-validation/ets-repository/pull/350)
* [#144](https://github.com/inspire-eu-validation/community/issues/144) Update from node() to text() on MD 2.0 - [#352](https://github.com/inspire-eu-validation/ets-repository/pull/352)
* [#148](https://github.com/inspire-eu-validation/community/issues/148) Add support for multiple email address on MD 2.0 Common Requirements C.10 - [#364](https://github.com/inspire-eu-validation/ets-repository/pull/364)
* [#150](https://github.com/inspire-eu-validation/community/issues/150) Add support for redirections on MD 1.3 - [#359](https://github.com/inspire-eu-validation/ets-repository/pull/359)
* [#154](https://github.com/inspire-eu-validation/community/issues/154) Fix missing "(" - [#365](https://github.com/inspire-eu-validation/ets-repository/pull/365)

#### 💅 Enhancements
* Add TR.invalidLegendFormat message. - [#344](https://github.com/inspire-eu-validation/ets-repository/pull/344)
* [#7](https://github.com/inspire-eu-validation/community/issues/7) Add label to test execution to search them easily
* [#68](https://github.com/inspire-eu-validation/community/issues/68) Update maximum size of file to 20MB on ETF-webapp
* [#94](https://github.com/inspire-eu-validation/community/issues/94) Update error message for invalid URL on MD 2.0 - [#325](https://github.com/inspire-eu-validation/ets-repository/pull/325) / [@fxprunayre](https://github.com/fxprunayre)
* [#128](https://github.com/inspire-eu-validation/community/issues/128) Update schema on MD 1.3 - [#341](https://github.com/inspire-eu-validation/ets-repository/pull/341)
* [#131](https://github.com/inspire-eu-validation/community/issues/131) Relax test on MD 2.0 & CC1.6 - [#343](https://github.com/inspire-eu-validation/ets-repository/pull/343)
* [#138](https://github.com/inspire-eu-validation/community/issues/138) Improve schemaLocation on MD 1.3 - [#346](https://github.com/inspire-eu-validation/ets-repository/pull/346)

#### 📝 Documentation
* [Training Material](https://github.com/inspire-eu-validation/community/tree/master/training%20material)
* [Contribution Guidelines](https://github.com/inspire-eu-validation/community/blob/master/contribution_guidelines.md)
* [Code of Conduct](https://github.com/inspire-eu-validation/community/blob/master/code_of_conduct.adoc)


## v1.0.7


**Status:** deployed in [production](http://inspire.ec.europa.eu/validator/)

**Release date:** 23/07/2019


## v1.0.6

**Status:** deployed in [production](http://inspire.ec.europa.eu/validator/)

**Release date:** 05/06/2019

### Modifications in ETS for the issue [#262](https://github.com/inspire-eu-validation/ets-repository/issues/262)
The Croatian title of the Regulation 1089/2010 has been added.
* ETS Repository: [metadata/iso](https://github.com/inspire-eu-validation/ets-repository/tree/master/metadata/iso)
* ETS: [md-iso.c.4: Dataset conformity](https://github.com/inspire-eu-validation/ets-repository/commit/5eea1ab22ccddbad45c728eb4a799adde58a0ed7)
* ETS Version: v0.3.0

## v1.0.5

**Status:** deployed in [production](http://inspire.ec.europa.eu/validator/)

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

**Status:** deployed in [production](http://inspire.ec.europa.eu/validator/)

**Release date:** 15/04/2019

### Modifications in ETS for the issue [#180](https://github.com/inspire-eu-validation/ets-repository/issues/180)
The assertion checks that there is a non-empty value of the element CI_DateTypeCode.
* ETS Repository: [metadata/iso](https://github.com/inspire-eu-validation/ets-repository/tree/master/metadata/iso)
* ETS: [md-iso.f.1: Dataset keyword](https://github.com/inspire-eu-validation/ets-repository/commit/2cdd5f60dce728c4a32ac197a1599eefbf5bbabd)
* ETS Version: v0.2.9

## v1.0.2

**Status:** deployed in [production](http://inspire.ec.europa.eu/validator/)

**Release date:** 07/03/2019

### Modifications in ETS and ATS for the issue [#117](https://github.com/inspire-eu-validation/ets-repository/issues/117)
Some modifications are needed in the ETS code. The validations have been divided in two main blocks of code. In a first step the ETS validates that exists at least one url that is a valid service (WFS, WMS, WCS, SOS or Atom). In a second step, if one or more URL exists and is valid, there will be no 'TR.unknownXMLResource' errors. If there is not any available URL, some warning(s) will be shown.
* ETS Repository: [metadata/iso](https://github.com/inspire-eu-validation/ets-repository/tree/master/metadata/iso)
* ETS: [md-iso.c.3: Dataset linkage](https://github.com/inspire-eu-validation/ets-repository/commit/08bf74c4db1935e16c358f2a9e6ca28ce448e9fa)
* ETS Version: v0.2.8
* ATS Repository: [metadata/iso](https://github.com/inspire-eu-validation/metadata/tree/master/iso-19115-19119)
* ATS: [ds-linkage.md](https://github.com/inspire-eu-validation/metadata/blob/master/iso-19115-19119/ds-linkage.md)

## v1.0.1

**Status:** deployed in [production](http://inspire.ec.europa.eu/validator/)

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
