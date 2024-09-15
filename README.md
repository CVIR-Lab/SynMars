# SynMars-Air

We release **SynMars-Air**, an all-terrain synthetic dataset for objects detection with viewpoint of Mars helicopter. It is an extension of our previous [SynMars-TW](https://github.com/CVIR-Lab/SynMars/tree/SynMars-TW) <sup>[1]</sup> dataset and contains 5 categories: big rock, small rock, bedrock, ridge,sand, and soil, all of which are labeled regardless of size, helping to more accurately assess the robustness of various object detection methods. Currently, SynMars-Air has a total of 11.700 labeled images with a resolution of 512 × 512 available for experiments. We divided them into 17,000 images for training, 1,500 for validation and 1,500 for testing. It was collected from a simulation environment generated by [Blender](https://wiki.blender.org/wiki/Main_Page), an open source and versatile 3-D computer graphics software allowing users to create and arrange 3-D objects. 
<div align=center>
  <img src=https://github.com/lumahuayuan/SynMars/blob/SynMars-Air/IMG/synmarsair.png width="40%" />
  <br>
  <strong>Fig.1.</strong>
  <em>An art scene with the Mars helicopter and the rover on SynMars-Air simulation platform.</em>
</div>


The simulated environment is a Mars-like terrain with an area of 300 x 300 m that is populated by thousands of rocks. We built this terrain by referring to objects' distribution photographed by Zhurong rover and Curiosity rover. The intrinsics and extrinsics of the camera were set according to those on the Ingenuity Mars helicopter such that the landform of SynMars-Air is closer to that of the real Mars dataset. Below is a comparison of partial scene images of SynMars Air and Ingenuity Mars helicopter from different perspectives.
<div align=center>
  <img src=https://github.com/lumahuayuan/SynMars/blob/SynMars-Air/Compare pictures.png width="20%" />
  <strong> Fig.2. </strong>
  <em> (a) - (c) is a comparison between some images of our SynMars Air and images captured by Ingenuity Mars helicopter probe</em>
</div>
In each scenario, as shown in Figure 3, the Mars helicopter collaborates with the Mars rover through a virtual camera for exploration. SynMars Air is capable of supporting various downstream visual tasks, including object detection, semantic segmentation, and 3D reconstruction. Referring to the Ingenuity Mars helicopter of Zhurong, its flight altitude is about 5 meters above the ground.
<div align=center>
  <img src=https://github.com/lumahuayuan/SynMars/blob/SynMars-TW/IMG/reverse_9_0053_l_image.png width="20%" />
  <img src=https://github.com/lumahuayuan/SynMars/blob/SynMars-TW/IMG/reverse_9_0053_l_mask.png width="20%" />
  <img src=https://github.com/lumahuayuan/SynMars/blob/SynMars-TW/IMG/reverse_9_0053_r_image.png width="20%" />
  <img src=https://github.com/lumahuayuan/SynMars/blob/SynMars-TW/IMG/reverse_9_0053_r_mask.png width="20%" />
  <br>
  <strong> Fig.3. </strong>
  <em> left to right: stero images and corresponding masks in SynMars-Air dataset</em>
</div>
Limited by the file size, we temporarily release 70 samples for the training set and 10 samples for both the validation and test sets.

Currently, you can download **SynMars-Air** samples, we will soon release all the data.

**Reference**  

[1] Xiong, Y., Xiao, X., Yao, M., Cui, H., & Fu, Y. (2024). Light4Mars: A lightweight transformer model for semantic segmentation on unstructured environment like Mars. ISPRS Journal of Photogrammetry and Remote Sensing, 214, 167-178.
