### DeviceTree

### Usage

Use the following commands to build the required DeviceTree configuration: 

| cmd           | info                                                                                                          |
| ------------- | ------------------------------------------------------------------------------------------------------------- |
| ```make```          | Build a standard classic DeviceTree for this device                                                             |
| ```make turbomod``` | Build a modified DeviceTree with turbo mode support (1.3V / 1.2GHz) |

### License and Sources

All foundational files are sourced from official upstream repositories. Original licenses and copyright notices are preserved without modifications. 

### Upstream Directories

* arm/ - Core ARM architecture devicetree directories
* dt-bindings/ - Standard device tree binding definitions

### Upstream Files

* sunxi-h3-h5.dtsi - Base Allwinner H3/H5 SoC configuration
* sun8i-h3.dtsi - Specific Allwinner H3 SoC definitions
* sunxi-common-regulators.dtsi - Common voltage regulator setups
