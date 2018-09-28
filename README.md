# Emergency Helper
This project is Emergency Helper. We joined Call for Code and using Node-RED.

## Team name
Team Osonoi

## Handouts
https://www.slideshare.net/secret/IDpw8kd8h66Q2D

## Consept & SourceCode
This concept is to carry container with minimal server using drone. The drone can be freely chosen and the container can be used for various purposes.
These sourcecode are imported json file to "Node-RED" and used.

コンセプトは、サーバー機能付きのコンテナをドローンで運ぶことです。ドローンは自由に選べますし、コンテナは様々な使い方ができます。

![Consept Image](https://github.com/kolinz/emergency-drone-messenger/blob/master/consept_image_1.PNG)

![Story](https://github.com/kolinz/emergency-drone-messenger/blob/master/consept_image_2.png)

1. When disaster occurs, The Drone and container takes off from the support base.
1. Broadcasting evacuation guidance message with sensor and speaker from Drone.
   - SourceCode [broadcasting-message.json](https://github.com/kolinz/emergency-drone-messenger/blob/master/node-red/broadcasting-message.json)
   - ![flow-image1](https://github.com/kolinz/emergency-drone-messenger/blob/master/program_image_1.PNG)  
   - ![case1](https://github.com/kolinz/emergency-drone-messenger/blob/master/example_use_1.PNG)  
1. You can use the "wish liist form" for evacuation shelters, by accessing a container that is separated from the drone.
The data of the “wish list form” are stored in the database of the cloud and can share information with the support base.
   - SourceCode [wishlist-form.json](https://github.com/kolinz/emergency-drone-messenger/blob/master/node-red/wishlist-form.json)
   - ![flow-image2](https://github.com/kolinz/emergency-drone-messenger/blob/master/program_image_2.PNG)   
   - ![case2](https://github.com/kolinz/emergency-drone-messenger/blob/master/example_use_2.PNG)  

## Software & Services
| Category | Name |  |
|:---|:---|:---|
|Software |Node-RED v0.19.4 |Install on Raspberry pi |
|IBM Cloud |Watson Text to Speech |https://console.bluemix.net/catalog/services/text-to-speech |
|IBM Cloud |IBM Cloudant |https://console.bluemix.net/catalog/services/cloudant |
|Node-RED nodes |node-red-node-watson |https://flows.nodered.org/node/node-red-contrib-speaker |
|Node-RED nodes |node-red-contrib-speaker |https://flows.nodered.org/node/node-red-contrib-speaker |
|Node-RED nodes |node-red-node-cf-cloudant |https://flows.nodered.org/node/node-red-node-cf-cloudant |
