# SLSC-EDS-Plugin-Custom-Device

SLSC EDS (Electronic Datasheet) Plugin Custom Device allows any generic SLSC Capabilities File to be used within VeriStand.

## LabVIEW Version ##

LabVIEW 2017


## Developer Documentation ##

### Design Decisions ###
- always use NVMEMcap.bin file and custom parser to extract all information from module. This reduces effort for maintaining the option of importing automatically from a connected module as well as an offline configuration.
- Not showing string properties since it is unknown how they would be used in VeriStand.


## Dependencies

- NI-SLSC >= 17.0
- [VeriStand-Addon-Inline-Async-API](https://github.com/NIVeriStandAdd-Ons/VeriStand-Addon-Inline-Async-API/tree/master/Built) >= 1.0.0.29
- [NI VeriStand Custom Device Testing Tools](https://github.com/ni/niveristand-custom-device-testing-tools)
- JKI JSON >= 1.1.10.37


## License

The NI VeriStand Custom Device Testing Tools are licensed under an MIT-style license (see LICENSE). Other incorporated projects may be licensed under different licenses. All licenses allow for non-commercial and commercial use.

**This project distribution includes the following licensed software. Reuse of this software requires compliance with the associated license:**
 - JKI JSON Serialization & Deserialization Library for LabVIEW: https://github.com/JKISoftware/JKI-JSON-Serialization/blob/master/LICENSE.md