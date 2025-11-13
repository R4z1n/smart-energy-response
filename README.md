# 🚗 **Accident Detection Using YOLOv8**

An AI-powered **real-time accident detection system** built using **YOLOv8**.  
This project detects road accidents in images and videos using a custom-trained YOLO model.

--------------------------------------------

## ✨ **Features**
- 🧠 **Custom-trained YOLOv8 accident detection model**
- 🗂 **YOLO-formatted dataset** (images + labels)
- 📒 **Training notebook included**
- 🎥 **Real-time & video accident detection**
- 🔳 **Bounding boxes + class predictions**
- 🖼 **Image detection using img.py**
- ▶️ **Video detection using main.py**
- 🎞 Includes multiple sample test videos

--------------------------------------------

## 📁 **Project Structure**

project/  
│── README.md  
│── yolo_model_training.ipynb  
│  
├── accident-detection/  
│   │── best.pt  
│   │── classes.txt  
│   │── main.py  
│   │── img.py  
│   │── cr.mp4  
│   │── test1.mp4 – test4.mp4  
│   │── yolo_model_training.ipynb  
│   │  
│   ├── data/  
│   │   ├── images/  
│   │   │   ├── training/  
│   │   │   └── validation/  
│   │   ├── labels/  
│   │   │   ├── training/  
│   │   │   └── validation/  
│   │   └── classes.txt  
│   │  
│   ├── images/  
│   └── .idea / .vscode  
│  
└── project/   # Unused (empty)

--------------------------------------------

## 🧠 **Model Training (YOLOv8)**

Training is done through:

`yolo_model_training.ipynb`

This notebook includes:
- 🗂 **Dataset preparation**
- ⚙️ **YOLOv8 configuration**
- 📊 **Training & validation**
- 💾 **Exporting best.pt**
- 🔧 **Fine-tuning workflow**

--------------------------------------------

## ▶️ **Running the Accident Detector**

### **1️⃣ Install Dependencies**
pip install ultralytics opencv-python numpy

### **2️⃣ Run Video-Based Detection**
python main.py  
(uses best.pt + test1.mp4 by default)

### **3️⃣ Run Image-Based Detection**
python img.py  
(update the image path inside the script if needed)

--------------------------------------------

## 🗂 **Dataset Format**

Each image has a YOLO label file:

image.jpg  
image.txt

Label format:
class x_center y_center width height

Dataset paths:
- accident-detection/data/images/
- accident-detection/data/labels/

--------------------------------------------

## 📦 **Model Weights**
- **best.pt** — custom-trained YOLOv8 model  
- Replace with new weights after retraining

--------------------------------------------

## 🛠 **Tech Stack**
- 🐍 Python  
- 🧠 YOLOv8 (Ultralytics)  
- 🎥 OpenCV  
- 🔢 NumPy  
- 📘 Jupyter Notebook  

--------------------------------------------

## 🚀 **Future Improvements**
- 🌐 Deploy via Flask / FastAPI  
- 📡 Real-time CCTV / RTSP support  
- 📈 Improve accuracy with larger dataset  
- 🆘 Accident severity classification  
- 🤖 Deploy on Jetson Nano / Raspberry Pi  

--------------------------------------------
