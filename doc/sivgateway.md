# Giesecke+Devrient (G+D) SIV Gateway with Azure IoT Edge

The name of the solution from G+D is “Secure Industrial Visibility” (SIV). Behind it, there is a smart box with a secure operating system and a piece of software that enables remote access to individual machines while also protecting them against cyber attacks. This is an exclusive limited public preview of the integration of Azure IoT Edge on the [G+D SIV Gateway](https://www.gi-de.com/en/au/mobile-security/industries/manufacturing-and-iiot/secure-iot-connection/). G+D is well known for its security innovation and practices which are the gold standards in the field of securing devices and gateways on the edge across many industries.
G+D SIV gateways have impressive and proven security features which include:
* Security especially with regards to secure execution.
* Shock and vibration proof
* Lifetime guarantees
* Several sector specific certifications

Our ecosystem partners who include silicon partners and processor partners (i.e., Intel, ARM) secure devices and IoT Edge from the ground up by working together to incorporate security features such as:
* Secure boot and updates
* Trusted attestations
* Hardware attestation
* Endpoint attestation
* Static (storage) attestation
* Runtime (memory) attestation
* Data Protection and Privacy
* At rest, in flight, persistent cache
* Monitoring and reporting
* Device health
* System/Network health
* Tamper resistance

** About this Hack Lab

This tutorial provides step-by-step guidance to configure the SIV Gateway to run Azure IoT Edge and deploy modules based on containers. Full credit goes to the G+D Mobile Security, Cyber Security Division.

** HOWTO - Access to the SIV Gateway WebGUI

1. Connect a wired connection to the SIV Gateway on LAN2 port which is the same network as your machine. Configure your machine's TCP/IP properties with a static IP, i.e., 1.0.1.2 with the subnet 255.255.255.0.
2. The SIV Gateway has a default IP on LAN 2: 1.0.1.1
2. To access the WebGUI for configuration, open a browser and enter following URL  https://1.0.1.1:4444. Accept the security warning on your browser.
3. Username: Admin, Password: Secure Visibility
4. In the WebGUI you can configure the "External LAN" for Internet access. Connect a wired connection fr6m your Internet AP/router onto the LAN1 port on the SIV Gateway.

** HOWTO - Setting up Azure IoT Edge on SIV Gateway

1. You should see this banner in the WebGUI main page. ![SIV Gateway Web GUI version](/doc/media/sivgwwebgui.jpg)
2. Select External LAN.
3. Select DHCP and click Submit.
4. When completed, you should see a display log with your LAN1 info eg. IP address and gateway
5. Click OK to return to the main menu.
6. Select Security.
7. Under the Firewall section, enter 443 5671 for “Allowed TCP ports for External LAN:” and click Submit
> This allows connectivity with Azure IoT Hub over HTTPS (port 443) or AMQP (port 5671 for edgeHub communication with IoT Hub).
8. When completed, you should see a display log showing eg. allowed TCP ports etc.
9. Click OK to return to the main menu.
10. Select Container Manager.
11. Under the Cloud container management section, next to “Device Connected String” enter the <Connection String> for your IoT Edge device and click Setup.
> You can retrieve the connection string from the IoT Edge (preview) section of your Azure IoT Hub by clicking on your IoT Edge device.
12. When completed, you should see a display log with various info regarding your IoT Edge device, ending with “Runtime started”.
13. Click OK to return to the Container Manager.
14. SIV Gateway's Azure IoT Edge now pulls container images as specified in your IoT Edge device configuration in the cloud.

  