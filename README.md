# SLSC-EDS-Plugin-Custom-Device

SLSC EDS (Electronic Datasheet) Plugin Custom Device allows any generic SLSC Capabilities File to be used within VeriStand.

## LabVIEW Version

LabVIEW 2015


## Developer Documentation

### Design Decisions
- always use NVMEMcap.bin file and custom parser to extract all information from module. This reduces effort for maintaining the option of importing automatically from a connected module as well as an offline configuration.
- Not showing string properties since it is unknown how they would be used in VeriStand.


## Dependencies

- NI-SLSC >= 17.0
- [NI VeriStand Addon Inline Async API](https://github.com/ni/niveristand-custom-device-inline-async-api) >= 1.0.0.29
- [NI VeriStand Custom Device Testing Tools](https://github.com/ni/niveristand-custom-device-testing-tools)
- JKI JSON >= 1.1.10.37


## Git History & Rebasing Policy
Branch rebasing and other history modifications will be listed here, with several notable exceptions:
- Branches prefixed with `dev/` may be rebased, overwritten, or deleted at any time.
- Pull requests may be squashed on merge.


## License

The SLSC EDS (Electronic Datasheet) Plugin Custom Device is licensed under an MIT-style license (see LICENSE). Other incorporated projects may be licensed under different licenses. All licenses allow for non-commercial and commercial use.

**This project distribution includes the following licensed software. Reuse of this software requires compliance with the associated license:**
 - JKI JSON Serialization & Deserialization Library for LabVIEW: https://github.com/JKISoftware/JKI-JSON-Serialization/blob/master/LICENSE.md
