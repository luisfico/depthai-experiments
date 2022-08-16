First install dependences of

git clone https://github.com/luxonis/depthai.git
cd depthai
python3 install_requirements.py
python3 depthai_demo.py


For linux run

echo 'SUBSYSTEM=="usb", ATTRS{idVendor}=="03e7", MODE="0666"' | sudo tee /etc/udev/rules.d/80-movidius.rules

sudo udevadm control --reload-rules && sudo udevadm trigger







From

https://github.com/luxonis/depthai-experiments

https://github.com/luxonis/depthai-experiments/tree/master/gen2-camera-demo


Other source
official: https://github.com/luxonis/depthai.git


Install dependences

sh install5pythonLibsInVirtualEnv.sh




Run 
smb://naboo/dev%20log/TEMP/OAK-D/oak-d/codePy/depthai-experiments/gen2-camera-demo/main.py

to get color image, stereo images and point cloud



cd envPyOak/oakd/codePy/depthai-experiments/gen2-camera-demo

python3 main.py -pcl


The recorded data is stocked in:

/home/lc/envPyOak/oakd/codePy/data/

