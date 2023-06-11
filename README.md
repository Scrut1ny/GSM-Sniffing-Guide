## GSM Sniffing

| `Name` | `Desc.` |
|-|-|
| IMEI | [International Mobile Equipment Identity](https://en.wikipedia.org/wiki/International_Mobile_Equipment_Identity) |
| IMSI | [International Mobile Subscriber Identity](https://en.wikipedia.org/wiki/International_mobile_subscriber_identity) |
| MCC | [Mobile Country Code](https://en.wikipedia.org/wiki/Mobile_country_code) |
| MNC | [Mobile Network Code](https://en.wikipedia.org/wiki/Mobile_country_code) |
| MSIN | [Mobile Subscription Identification Number](https://en.wikipedia.org/wiki/Mobile_identification_number) |
| ICCID | [Integrated Circuit Card Identifier](https://en.wikipedia.org/wiki/SIM_card#ICCID) |
| MSID | Gigits Give Network you use |
|==========|==============================|
| GSM | [Global System for Mobile Communications](https://en.wikipedia.org/wiki/GSM) |
| SIM Card | [Subscriber Identity Module Card](https://en.wikipedia.org/wiki/SIM_card) |
| SMS | [Short Message/Messaging Service](https://en.wikipedia.org/wiki/SMS) |
| SDR | [Software-Defined Radio](https://en.wikipedia.org/wiki/Software-defined_radio) |

![image](https://user-images.githubusercontent.com/53458032/209445888-a0b016ee-0b05-49d6-a4ab-d14d72f632f7.png)

### Useful Websites
- OpenCellID - [Link](https://opencellid.org/)
- Cell Tower Locator (Cell2GPS) - [Link](http://www.cell2gps.com/)
- Cell Phone Trackers - [Link](https://cellphonetrackers.org/)
- International Numbering Plans - [Link](https://www.numberingplans.com/)
- GSM World Coverage Map and GSM Country List - [Link](https://www.worldtimezone.com/gsm.html)

### Information & Explanations
- IMSI-catcher - [Link](https://en.wikipedia.org/wiki/IMSI-catcher)
- GSM frequency bands - [Link](https://en.wikipedia.org/wiki/GSM_frequency_bands)
- List of software-defined radios - [Link](https://en.wikipedia.org/wiki/List_of_software-defined_radios)

### Useful Apps
- Mobile Software
  - Android-IMSI-Catcher-Detector - [Link](https://github.com/CellularPrivacy/Android-IMSI-Catcher-Detector)
  - SnoopSnitch - [Link](https://f-droid.org/en/packages/de.srlabs.snoopsnitch/)
- Desktop Software
  - GsmEvil 2 - [Link](https://github.com/ninjhacks/gsmevil2)
  - IMSI-catcher - [Link](https://github.com/Oros42/IMSI-catcher)

### Equipment
``GSM 900 / GSM 1800 MHz are used in most parts of the world: Europe, Asia, Australia, Middle East, Africa.``
``GSM 850 / GSM 1900 MHz are used in the United States, Canada, Mexico and most countries of S. America.``
- SDR
  - RTL-SDR (65MHz-2300MHz) - [Link](https://www.amazon.com/dp/B06Y1HKLHY)
- Antenna
  - Antenna - [Link](https://www.amazon.com/dp/B07HQJKMBD)

### Equipment
- Catching IMSI Catchers - [Link](https://youtu.be/eivHO1OzF5E)

### GSM Sniffing Install/Setup Guide
```
# Install
sudo apt-get update && apt install python3-numpy python3-scipy python3-scapy
sudo apt install gr-gsm
git clone https://github.com/Oros42/IMSI-catcher && cd IMSI-catcher
sudo grgsm_livemon && python3 simple_IMSI-catcher.py --sniff

# GSM Install Error? Try this!

sudo apt-get install -y \
    cmake \
    autoconf \
    libtool \
    pkg-config \
    build-essential \
    docutils \
    libcppunit-dev \
    swig \
    doxygen \
    liblog4cpp5-dev \
    gnuradio-dev \
    gr-osmosdr \
    libosmocore-dev \
    liborc-0.4-dev \
    swig
    
gnuradio-config-info -v

# Tips
sudo grgsm_scanner -l    # List your SDR connected.
sudo grgsm_scanner       # Scan for cell towers near you.
```


