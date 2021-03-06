# Opcon WebServices Templates for Nutanix RestAPI
We share here .json templates that can be use as models to create WebServices  jobs subtypes in Opcon in order to interact with Nutanix clusters.

# Disclaimer
No Support and No Warranty are provided by SMA Technologies for this project and related material. The use of this project's files is on your own risk.

SMA Technologies assumes no liability for damage caused by the usage of any of the files offered here via this Github repository.

# Prerequisites
- Opcon V19.1
- SMA Webservices Connector for Windows or Linux V20.0.3
- A Nutanix Cluster running Nutanix API V2
- Create on Opcon on global property (mandatory) for Nutanix API url: 
    - [[myNutanixPrism]]: your Nutanix Prism API url (https://xxx.xxx.xxx.xxx:9440)
- Create two Optionnal global properties (crypted) for Nutanix user & password:
    - [[NutanixUser]]
    - [[NutanixPwd]]

# Instructions
- Download the .json file
- Create your Opcon job Type = Windows or Linux, Sub-type = Web Services and name it.
- Import Template, choose your .json
- On Variable tab, check if @User=[[NutanixUser]], @Password=[[NutanixPwd]] are ok and set any other variable required (OpCon Properties are supported).
- On Steps tab, Step1 in your job, check the body json, and modify it if need.
- On Failure Criteria tab, set the OK return code to 200.
- Save your Job. 
# License
Copyright 2019 SMA Technologies

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at [apache.org/licenses/LICENSE-2.0](http://www.apache.org/licenses/LICENSE-2.0)

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

# Contributing
We love contributions, please read our [Contribution Guide](CONTRIBUTING.md) to get started!

# Code of Conduct
[![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-v2.0%20adopted-ff69b4.svg)](code-of-conduct.md)
SMA Technologies has adopted the [Contributor Covenant](CODE_OF_CONDUCT.md) as its Code of Conduct, and we expect project participants to adhere to it. Please read the [full text](CODE_OF_CONDUCT.md) so that you can understand what actions will and will not be tolerated.
