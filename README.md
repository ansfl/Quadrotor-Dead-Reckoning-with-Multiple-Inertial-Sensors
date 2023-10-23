# Introduction

This repository describes the dataset associated with our paper "Quadrotor Dead Recooking with Multiple Inertial Sensors".   

Quadrotors are widely used for surveillance, mapping, and deliveries. In several scenarios the quadrotor operates in pure inertial navigation mode resulting in a navigation solution drift.  To handle such situations and bind the navigation drift, the quadrotor dead reckoning (QDR) approach requires flying the quadrotor in a periodic trajectory. Then, using model or learning based approaches the quadrotor position vector can be estimated. We propose to use multiple inertial measurement units (MIMU) to improve the positioning accuracy of the QDR approach. Several methods to utilize MIMU data in a deep learning framework are derived and evaluated. Field experiments were conducted to validate the proposed approach and show its benefits. 

# Experiment Setup
The experiment platform was a DJI’s Phantom 4 quadrotor. This quadrotor has a RTK GNSS receiver providing our ground-truth trajectories. In addition, the quadrotor was equipped with four Xsens DOT IMUs to create the MIMU dataset for evaluations

![alt text](https://github.com/ansfl/Quadrotor-Dead-Recooking-with-Multiple-Inertial-Sensors/blob/main/2033_ISS_HurwitzKlein_Fig7.png?raw=true)

# Dataset
The datasets include the following recordings:

•	Straight lines trajectories: four trajectories with a total time duration of 66 seconds while the quadrotor had an average speed of 5.4 m/s. 

•	Horizontal periodic QDR trajectories: 27 trajectories with a total time duration of 16.1 minutes while the quadrotor had an average speed of 3.7 m/s.

•	Vertical periodic QDR trajectories: 31 trajectories with a total time duration of 12.6 minutes while the quadrotor had an average speed of 4.5 m/s.

In each trajectory includes 4 IMUs recording were made with a RTK-GNSS measurement severed as the ground truth (GT).  In the vertical periodic QDR trajectories 17 out of the 31 trajectories included a single IMU due to IMU failure during the experiments. 

An example of QDR trajectories vertical (side view) and horizontal (top view) trajectories can be seen in the figure below.

![alt text](https://github.com/ansfl/Quadrotor-Dead-Recooking-with-Multiple-Inertial-Sensors/blob/main/2033_ISS_HurwitzKlein_Fig8.png?raw=true)

# The Autonomous Navigation and Sensor Fusion Lab
The Autonomous Navigation and Sensor Fusion Lab (ANSFL) researches questions and challenges in the fields of autonomous navigation, inertial navigation systems, and estimation theory, as well as in related fields. Our research goals are to derive innovative inertial and sensor fusion algorithms, to develop novel inertial navigation system architectures, and to pioneer deep-learning-based navigation approaches.\
**Lab website**:  http://marsci.haifa.ac.il/labs/ansfl/ 
![Picture1](https://user-images.githubusercontent.com/93155156/143600162-787b7824-a863-46e2-ac19-ad6292a7c006.png)

# License
All datasets on this page are published under the [Creative Commons Attribution Version 4 License](https://creativecommons.org/licenses/by/4.0/legalcode)

# Cite Us
If you found the experimental DATA useful for your research, please cite our paper:

 @article{mimuquadnet2023,
  title={Quadrotor Dead Recooking with Multiple Inertial Sensors},   
  author = {Hurwitz, Dror and Klein, Itzik},   
  journal={arXiv preprint arXiv:2310.13452},   
  url = {https://arxiv.org/abs/2310.13452},   
  year={2023}
}
 ```
 
