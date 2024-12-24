# SLSC EDS Plugin Custom Device

The SLSC Electronic Datasheet (EDS) Plugin Custom Device enables access to _properties_, _commands_, and _physical channels_ of any [SLSC](https://www.ni.com/en-us/shop/select/slsc-category) module within VeriStand.

In the absence of a VeriStand custom device for a specific hardware module, this custom device can be used by directly referencing its SLSC Capabilities File.

## Using the Custom Device

- Download the latest release of the VeriStand Custom Devices on [ni.com](https://www.ni.com/en-us/support/downloads/software-products/download.veristand-custom-devices.html) or manually from the [GitHub Releases page](https://github.com/ni/niveristand-slsc-eds-custom-device/releases)
- See the [User Guide](Docs/User%20Guide.md) for a walkthrough of using the Custom Device.

## LabVIEW Source Code Version

LabVIEW 2020

## Dependencies

### Running the custom device

- [VeriStand 2023 or later](https://www.ni.com/en-us/support/downloads/software-products/download.veristand.html)

### Developing or building from source

- [LabVIEW 2023 or later](https://www.ni.com/en-us/support/downloads/software-products/download.labview.html)
- [LabVIEW Real-Time Module](https://www.ni.com/en-us/support/downloads/software-products/download.labview-real-time-module.html)
- [NI R Series Multifunction RIO](https://www.ni.com/en-us/support/downloads/drivers/download.ni-r-series-multifunction-rio.html)
  - Required for FPGA-based loopback test, not a direct dependency of the Custom Device
- [VeriStand Custom Device Development Tools](https://github.com/ni/niveristand-custom-device-development-tools)
  - Install the latest package from the [release page](https://github.com/ni/niveristand-custom-device-development-tools/releases)
- [VeriStand Custom Device Testing Tools](https://github.com/ni/niveristand-custom-device-testing-tools)
  - Install the latest package from the [release page](https://github.com/ni/niveristand-custom-device-testing-tools/releases)

## Git History & Rebasing Policy
Branch rebasing and other history modifications will be listed here, with several notable exceptions:
- Branches prefixed with `dev/` may be rebased, overwritten, or deleted at any time.
- Pull requests may be squashed on merge.

## License

The SLSC EDS (Electronic Datasheet) Plugin Custom Device is licensed under an MIT-style license (see LICENSE). Other incorporated projects may be licensed under different licenses. All licenses allow for non-commercial and commercial use.

**This project distribution includes the following licensed software. Reuse of this software requires compliance with the associated license:**
 - JKI JSON Serialization & Deserialization Library for LabVIEW: https://github.com/JKISoftware/JKI-JSON-Serialization/blob/master/LICENSE.md
