## Description
A Linux script to easily install and enable the bias tee from an **RTL-SDR Blog V3** USB dongle to power the **RTL-SDR Blog ADS-B Triple Filtered LNA**.


## Install & Enable Bias Tee
Run the following command to install and enable the bias tee.  Be sure the RTL-SDR Blog V3 USB dongle and the RTL-SDR Blog ADS-B Triple Filtered LNA are both connected before running this script!
```
bash -c "$(wget -O - https://github.com/mypiaware/rtlsdr_bias_tee/raw/master/rtlsdr_bias_tee.sh)"
```


## Compatibility:
This bias tee installation script has been tested and confirmed to work with the following:
* FlightAware's PiAware SD image (3.7.1)
* **_dump1090-fa_** addon package installed on Raspbian Stretch and Raspbian Buster
* **_dump1090-mutability_** addon package installed on Raspbian Stretch and Raspbian Buster
