# Cascade_Juggling
A computer vision pipeline for analyzing three-ball cascade juggling using ball tracking and 2D human pose estimation

It combines ball detection, hand tracking, body pose estimation, and spatial inconsistency analysis.

For hand tracking and body pose estimation, pre-trained AI models are used to identify hand positions, wrist movements, and body landmarks without needing to train new models.

For ball detection, a custom YOLO model is trained using a dataset created in Roboflow. Video frames are collected and uploaded to Roboflow, where each ball is manually labelled using bounding boxes. The annotated dataset is then exported in YOLO format and used to train the model to recognize juggling balls. Once trained, the model is saved as a .pt file and can be used to detect balls in new videos.
