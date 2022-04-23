# motion_config
Example motion config files for multiple cameras on a Rasperry Pi.

## Install motion
sudo apt install motion -y
sudo systemctl enable motion
mkdir /var/log/motion
chown -R motion:motion /var/log/motion

## Show devices
v4l2-ctl --list-devices

## Show device capabilities
v4l2-ctl --device /dev/video* --all

## restart service
sudo systemctl restart motion


