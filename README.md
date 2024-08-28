<h2>Object Detection and Classification Using Pre-Trained Models</h2>
This project involves performing object detection and classification on a set of input images using the following pre-trained models:

**1. Faster R-CNN with FPN:**
Faster R-CNN (Region-based Convolutional Neural Network) with FPN (Feature Pyramid Network) model looks at an image in two steps: first, it finds potential objects, and then it closely examines those areas to identify what they are. The FPN helps it see both big and small objects more clearly.

**2. YOLOv8:**
YOLOv8 (You Only Look Once, version 8) is like a quick scanner that can look at an image and instantly tell you what objects are in it, all in one go. It’s built to be fast and accurate, even better than its earlier versions.

**3. YOLOv5 Fog:**
YOLOv5 fog model is a specialized version of the YOLOv5 object detection model, designed to handle images with foggy or hazy conditions. It adapts the standard YOLOv5 architecture to improve detection accuracy in low-visibility environments by incorporating techniques like dehazing or enhancing features that are often obscured by fog.

**Differences:**
<br>> **_Steps:_** Faster R-CNN checks the image twice (finds objects, then identifies), while YOLO models do it all at once.
<br>> **_Speed:_** YOLOv5 and YOLOv8 are faster and better for tasks where speed is crucial, like real-time video.
<br>> **_Detail:_** Faster R-CNN with FPN is better at spotting small details, while YOLO models focus on speed.


<h3>Process Overview</h3>

**i) Input Images:**
<br> Place the images you want to process in a designated folder (/input/).
<br> **ii) Model Iteration:**
<br> The script will iterate over each image in the folder.
<br> For each image, the object detection and classification will be performed using the pre-trained models listed above.
<br> **iii) Detection and Display:**
<br> For each image, the model will generate bounding boxes around detected objects.
<br> The detected objects will be classified, and their names will be displayed on the image along with the bounding boxes.
<br> **iv) Saving the Output:**
<br> The processed images (with bounding boxes and object names) will be saved in separate folders inside the output folder named after each model (e.g., /output/model_output/).

<h3>Folder Structure</h3>
> _/input/:_ Contains the input images to be processed.
<br>> /_output/faster_rcnn_output/:_ Contains the output images processed by the Faster R-CNN with FPN model.
<br>> _/output/yolov8_output/:_ Contains the output images processed by the YOLOv8 model.
<br>> _/output/yolov5_fog_output/:_ Contains the output images processed by the YOLOv5 model.
