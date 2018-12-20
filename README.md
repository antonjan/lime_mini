# lime_mini
This repository will have all my Lime mini configurations.
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
## Testing the transmitter in Gnuradio
Here is a Gnuradio block that will modulate the Lime mini sdr with Fm from Microphone and 1 Khz zone.<br>
Slide
In the gnuradio radio directory is a working Transmitter testing code.
![Lime_gnuradio_TX_1.png](gnuradio/Lime_gnuradio_TX_1.png?raw=true "Block diagram")<br>
Here is the settings for the Lime mini. (you need to install the soapySDR drivers.<br>
![Lime_gnuradio_TX_2.png ](gnuradio/Lime_gnuradio_TX_2.png?raw=true "Block diagram")<br>
Screenshot of Application<br>
![Lime_gnuradio_TX_3.png](gnuradio/Lime_gnuradio_TX_3.png?raw=true "Block diagram")<


