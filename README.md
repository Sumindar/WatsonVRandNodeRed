# Watson Visual Recognition and Node-Red

Simplify calorie counting using the power of IBM Watson Cognitive Services. IBM Watson Visual Recognition food model provides a built-in capability for recognising 2,000+ different foods globally, which is perfectly suited to replace the manual process of food logging with automatic food identification using image recognition.

In this lab, you will create a calorie counter web app using Node-RED, Watson Visual Recognition and Nutritionix API. This web app analyses food images using Watson Visual Recognition service and extract nutritional information of the food analysed using Nutritionix API (The largest verified database of nutritional information

![](img/flowdiagram.png)

## Pre-requisites:

1. Create an [IBM Cloud](https://cloud.ibm.com/login) account

## Steps:

1. Login to IBM Cloud, create a ``Node-Red`` service instance. (Name the instance, click create/next to finish the instance creation)

![](img/instancecreateNR.png)

2. Go to ``Resource list`` on from cloud page and open Node Red application from Cloud Foundry Applications. Then click on ``visit app url``.

![](img/visitappurl.png)

3. Click on ``Next`` till the application is created.

![](img/noderednext.png)

4. Click on ``Go to your Node-Red flow`` editor

![](img/nrvisitapp.png)

5. Click on the right corner of the screen and click on ``import``.

![](img/nrimport.png)

6. Go to https://raw.githubusercontent.com/rachana5198/WatsonVRandNodeRed/master/Node-Flow in a new tab and copy the flow. Head back to Node-red and paste this flow.

![](img/nrimport1.png)

7. Double click on the ``visual recognition`` node in the flow.

![](img/flowvrnode.png)

8. Head back to IBM Cloud, search for ``Visual Recognition`` service or find it under AI services. Click on it.

![](img/instancecreateVR.png)

9. Click on ``create``

![](img/instancecreateVR-1.png)

10. On the left side of the screen, click on ``service credentials``.

![](img/servicecredVR.png)

11. Click on view credentials under ``Auto-generated credentials`` and copy the ``apikey`` without ""

![](img/apikeyVR.png)

12. Head back to Node-Red flow editor and paste it in the visual recognition node. Click on ``Done`` which closes the node properties.

![](img/nrcopyapivr.png)

13. On the right corner of the screen, click on ``Deploy``

![](img/nrdeployflow.png)

14. Copy the url of the node-red flow editor until domain extension which will look something like this https://YOUR_APP_NAME.eu-gb.mybluemix.net/ and add foodDetails to the link which will look something like this https://YOUR_APP_NAME.eu-gb.mybluemix.net/foodDetails. Open this url in a new tab.

![](img/nrurlcopy.png)

15. You will be landed on a page that looks something like this. Select an image from web or select one of the images from the ui, copy the image location or ``image address`` and paste it in the text box below.

![](img/output01.png)

16. Click on ``Analyze`` and you will see the image recognised by watson and also the calorie details in the food image.

![](img/output02.png)

### Congragulations!! You have now completed a minilab on Watson Visual Recognition and Node Red Starter Kit on IBM Cloud, finish the task below and meet us at Novus Launch to grab IBM Swag kits.

## Task:
1. Add on top of the node red application that you have created.
2. Create a simple dashboard that displays the calories consumed and suggests exercise to be done to burn the calories.

HAPPY CODING!!
