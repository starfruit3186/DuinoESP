1. Made changes for the ESP to connect to Pulse-Pool server:

    const char * host = "149.91.88.18";
    const int ports[] = {6000};
    
2. Apparently Pulse-Pool server uses "\r" as END_TOKEN not "\n"

3. The ESP have to request for MOTD from the server before requesting for JOB.

