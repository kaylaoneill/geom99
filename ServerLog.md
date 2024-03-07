#Start your own ArcGIS Server on GCP

## Step 1 - Get it Running
Time: Start: 8:15, end: 9:15 (note: time started slower when trying to take notes and do the steps at the same time. Next time may be quicker)

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

##  Step 5: Logging in
- Copy ip address (this changes everytime)
- In command: click Remote Deskptop
- Type in your unique IP (if using non standard port, do IP:PORTNUMBER)
- Connect
- prompt for username and password
- Put in what you set above
- Click Ok

- You will now be logged in 
