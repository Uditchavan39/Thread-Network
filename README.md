# Thread-Network
Connect DHT11 at Port 0 pin 11
Press Button 1 on each NRF board Including receiver board.
So Temperature
Reading will be transmitted to central board
With 8 sec delay. 


## ESP to NRF connection
connect pins as follows.
NRF Tx => ESP Rx
NRF Rx => ESP Tx
NRF CTs => ESP RTs
NRF RTs => ESP CTs
Pin number is mentioned in the ESPGoogleSheet.ino file
