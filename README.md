# Object-detection-in-Acoustic-Imagery
=> Implemented a YOLOv8-based object detection model on sonar (acoustic) images using the UATD dataset to detect underwater objects across 10 classes, addressing challenges such as noise, low visibility, and poor spatial resolution in underwater environments.
=>Input sonar images (640×640) pass through a CSPDarkNet backbone with convolutional layers, C3 modules, Spatial Pyramid Pooling (SPP), and E-LAN blocks to extract hierarchical feature maps from low-resolution, high-noise acoustic imagery.
=> A Feature Pyramid Network neck fuses multi-scale feature maps at P3, P4, and P5 scales, enabling the model to handle the diverse object sizes present across 10 underwater classes in the imbalanced UATD dataset.
=> A multi-scale detection head predicts bounding boxes, class probabilities, and objectness scores at three resolutions (20×20, 40×40, 80×80), optimized using CIoU loss for localization and cross-entropy for classification, achieving mAP@50 of 83.89% at 634 FPS inference.
<img width="521" height="836" alt="image" src="https://github.com/user-attachments/assets/65798686-e47e-4cc9-8132-3c52b9d28a1d" />
<img width="800" height="535" alt="image" src="https://github.com/user-attachments/assets/1b40a7db-c370-437c-b8dc-7d0fd29dd3e3" />
