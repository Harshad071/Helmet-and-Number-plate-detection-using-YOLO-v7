# Real-Time Helmet and Number Plate Detection using YOLOv7

### This project focuses on real-time detection of helmets and vehicle number plates using the YOLOv7 model. The dataset is trained on Roboflow and consists of 3,000 images of helmets and 5,000 images of number plates, each categorized into different classes.

## Project Overview
YOLOv7 is utilized for object detection, providing a fast and accurate method for real-time detection.
A Flask-based web interface is implemented to allow users to upload images or videos for detection through a local server. The YOLOv7 model detects helmets and number plates in real time, returning the results (such as bounding boxes) via the web interface.

## Project Setup

### 1. Install YOLOv7
Clone the YOLOv7 repository from GitHub:

Copy code
### git clone https://github.com/WongKinYiu/yolov7
Open the YOLOv7 repository in VS Code or your preferred IDE.

### 2. Add Custom Python Files
After cloning the YOLOv7 repository, paste the following custom Python scripts into the YOLOv7 folder:

flaskaap.py
flaskaap1.py
flaskaap2.py
flaskaap3.py
hubconfCustom.py
hubconfcustomweb.py
These Python scripts set up the Flask web services, handle model interactions, and manage object detection requests.

### 3. Change Model Weights
Replace the model weights in the custom scripts (hubconfCustom.py and hubconfcustomweb.py) with the trained weights:

Change weights to epochs80.pt in these scripts.
If you have a different trained model (e.g., best.pt), you can replace it with your own dataset-trained weights.

### 4. HTML Files for the Web Interface
Paste the three provided HTML files into the templates folder within the YOLOv7 project. These files form the frontend for the Flask web interface.

You can customize the HTML files as needed, such as adding images or modifying the user interface to suit your requirements.

### 5. Run the Flask Application
To run the Flask application on your local environment:

Ensure Flask and all necessary libraries (YOLOv7 dependencies, Flask, etc.) are installed.
Run the Flask app locally to enable users to upload media files for detection.

## Additional Customization

You can modify the HTML templates or Flask scripts to fit your specific requirements. For example, you may adjust the web interface design, tweak detection thresholds, or add new features.
If you are training the model with a different dataset, replace the epochs80.pt file with your custom-trained .pt file from your YOLOv7 model.
