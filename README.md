# convnetart

You can run graphical programmes including full sessions on your EC2 machine with VNC.

This is useful for testing packages or collaborative working.

set up a Security Group with port 5900 - 5950 open (and 22 for ssh)
run an ec2 machine using that Security Group with an Ubuntu image - e.g. you can copy and paste the command from here if you have an account set up http://cloud-images.ubuntu.com/releases/14.04/release/

sudo apt-get update && sudo apt-get install kubuntu-desktop 

or you may prefer a lighter version

sudo apt-get update && sudo apt-get install --no-install-recommends lubuntu-desktop

Install tightVNC server

sudo apt-get install tightvncserver
run vncserver and set a password
on your local machine run krdc and connect to the EC2 machine and the port reported when running vncserver e.g. vnc://ec2-50-17-135-186.compute-1.amazonaws.com:5901
from your ssh login on the EC2 machine export DISPLAY=:1 and startkde
You can share the VNC details around if you want to work on something collaboratively such as running a tutorial.



ssh -i "virginia.pem" ubuntu@ec2-54-152-90-116.compute-1.amazonaws.com
sudo apt-get update && sudo apt-get -y upgrade && sudo apt-get -y install kubuntu-desktop && sudo apt-get install -y tightvncserver

tightvncserver ec2-54-152-90-116.compute-1.amazonaws.com
export DISPLAY=:1 
startkde



vncviewer ec2-54-152-90-116.compute-1.amazonaws.com:5091

 ec2-54-152-90-116.compute-1.amazonaws.com


sudo pip3 install --upgrade https://storage.googleapis.com/tensorflow/linux/gpu/tensorflow-0.7.1-cp27-none-linux_x86_64.whl




