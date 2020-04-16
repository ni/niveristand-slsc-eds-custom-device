## Overview

The SLSC Electronic Datasheet (EDS) Plugin Custom Device enables access to _properties_, _commands_, and _physical channels_ of any [SLSC](https://www.ni.com/en-us/shop/select/slsc-category) module within VeriStand.

In the absence of a VeriStand custom device for a specific hardware module, this custom device can be used.

## Usage

### Adding a Module

The SLSC EDS Plugin Custom Device is added to VeriStand in an SLSC Chassis under the desired controller. An example of this location is _Targets » Controller » Hardware » SLSC » SLSC Chassis » Modules_, as shown below.

![Add Module to System Definition](Support/Add%20Module%20to%20System%20Definition.png)

Once the module has been added to a slot, clicking the **Autodetect** button at the top of the System Explorer window will enable configuration of the module's _properties_, _commands_, and _physical channels_.

If the chassis is online and a module is present in the chosen slot when **Autodetect** is clicked, the module's capabilities will be read directly from the module to provide configuration for the _properties_, _commands_, and _physical channels_. If the module is not present, a configuration can be imported by selecting a capabilities file stored on disk when clicking **Autodetect**.

![Module Configuration](Support/Module%20Configuration.png)

### Configuring a Module

#### Default and Reset Values

Each _property_ and _command_ will have an entry for **Default Value**. This value is applied to the module on deployment of the system definition by default. To disable this behavior, uncheck the **Apply Default Values on Deployment?** checkbox.

Similarly, each _property_ and _command_, where available, will have a **Reset Value** that is applied by default when the system definition is undeployed. To disable this behavior, uncheck the **Apply Rese Values when Undeployed?** checkbox.

To modify the default values, select the _property_ or _command_ in the table and a control will appear above the table. When modifying a value, it is assumed to be the **Default Value**. To modify the **Reset Value**, check the **Modify Reset Value?** checkbox next to the value entry above the table.

![Modify Command Value](Support/Modify%20Command%20Value.png)

#### Runtime Configuration

By default, each _property_ and _command_ will have a VeriStand channel created for it. While the system definition is deployed, these channel values can be changed to alter the default configuration of the module.

These channels can be removed from the system definition if they are not required for the application. If the system has a large channel count, reducing the number of deployed channels can increase system performance.

### Developer Plugins

The SLSC EDS Plugin Custom Device supports displaying circuit diagrams and device pinouts for a module. When developing a module intended for use with the SLSC EDS custom device, the dynamic buttons at the top of the System Explorer window can be enabled by placing files in the following locations:

**Diagram** button: `%PUBLIC%\Documents\National Instruments\NI VeriStand\<version>\SLSC Plugins\Modules\SLSC EDS Plugins\<vendor prefix>\<product number>_Diagram.png`

**Pinout** button: `%PUBLIC%\Documents\National Instruments\NI VeriStand\<version>\SLSC Plugins\Modules\SLSC EDS Plugins\<vendor prefix>\<product number>_Pinout.png`

**Note**: `<vendor prefix>` and `<product number>` are defined in the SLSC capabilities files for the module.

![Diagram and Pinout](Support/Diagram%20and%20Pinout.png)

## References

[Legacy Release Notes](https://forums.ni.com/t5/NI-VeriStand-Add-Ons-Documents/SLSC-Electronic-Datasheet-EDS-Plugin-Custom-Device/ta-p/3812754)

[Legacy Support Forum](https://forums.ni.com/t5/NI-VeriStand-Add-Ons-Discussions/SLSC-EDS-Plugin-Custom-Device-Feedback/td-p/3812753)
