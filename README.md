## Description
A Linux script to easily install and enable the bias tee from an **RTL-SDR Blog V3** USB receiver dongle to power the **RTL-SDR Blog ADS-B Triple Filtered LNA**.

## Install & Enable Bias Tee
Run the following command to install and enable the bias tee.  Be sure the RTL-SDR Blog V3 USB receiver dongle and the RTL-SDR Blog ADS-B Triple Filtered LNA are both connected before running this script!
```
bash -c "$(wget -O - https://github.com/mypiaware/rtlsdr_bias_tee/raw/master/rtlsdr_bias_tee.sh)"
```

## Options
An option will first be given to "temporarily" enable the bias tee.  Selecting "yes" to this option immediately enables the bias tee. If the USB receiver dongle, LNA, computer and antenna are all connected and functioning, aircraft should be detected within two or three seconds after selecting "yes".  Note that at this point, the bias tee has not been configured to be enabled at every system boot.

A second option will be given to enable the bias tee at every system boot.  Typically, a user would want the bias tee enabled at every system boot.

## Uninstall
This script also provides an uninstall option that will uninstall the bias tee software and undo any edits that may have been done to any files.  The uninstall option will do a good job of returning the system to the way it was prior to this installation of the bias tee.  Note that performing the uninstall will also immediately disable the bias tee.


## Compatibility:
This bias tee installation script has been tested and confirmed to work with the following:
* FlightAware's PiAware SD image (3.7.1 & 3.7.2)
* **_dump1090-fa_** addon package installed on Raspbian Stretch and Raspbian Buster
* **_dump1090-mutability_** addon package installed on Raspbian Stretch and Raspbian Buster
