This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/). For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments

# About 
Microsoft Cloud Workshops are the closest thing to building your own Azure solution. Experts will guide attendees through a full end-to-end solution hack lab.

> Please note: Workshop content presumes a 200 to 300-level of architectural expertise of infrastructure and solutions design in this domain (even if on another platform). We suggest attendees take the Microsoft Azure Essentials course as a prerequisite if unfamiliar with Azure. 

> Prerequisite: You will use your own Azure subscription or you can create your Azure free account prior to the workshop.

## Two-Day IoT Cloud Workshop
The goal of this workshop is to develop a POC-quality IoT solution that includes IoT on the edge, device management, telemetry ingestion, hot/cold/warm path processing and reporting.

We begin with a short, informal Azure IoT briefing designed to explain key concepts and the latest announcement of the Azure IoT Suite and services. Please [Download](https://github.com/faister/msiotcloudworkshopau/blob/master/doc/Microsoft%20IoT%20Cloud%20Workshop.pdf) the presentation deck.
 
This will be followed by a hands-on lab session where you will learn how to implement an end-to-end solution simulating high velocity data emitted from smart meters and analysed in Azure. You will implement a lambda architecture, filtering a subset of the telemetry data for real-time visualization on the hot path, and storing all of the data in long-term cloud storage for the cold path. 

### Download Hands-on Lab (HOL)
Please [download](https://github.com/faister/msiotcloudworkshopau/blob/master/doc/hands-on%20lab%20step-by%20step%20-%20internet%20of%20things%20-%202018-03-v1.2.pdf) the HOL document.

If you are already comfortable with this HOL, you can proceed to the hack lab. 

## Hack Labs
During the hack lab, you can work individually or in your chosen group on any of the following scenarios: 

### PaaS Hack Labs
* Extend the Azure IoT Remote Monitoring or [Connected Factory preconfigured solutions](https://github.com/faister/connectedfactory) to connect to your own IoT assets
* Extend a solution from our Azure IoT solution partners who are co-delivering this workshop with Microsoft
  - [Giesecke+Devrient (G+D) SIV Gateway with Azure IoT Edge](https://github.com/faister/msiotcloudworkshopau/blob/master/doc/sivgateway.md)
* [Build custom Azure IoT Edge modules](https://github.com/faister/iot-workshop) to connect a sensor like TI Sensor Tag and perform  edge processing 
* Connect to process control systems and [publish OPC nodes/PLC tags to IoT Hub](https://github.com/faister/connectedfactory/blob/master/README.md#opc-ua-integration) using OPC UA Publisher on the edge
* [Learn](https://docs.microsoft.com/en-us/azure/iot-hub/iot-hub-arduino-iot-devkit-az3166-translator) how to make the IoT DevKit as a language translator by using Azure Cognitive Services. It records your voice and translates it to English text shown on the DevKit screen.
* [Learn](https://docs.microsoft.com/en-us/azure/iot-dps/how-to-connect-mxchip-iot-devkit#start-the-devkit) how to configure the IoT DevKit in order to make it automatically register to IoT Hub using the Device Provisioning Service (DPS).
> Borrow a MXChip IoT Devkit from one of your friendly workshop proctors
* Bring-your-own-IoT-scenario and we will try our best to guide how you build it using Azure IoT services

### SaaS Hack Lab
* [Check out](https://docs.microsoft.com/en-au/microsoft-iot-central/howto-connect-devkit) this tutorial to see if you are keen to put on a hat as a device developer to connect a MXChip IoT DevKit (DevKit) device to your Microsoft IoT Central application. If the answer is yes, please follow the steps below.
* [Start](https://www.microsoft.com/en-us/iot-central/) a Microsoft IoT Central 30-day free trial. Create a new app and choose "Sample Devkits" as your application template.
![IoT Central](/doc/media/iotcentralcreateapp.JPG?raw=true "IoT Central")
> Borrow a MXChip IoT Devkit from one of your friendly workshop proctors
