# surfacego-chromeos

fix bluetooth chrome os
sudo su
sudo sh -c "echo 1 > /sys/module/bluetooth/parameters/disable_ertm"

cd /media/removable/SD\ Card

Create chromeos.img
sudo bash install.sh -src rammus.bin -dst chromeos.img -s size

sudo mount -o remount,exec /media/removable/SD\ Card
