### **Kidney Stone Detection Using YOLOv8**

A deep learning model to detect kidney stones in CT/X-ray medical images using the YOLOv8 object detection framework.



###### **🔬 Project Summary:**

This project uses YOLOv8 to detect kidney stones in medical imaging.

We trained the model on a labeled dataset containing bounding boxes for stones.



###### **Model Capabilities:**

Detect kidney stones

Mark exact stone location using bounding boxes

Count number of stones per image



###### **Visualize predictions**

How to Run the Project

1️⃣ Install Requirements

pip install ultralytics opencv-python-headless matplotlib



2️⃣ Train the Model

from ultralytics import YOLO

model = YOLO("yolov8n.pt")

model.train(data="data.yaml", epochs=50, imgsz=512)



3️⃣ Run Inference

model = YOLO("models/best.pt")

results = model("test\_image.png", show=True)



###### **📊 Results**

Achieved high accuracy on validation set

Detects stones with bounding boxes

Works on CT and X-ray images



###### **📁 Dataset**



Dataset source: [Kidney Stone Images with Bounding Box Annotations](https://www.kaggle.com/datasets/safurahajiheidari/kidney-stone-images?resource=download)

This dataset contains images and YOLO-style bounding box labels for kidney stone detection.



###### **🧠 Model Used**



YOLOv8 Nano for fast training and inference



Can be upgraded to YOLOv8s / YOLOv9 / YOLOv10

