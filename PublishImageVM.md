#Publish an Image in ArcGIS Pro through VM connection

## Step 1 - Turn on VM
Time: 15-30 minutes

- Make sure your VM is running and active.
- Go to: /console.cloud.google.com
- Click three lines on side
- Go to compute engine and then VM Instances
- Click on the three dots beside your VM
- CLick Start/Resume

## Step 2 - Add Server Connection
- Open ArcGIS Pro
- Start a new project
- On the top bar,  click connections, create a new connection, ArcGIS Server
- You will recieve this pop up:
- ![Serverwindow](https://github.com/kaylaoneill/geom99/assets/146447016/db9da531-165b-4ff0-b7b2-7376bef764c7)
- in Server URL, paste in your IP address, found on Google Cloud, on the main VM information:![image](https://github.com/kaylaoneill/geom99/assets/146447016/7a445744-1d8d-4f34-b649-37029b357beb)
  -This one is blank as the server was not running, but note this changes every time so this connection would need to be made every time
- Paste your External IP in with a /arggis at the end
- ![serverwindow2](https://github.com/kaylaoneill/geom99/assets/146447016/ff1ebf69-27a3-4a29-af56-9e1e9689386e)
- Put in your username and password
- For this case, we don't have SS certificate so click yes on the certification popup

## Step 3- Check server connection
- Inside Catelog view
- Go to Servers
- This is what the server looks like:
- ![Server](https://github.com/kaylaoneill/geom99/assets/146447016/7746ebd8-efa5-47af-a297-b9730bcf9660)

