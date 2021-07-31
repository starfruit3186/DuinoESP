Please use the original DuinoCoin_Esp_Master.ino and DuinoCoin_Wire.ino by ricaun.

Replace the whole DuinoCoin_Clients.ino with this one.

Basically, the new DuinoCoin_Clients.ino only updated in order to switch to the new Pulse-Pool server. 
Duino Coin Master server does not response to "JOB" command anymore.

These are the major changes:

1. Made changes for the ESP to connect to Pulse-Pool server:

    const char * host = "149.91.88.18";
    const int ports[] = {6000};
    
2. Apparently Pulse-Pool server uses "\r" as END_TOKEN not "\n"

3. The ESP have to request for MOTD from the server before requesting for JOB.

