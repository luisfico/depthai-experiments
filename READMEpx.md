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



## Px Summary

C++ project
git remote add origin git@github.com:luisfico/depthai-core.git	     
(oak c++ running as example of library) OK get cloud from aligned 4Kimages with depth 400p. Min distance of deteccion=65cm   (Depth aligment with color camera performed by ISP oakd)

C++ project
git remote add origin git@github.com:luisfico/depthai-core-example.git  
(oak c++ isolated project ) ko get correct cloud  

Python project
git remote add origin git@github.com:luisfico/depthai-experiments.git   
(oak python get color ) OK get cloud from aligned stereo images 400p. Min distance of deteccion=35cm (no depth aligment with color camera. TODO)



## Node graph
+USAGE of depthai_pipeline_graph to see internal connection
+https://github.com/geaxgx/depthai_pipeline_graph
+run:    pipeline_graph run "python main.py -pcl"   