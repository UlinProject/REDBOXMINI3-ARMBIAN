<div id="header" align="center">

<b>[redboxmini3-armbian]</b>

(All technical information about the REDBOX MINI 3 device, including the ability to build the Linux ARMBIAN distribution.)
</div>


<b><i>Important: The data in this repository is experimental and may contain errors. This repository was developed primarily for devices with V3 specifications. Devices with less RAM and permanent memory, or different processors, are not currently supported.</b></i>

<b><i>Important: Users are solely responsible for making decisions about using this data and for collecting images to run third-party software.</b></i>

## Board versions

### * V3

<b><img src="./img/V301.jpg" width="20%"></img><img src="./img/V302.jpg" width="20%"></img><img src="./img/V303.jpg" width="20%"></img></b>

<b>CPU:</b> Allwinner H3 (armvh7, x4, 0.2Ghz-1.01Ghz)

<b>MEM:</b> 1GB (DDR3, 336.00 GHz - 672.00 GHz <b>(1344.01 GHz works too)</b>)

<b>Eth:</b> Internal (100mbit)

<b>WI-FI:</b> XR819 (was not considered)

<b>USB:</b> x2 2.0, (works, presumably the board has contacts for additional USB, This version does not have USB power management (it is always on))

<b>EMMC:</b> FORESEE MCEMAM6G-08G (booting from it works and tested on uboot-orange-pi-pc-plus)

<b>GPIO:</b> LED_PWR (1c20800, 15-PA15), LED_STATUS (1f02c00, 362-PL10), IR (1f02c00, 363-PL11), KEY_RESET (1f02c00, 355-PL3) (On this board you can get absolutely any gpio that is available on allwinner h3 (I’m just giving a list of those pins that you can get without much effort).)
