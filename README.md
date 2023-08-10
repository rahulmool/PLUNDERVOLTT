# PLUNDERVOLTT

# FANCONTROL
sudo systemctl disable apparmor

sudo dell-bios-fan-control 0

sudo modprobe i8k force=1

sudo gedit /etc/default/i8kbuttons

sudo gedit /etc/default/i8kmon

sed -i.bak 's/ENABLED=0/ENABLED=1/' /etc/default/{i8kmon,i8kbuttons}

sudo sed -i.bak 's/ENABLED=0/ENABLED=1/' /etc/default/{i8kmon,i8kbuttons}

/etc/init.d/i8kmon start

 2009  sudo i8kctl fan - 0
 
 2010  sudo i8kctl fan - 1
 
 2011  sudo i8kctl fan - 2
