# lime_mini
This repository will have all my Lime mini configurations.
## Installing soapysdr on ubuntu 18.10
sudo apt-get install python3-pip python3-pyqt5 python3-numpy python3-scipy soapysdr python3-soapysdr
#packages for soapysdr available at myriadrf PPA<br>
/usr/share/doc/soapysdr-tools<br>
cd /usr/share/doc/soapysdr-tools/
sudo add-apt-repository -y ppa:myriadrf/drivers<br>
sudo apt-get update<br>
sudo apt-get install limesuite liblimesuite-dev limesuite-udev limesuite-images<br>
sudo apt-get install soapysdr-tools soapysdr-module-lms7<br>
sudo apt-get install soapysdr<br>
LimeUtil --info<br>
SoapySDRUtil --info<br>
SoapySDRUtil --find="driver=lime"<br>

## Testing the Lime Mini
LimeUtil --info<br>
LimeUtil --find<br>
SoapySDRUtil --info<br>
SoapySDRUtil --find="driver=lime"<br>
#testing<br>

cd /home/anton/lime-tools/build<br>
sudo ./LimeMon<br>
sudo ./LimeScan<br>

/usr/bin/LimeQuickTest<br>
/usr/bin/LimeSuiteGUI<br>
/usr/bin/LimeUtil<br>
#LimeQuickTest<br>
<br>
LimeQuickTest --no-gui<br>
LimeQuickTest --gui<br>
#testing lime<br>
https://wiki.myriadrf.org/Testing_the_LimeSDR<br>
<br>
LimeSuiteGUI<br>
https://wiki.myriadrf.org/LimeSDR-USB_Quick_Test<br>
## Testing the transmitter in Gnuradio.
Link to block source https://github.com/antonjan/lime_mini/blob/master/gnuradio/Lime_transmitter_test_zr6aic.grc
Here is a Gnuradio block that will modulate the Lime mini sdr with Fm from Microphone and 1 Khz zone.<br>
In the gnuradio radio directory is a working Transmitter testing code.<br>
![Lime_gnuradio_TX_1.png](gnuradio/Lime_gnuradio_TX_1.png?raw=true "Block diagram")<br>
Here is the settings for the Lime mini. (you need to install the soapySDR drivers.<br>
![Lime_gnuradio_TX_2.png ](gnuradio/Lime_gnuradio_TX_2.png?raw=true "Block diagram")<br>
Screenshot of Application<br>
Changing the PTT value to 1 enables modelation.<br>
Changing the enable tone to value 1 will switch the modelation from internal Microphone of laptop to the 1Khz tone generator.<br>
The Moddulation can be seen in the FFT Plot box.<br>
![Lime_gnuradio_TX_3.png](gnuradio/Lime_gnuradio_TX_3.png?raw=true "Block diagram")


