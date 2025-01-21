# Distanced Peak

Sometimes you are in front of a desktop that isn't yours wishing somehow it could be. Lucky for us if you are using macOS, this situation is not a problem. With a little skill on Terminal and use of a first-party [Screen Sharing.app](https://support.apple.com/guide/mac-help/share-the-screen-of-another-mac-mh14066/mac) you have the ability to access your Desktop from anywhere.

### Step 1: Prepare Distance Machine

Unfortunately, you need a little foresight before using this ability as you must allow either Screen Sharing or Remote Management from Sharing settings.

### Step 2: Tunnel In

From the terminal of your distance machine enter in
- `ssh -L local_port:localhost:remote_port user@your_mac_ip`

Ex: `ssh -L 5900:localhost:5900 user@your_mac_ip`

### Step 3: Open Sesame

Open the Screen Sharing app on your Mac (use Spotlight search or go to Application/Utilities).

### Step 4: Sharing is caring

Connect to `localhost:5900`
