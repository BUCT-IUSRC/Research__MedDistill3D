# Research__MedDistill3D
# MedDistill: Multi-Level Distilled Foundation-to-Lightweight Model Co-Learning for Unsupervised Medical Segmentation

<font style="color:rgb(0,0,0);">Te Guo, Yifan Huang, Tianyu Shen, </font> Kunfeng Wang<font style="color:rgb(0,0,0);"></font>

## Framework Overview
<img width="2830" height="1532" alt="overrall" src="https://github.com/user-attachments/assets/f73451c8-aa0e-4175-9c50-63749e6dee5a" />


<font style="color:rgb(0,0,0);">The overall framework of MedDistill3D.  A large-scale visual foundation model serves as a teacher to generate high-quality masks and guide a lightweight student network.  During weakly supervised training, Multi-level knowledge distillation aligns intermediate features and transfers structural information, while 3D hierarchical enhanced distillation supervises pseudo-volumes to correct 2D discontinuities and improve 3D segmentation continuity.</font>

## Install
### Environment
<font style="color:rgb(31, 35, 40);">The code is built with following libraries:</font>

+ <font style="color:rgb(31, 35, 40);">Python = 3.10</font>
+ <font style="color:rgb(31, 35, 40);">tensorflow = 2.19</font>
+ <font style="color:rgb(31, 35, 40);">h5py = 3.13</font>
+ <font style="color:rgb(31, 35, 40);">imageio = 2.37</font>
+ <font style="color:rgb(31, 35, 40);">keras = 3.10</font>
+ markdown = 3.5.1
+ <font style="color:rgb(31, 35, 40);">medpy = 0.5.2</font>
+ <font style="color:rgb(31, 35, 40);">nibabel = 5.3.2</font>
+ <font style="color:rgb(31, 35, 40);">opencv-python = 4.11</font>
+ <font style="color:rgb(31, 35, 40);">pandas =2.2.3</font>
+ <font style="color:rgb(31, 35, 40);">scikit-image = 0.25.2</font>

### <font style="color:rgb(31, 35, 40);">Training</font>
#### <font style="color:rgb(31, 35, 40);">1.Download Datasets</font>
<font style="color:rgb(31, 35, 40);">You can download the </font><font style="color:rgb(0,0,0);">public</font><font style="color:rgb(31, 35, 40);"> datasets using the following links: </font>

[http://medicaldecathlon.com/](http://medicaldecathlon.com/)
#### <font style="color:rgb(31, 35, 40);">2.Data preprocessing</font>
    --python preprocessing.py 
#### <font style="color:rgb(31, 35, 40);">3.Box Generation </font><font style="color:rgb(0,0,0);"></font>
    --pyhton box.py 
#### <font style="color:rgb(0,0,0);">4.Distillation network</font>
    --pyhton meddistill.py
#### <font style="color:rgb(0,0,0);">5.Test
    --python predict_eval.py 
### <font style="color:rgb(31, 35, 40);">Contact Us</font>
<font style="color:rgb(31, 35, 40);">If you have any problem about this work, please feel free to reach us out at te.guo@buct.edu.cn</font>`

