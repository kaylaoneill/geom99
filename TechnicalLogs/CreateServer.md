# Start your own ArcGIS Server on GCP

## Step 1 - Get it Running
Time: Start: 1 hour (note: time started slower when trying to take notes and do the steps at the same time. Next time may be quicker)

- Go to: /console.cloud.google.com
- Click three lines on side
- ![image](https://github.com/kaylaoneill/geom99/assets/146447016/7aca9287-311e-4389-af17-a6f723f9f2ca)
- Go to compute engine and then VM Instances 
- Enable Compute Engine API (this can take a few minutes - let it load)
- TIP: make sure your billing is set up or this will not work

## Step 2 -Starting 
- Now that it is running:
- Click: create instance
- Name it: Name must consist of lowercase letters (a-z), numbers, and hyphens Name must start with a lowercase letter
- Set region and machine (for this we used: E2 medium)
- Set Boot Disk (for this we used:Windows - custome image given:allow HTTP and HTTPS Traffics)
- Hit create (this can take a few minutes)

  ## Step 3: Setting up the rules
  First Rule:
  - Firewall rule
  - Click: set up firewall rules
  - Create firewall rulew
  - Name it: make it something that makes sense
  - Ingree rule, allow action on match, targets: all instances
  - Add in your IP range (this is personal to your computer)
  - TCP port
  - Click create

 Second rule (once logged into machine)
  -Create a firewall rule by going to firewall in side menu and then following instructions above: allowing ports 6443 
  - In your server:
      - go into settings
      - firewall
      - inbound rules
      - Set up rules for ports you would like
      - Allow connection
      - click save 

## Step 4: Set up account
- Set password and username personal to you
- Will give you a password (copy this down)
- ![image](https://github.com/kaylaoneill/geom99/assets/146447016/65277e5f-4a18-4834-a9cd-c1b3e27f911b)

##  Step 5: Logging in
- Copy ip address (this changes everytime)
- In command: click Remote Deskptop
- Type in your unique IP (if using non standard port, do IP:PORTNUMBER: Example: 10.33.55.81:444)
- Connect
- prompt for username and password
- Put in what you set above - unique to you 
- Click Ok

- You will now be logged in
![Capture11](https://github.com/kaylaoneill/geom99/assets/146447016/069a91d0-eef8-4abe-b77d-975135c90a6a)

## Step 6: Shutting down
- There are two ways to shut down - do this when not using it to ensure you aren't billed.
  - Note that while shut down, you can't use the device or run the contents on it
 
- Way 1: Turn off using a Windows Desktop Console
- Similar to shutting down own computer
- Go to windows setting button in bottom left corner
- click the Power icon and then Shutdown.

- Way 2: On the console.cloud.google.com website
- Go to VM instances (instructions above on where to find this)
- Click the ... beside the VM option
- ![image](https://github.com/kaylaoneill/geom99/assets/146447016/acf82cd4-3a85-47af-a531-477e9fee01bf)
- Click stop.

- If you see this then your Virtual Machine is no longer running 
- ![image](https://github.com/kaylaoneill/geom99/assets/146447016/003b4114-37c3-419c-9dd2-257ef29bcaf7)

## View Rest Endpoint
- You can view the Rest Endpoint for this now by typing in https://IP/arcgis/rest/services
  - Remember this IP changes every time
- When the VM is running and your IP is current, you will see something like this:
- ![Capture12](https://github.com/kaylaoneill/geom99/assets/146447016/0b08a1c1-f3b5-486f-b940-c81290c11695)

