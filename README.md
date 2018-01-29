# bosh_lite_installer
Shell script(s) that automates the installation of bosh-lite.

When you play around with bosh as much as i do setting up a new environment every other day tends to become rather tedious.
To circumvent this slow erosion of my soul i started to created this shell script that will do most of the work for me.

Then i figured:"why not share this with the community?"

#### A word of warning!
There is much to learn from installing your own bosh-lite environment.
I would advise you to use this script once you are comfortable installing bosh-lite, and only use it for convenience.

## Requirements.
### Operating System.
Im developing this script on my macbook, there for it currently works on macOS, it should work on linux but your milage may vary.
I am planning on making this fully linux compatible.
Windows, meh... I might take a look at the "subsystem for linux" thingy but dont get your hopes up.
### Tools.
#### Git.
Seeing as you are probably reading this on github or from a cloned repo, i would be very surprised if you didnt have git installed already.
But just in case, get it here: 
https://git-scm.com/book/en/v2/Getting-Started-Installing-Git
#### VirtualBox
The amazing hypervisor that wil be hosting all those wonderfull bosh deployments.
Get it here:
https://www.virtualbox.org/wiki/Downloads
#### Bosh
Obviously we will be needing Bosh.
I am actually considering having the script install it if you dont have it yet, but for the time being.
Get it here:
https://bosh.io/docs/cli-v2.html#install

## Usage.
Clone this repository to a folder of your choosing, execute install.
On a new system it will simply setup bosh-lite on virtualbox.
When run again it will clean your bosh environment and set up a "clean" one.

## Sources.
bosh.io documentation:
http://bosh.io/docs
CloudFoundry bosh docs:
https://www.cloudfoundry.org/bosh/
Dr Nic's Ultimate guide to bosh:
https://ultimateguidetobosh.com

## Todo.
* Ensure the script works on both macOS and Linux.
* ~~work with vboxmanage to list and remove old vm's when needed.~~
* check for binaries and install or advise where to acquire.
