# CatSniffer
Code Samples and Documentation for the Electronic Cats Cat Sniffer

Original Documentation and Code Samples (from Electronic Cats):
https://github.com/ElectronicCats/CatSniffer

The initial CatSniffer code (from the github above in firmware/SAMD/) is standard arduino code for working with the SemTech LoRa chips.  Being arduino compatible, Electronic Cats has another repo for adding in its boards to the "Boards Manager" section within the arduino IDE. 
https://github.com/ElectronicCats/Arduino_Boards_Index

Once the Electronics Cats boards are added (with json link), restart arduino and install them from the "Boards Manager" tab in the IDE.  This will install the necessary base files we need further for the CatSniffer to work with LoRa.  

Second, you will also need the RadioLib library from jgromes, found here: https://github.com/jgromes/RadioLib.  You can either download and manually install it (as I did), or you can also find it in the IDE under Tools >> Manage Libraries >> Search for "RadioLib".  The Electronic Cats transmit LoRa .ino needs the RadioLib to work. 

located in the "./arduino" folder are the sample sketched I used to get some receive and transmit LoRa packets. Two CatSniffers were used to prove out, one sending and one receiving the LoRa packets.  an SDR can also be used to verify/view the transmitted packets in the respective frequency/channel specified in radio.begin(). 

More to come in the near future!
