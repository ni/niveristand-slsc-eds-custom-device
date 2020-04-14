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

Each _property_ and _command_ will have an entry for **Default Value**. This value is applied to the module on deployment of the system definition by default. To disable this behavior, uncheck the **Apply Default Values on Deployment?** checkbox.

Similarly, each _property_ and _command_, where available, will have a **Reset Value** that is applied by default when the system definition is undeployed. To disable this behavior, uncheck the **Apply Rese Values when Undeployed?** checkbox.

To modify the default values, select the _property_ or _command_ in the table and a control will appear above the table. When modifying a value, it is assumed to be the **Default Value**. To modify the **Reset Value**, check the **Modify Reset Value?** checkbox next to the value entry above the table.

![Modify Command Value](Support/Modify%20Command%20Value.png)

## References


It is recommended to target a SLSC board when the chassis running because this would allow the SLSC EDS to read the capabilities features in the board. If you do that, then the module in the specific slot will return the specific capability in the specific slot: