# Wireless Protocols

## Frequencies and channels

**Frequency is a characteristic of a signal that describes the number of cycles per unit time this signal makes**. Phase, amplitude, wavelength, wave number are other characteristics of a signal. Channel is a term used to describe a medium upon which information passes under certain conditions.

**TODO**
Digest these two articles:
- https://petri.com/2-4ghz-vs-5ghz-wifi/
- https://www.centurylink.com/home/help/internet/wireless/which-frequency-should-you-use.html

## 802.11

[802.11](https://www.techtarget.com/searchmobilecomputing/definition/80211) is a body of wireless communication standards that's developed by the [Institute for Electrical and Electronic Engineers (IEEE)](https://www.ieee.org/).

### [Standards Chart](https://en.wikipedia.org/wiki/IEEE_802.11)

**\* Note**: Speeds are theoretical

|Standard|Year Released|Frequency (GHz)|Speed|Range (Indoor)|Range (Outdoor)|
|--- |--- |--- |--- |--- |--- |
|802.11|1997|2.4|2Mbps|20m|100m|
|802.11a|1999|5|1.5-54Mbps|35m|120/5000m|
|802.11b|1999|2.4|11Mbps|35m|120m|
|802.11g|2003|2.4|54Mbps|38m|140m|
|802.11n|2009|2.4/5|600Mbps|70m|250m|
|802.11ac|2013|2.4/5|450/1300Mbps|35m|-|
|802.11ax|2019|2.4/5|10-15Gbs|30m|120m|

## Bluetooth

Bluetooth is a short-range wireless technology standard that is used for exchanging data between fixed and mobile devices over short distances and building personal area networks. In the most widely used mode, transmission power is limited to 2.4 GHz, giving it a very short range of up to 10 meters or 30 feet.

In the early days, Bluetooth was really focused on internet of thing devices, and while trying to discover other devices the battery would drain pretty bad. Bluetooth 4.0 introduced [Bluetooth LE (low energy)](https://www.bluetooth.com/learn-about-bluetooth/feature-enhancements/le-audio/), which consumed less power.

## Near Field Communication 

[Near Field Communication (NFC)](https://squareup.com/us/en/the-bottom-line/managing-your-finances/nfc)  is a point-to-point contact technology that allows two devices, like a smartphone and a payments terminal, to talk to each other when they’re very close together (0- 2 cm). It runs over 13.56 MHz and can be used to transfer information. 

### Radio Frequency Identification

[Radio Frequency Identification (RFID)](https://www.techtarget.com/iotagenda/definition/RFID-radio-frequency-identification) uses close to the same technology as NFC, but allows further communication.

There are three main components:
- Tag: container that digitizes and stores information. You have a reader that reads that information out of the tag.
	- **Active RFID.** An active RFID tag has its own power source, often a battery. They cover distances of 100 meters or 300 feet.
	- **Passive RFID.** A passive RFID tag receives its power from the reading antenna, whose electromagnetic wave induces a current in the RFID tag's antenna. They cover distances close to near field communication or 10-20 feet max. 
- Reader: reads information out of a tag.
- Antenna: associated with the wireless communication.

## Long range fixed wireless

Wi-Fi is pretty restrictive in distance. A lot of times what you'll see is:
- the higher the power, the shorter the distance
- the shorter the power, the greater the distance

For greater distances, long range fixed wireless comes in. This is where you have providers that use license and unlicensed bands and get the ability to extend the reach of that wireless communication beyond the limitations of Wi-Fi and again sometimes up to 100 meters.