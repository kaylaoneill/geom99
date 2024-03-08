# Publishing and Registering data in Esri ArcGIS Server, on our own VM using ArcGIS Pro
Time: 45 minutes

## Step: Create Map 
- Design your map to be ready to be published
- ![1CreateMap](https://github.com/kaylaoneill/geom99/assets/146447016/06e7f1b4-a177-479f-bdd1-e7aea7486853)

## Step: Add new server connection
- On the top bar, click the connections button
- ![4addnewserver](https://github.com/kaylaoneill/geom99/assets/146447016/f0a63e3f-64d4-484f-a674-38931cbe4c3d)
- From the drop down, select "new  ArcGIS Server":
- ![Serverwindow](https://github.com/kaylaoneill/geom99/assets/146447016/410aa31a-ca60-4ffd-88ea-706ec55930bf)

- For this case, I used this URL: https://34.135.35.82:6443/arcgis/
- ![addconnections](https://github.com/kaylaoneill/geom99/assets/146447016/4b366cce-866e-498c-8866-63cf956d641f)
- Once your server URL, Username (left off screenshot) and Password are filled in, click "OK"
  - NOTE: Make sure your a user who can access this data when you log in
- If you want to double check it connected, look in your catelog pane
- ![7showsconnections](https://github.com/kaylaoneill/geom99/assets/146447016/923b195c-ae20-4099-8083-084a744033f4)
  - For this case. we understand cettificate is invalid and click ok
- If you did it correctly, when you right click on it, and there is a publish option

## Step: Publish a map service
- When you've right clicked on the service, click publish and clikc Map service
- Select which map you would like to publish
- ![9selectmap](https://github.com/kaylaoneill/geom99/assets/146447016/b2fe5c46-b8bd-4784-8748-0a74e6845de8)
- Click "ok" when you have the right map


## Step: Publish Map as a Map Server
- ![13Publish](https://github.com/kaylaoneill/geom99/assets/146447016/f1dc26c4-009c-4e49-81c6-2bf4055b2c86)
- Give it a name (will automatically have name as whatever your map was called, can change it- this is the name it will have when published)
- Add any summary and tags as needed
- Make sure it says "reference registered data"
- Double check the Server
- Decide if you want to put it into a folder or not
- Click Analyze
  
## Step Errors:
- A map server will not publish if there are errors. It will publish with warnings but it is a good idea to clear those. 
- An important one here is: "Layers data source is not registered with the server and data will be copied to server"
- ![11Gteridoferrors](https://github.com/kaylaoneill/geom99/assets/146447016/b94f1082-9448-4f8e-ac61-04b427f40ea7)
  - Right click
  - Have path to data on local computer
  - Have path to data on server
  - Give it a name
  - Resgister
  - ![13registerdata](https://github.com/kaylaoneill/geom99/assets/146447016/a2b1c06f-b117-4230-b2c2-9eb476678919)
- Re analyze
- If it was registered, this warning will dissapear:
- ![14NoWarnings](https://github.com/kaylaoneill/geom99/assets/146447016/1c2d9247-8bcc-4110-a5d3-a3758215bb7a)
- Click Publish
  - This can take a few minutes

## Step: Publish
-When it is finished publishing, you will get a complete note:
- ![16PublishSuccessful](https://github.com/kaylaoneill/geom99/assets/146447016/bf99c64e-23a2-477e-9027-0379989fc0c6)
-If you click the link attached to "Manage the map service" it will take you directly to where it is stored. 

## Explore Published 
- You can see through the REST that this was published to the server
![17publishproof](https://github.com/kaylaoneill/geom99/assets/146447016/3a4d36bb-27c7-4ff2-a233-d6c5e078d566)
- And if you click on ArcGIS JavaScript, you can see what the map looks like
- ![18PublishJava](https://github.com/kaylaoneill/geom99/assets/146447016/3b702359-19e9-448e-ab42-27476e13f1ac)

- NOTE: If you were to use this data now, remove the 6443 from the URL. 6443 should be for managing only
- ![19no6443](https://github.com/kaylaoneill/geom99/assets/146447016/8ee048aa-4f6e-49a1-9eb1-580a73cd07a6)
