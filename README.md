# Flutter-PoseNet-TFlite

Integrating Mobile Camera for Real-Time Pose Estimation with Flutter, TensorFlow Lite, and PoseNet

Introduction 
Human Pose estimation is an important problem that has enjoyed the attention of the Computer Vision community for the past few decades. It is a crucial step towards understanding people in images and videos. Human Pose Estimation is defined as the problem of localization of human joints (also known as keypoints - elbows, wrists, etc) in images or videos. It is also defined as the search for a specific pose in space of all articulated poses. What about 2D and 3D pose estimations? 2D Pose Estimation - Estimate a 2D pose (x,y) coordinates for each joint from a RGB image. 3D Pose Estimation - Estimate a 3D pose (x,y,z) coordinates a RGB image.

Idea Presentation 

1. A Human Pose Skeleton represents the orientation of a person in a graphical format. Essentially, it is a set of coordinates that can be connected to describe the pose of the person. Each coordinate in the skeleton is known as a part (or a joint, or a keypoint). A valid connection between two parts is known as a pair (or a limb).
2. This works by providing 3D human pose estimation technology which detects keypoints on a human body like Left and Right hands, shoulders, elbows, neck base etc.
3. The process usually involves the extraction of joints on a human body, and then analysis of a human pose by deep learning algorithms.
4. There are several ways to develop the 3D human pose estimation system for fitness. The most optimal ways are training of a deep learning model to extract 3D or 2D key points from the given images/frames.
5. For the start and the end points indication, we can automatically detect the position of body control points by using arbitrary thresholds. For example, when squatting, it is possible to detect the angle of arms and position of hands by height, and then, by using arbitrary thresholds, we can detect the start and the end points of an exercise.

Technical Aspects
1. TensorFlow Lite-
TensorFlow Lite gives us pre-trained and optimized models to identify hundreds of classes of objects including people, activities, animals, plants, and places. 
2. Camera Plugin-
Using this plugin, we can capture the live feed provided by the mobile camera frame-by-frame. Then we can provide these frames as images to estimate the pose of a human.
3. PoseNet MobileNet V1
PoseNet is a deep learning model that allows us to detect the pose of a person based on where their joints are. The PoseNet model takes an image as an input and outputs an array of information about key points with a confidence score.
