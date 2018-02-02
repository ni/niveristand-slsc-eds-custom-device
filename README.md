# SLSC-EDS-Plugin-Custom-Device
SLSC EDS (Electronic Datasheet) Plugin Custom Device allows any generic SLSC Capabilities File to be used within the VeriStand.

### LabVIEW Version ###

LabVIEW 2017

### Built Availability ###

Builds of this IP are available on request through NI field sales.

### Quality, Limitations ###

Preview

Only user "admin" with empty password access is supported at the moment due to a limitation from the chassis custom device.

### Developer Documentation ###

#### Design Decisions ####
- always use NVMEMcap.bin file and custom parser to extract all information from module. This reduces effort for maintaining the option of importing automatically from a connected module as well as an offline configuration.
- Not showing string properties since it is unknown how they would be used in VeriStand.
- 

### Dependencies ###
- NI SLSC >= 17.0
- [VeriStand-Addon-Inline-Async-API](https://github.com/NIVeriStandAdd-Ons/VeriStand-Addon-Inline-Async-API/tree/master/Built) >= 1.0.0.29
- [JKI JSON Serialization & Deserialization Library for LabVIEW](vipm://jki_lib_json_serialization?repo_url=http://www.jkisoft.com/packages) >= 1.1.10.37

### License ###

*This repository and any materials provided by NI therein are provided AS IS. NI DISCLAIMS ANY AND ALL LIABILITIES FOR AND MAKES NO WARRANTIES, EITHER EXPRESS OR IMPLIED, INCLUDING WITHOUT LIMITATION ANY WARRANTIES OF MERCHANTABILITY, FITNESS FOR  PARTICULAR PURPOSE, OR NON-INFRINGEMENT OF INTELLECTUAL PROPERTY. NI shall have no liability for any direct, indirect, incidental, punitive, special, or consequential damages for your use of the repository or any materials contained therein.*

**This project distribution includes the following licensed software. Reuse of this software requires compliance with the associated license:**
 - JKI JSON Serialization & Deserialization Library for LabVIEW: https://github.com/JKISoftware/JKI-JSON-Serialization/blob/master/LICENSE.md