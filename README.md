Task: integrate YOLOv5 into Portfolio 1
Integrating yolov5_ros with portfolio tasks 1 and 4 involves incorporating the YOLOv5 object detection capabilities into a ROS 2 environment. Additionally, you should create a ROS publisher node to publish video frames to the /image_raw topic, and adapt YOLOv5 to detect traffic signals using the provided GitHub repository.
1. Create a ROS Publisher for Video Frames
Create a ROS Publisher Node: Develop a ROS 2 node that reads video frames from a specified file or camera and publishes them to the /image_raw topic. You can use the code from Lab 6 as a reference and modify it according to your requirements.
Test the Publisher Node: Verify that the publisher node works correctly by running it and subscribing to the /image_raw topic to visualise the published frames.
2. Adapt YOLOv5 for Traffic Signal Detection
Learn about YOLOv5: Read the details about YOLOv5 here .
Download the Repository: Obtain the road signs dataset from here  and train it for YOLOv5s [small].
Understand how to train YOLOv5 on Roboflow: Check this article on how to train datasets on Roboflow here .
Modify as Needed: You will have to modify and adapt the yolov5_ros package to use the newly trained weights and configuration files.
Test the Adapted Model: Once you've made the necessary modifications, test the adapted YOLOv5 model to ensure that it performs accurately for traffic signal detection.

Report Section Requirements
As mentioned above, you will need to write up a text detailing what you did and why, your results and the background concepts behind the techniques you used for your solution. This text will be included as Section 5 of a final report you will submit on your overall portfolio work (see the full requirements for the final report in the Portfolio Specifications Document here).  You should be aiming towards writing a section that should not be more than 12 pages long. The text must not contain any code snippets. To describe code, use code design illustration languages such as UML.
Here is the recommended structure and numbering for the respective report section:
5. Navigation with ROS2 in Gazebo Simulation
5.1 Introduction
•	Brief background on NNs, CNNs and object detection
•	Objectives
5.2 Background
•	Short overview of object detection strategies using deep learning
•	Discussion of approaches for object detection, including a feature comparison table
5.3 System Design
Here you should include all information required for your marker to understand what you implemented. You will need to include at least the following:
•	High-level architecture diagram of the system
•	Discussion of key ROS2 packages used and justification for chosen navigation and collision avoidance algorithms
•	Explanation of key nodes, topics and/or services
It is recommended that you also include the following details:
•	UML diagrams showing class structures and interactions
5.4 Results
Here you should include all information required for your marker to understand how you evaluate the performance of your solutions. You are expected to cover the following topics:
•	Description of test scenarios and results
•	Analysis of object detection performance
•	Limitations and potential improvements
5.5 Conclusion
•	Summary of work completed
•	Assessment of objectives achieved given results
5.6 References
•	Your reference list.
