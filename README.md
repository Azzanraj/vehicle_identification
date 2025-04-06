🚗 Vehicle Classification using YOLOv8 and Flask
This project implements real-time object detection and classification (with a focus on vehicles) using YOLOv8 and a Flask web application interface. It allows users to upload video files or use a webcam to detect and classify objects like cars, trucks, buses, motorbikes, and more.

📌 Features
🔍 Real-time Object Detection using Ultralytics YOLOv8

📹 Supports Video Uploads for object detection

🎥 Live Webcam Feed for real-time detection

🌐 Flask-based Web Interface

💾 Session-based video handling

📦 Modular code structure

🧠 Model
The project uses the YOLOv8n (Nano) model from Ultralytics, which is lightweight and ideal for real-time applications on low-resource devices.

🖼️ Object Classes
YOLOv8 supports 80 COCO classes. Some of the key vehicle-related classes used:

🚗 Car

🚌 Bus

🚛 Truck

🏍️ Motorbike

🚲 Bicycle

📁 Project Structure
bash
Copy
Edit
├── app.py                  # Flask application
├── YOLO_Video.py           # Video processing and detection logic
├── templates/
│   ├── indexproject.html   # Home page
│   ├── ui.html             # Webcam interface
│   └── videoprojectnew.html # Video upload interface
├── static/
│   └── files/              # Uploaded video storage
├── requirements.txt        # Python dependencies
└── README.md               # Project documentation
⚙️ Installation
Clone the repository

bash
Copy
Edit
git clone https://github.com/yourusername/vehicle-classification-yolov8-flask.git
cd vehicle-classification-yolov8-flask
Set up a virtual environment (optional)

bash
Copy
Edit
python -m venv venv
source venv/bin/activate   # On Windows: venv\Scripts\activate
Install dependencies

bash
Copy
Edit
pip install -r requirements.txt
Download YOLOv8 Weights Download YOLOv8n weights from Ultralytics and place it in a folder named YOLO-Weights.

🚀 Usage
Run the Flask App

bash
Copy
Edit
python app.py
Navigate to the Web App Open your browser and go to: http://127.0.0.1:5000

Choose your mode

📤 Upload a video (FrontPage button)

📷 Use your webcam (Webcam button)

🧪 Demo
Mode	Screenshot
Video Upload
![5 1](https://github.com/user-attachments/assets/ca76e832-36dd-4872-b2f6-7eadaee9b902)
![5 2](https://github.com/user-attachments/assets/ac8073da-36fe-464c-b340-84809527cd82)

Webcam Stream	
📦 Requirements
Python 3.7+

OpenCV

Flask

Flask-WTF

WTForms

Ultralytics (YOLOv8)

Install all using:

bash
Copy
Edit
pip install -r requirements.txt
📌 Notes
The application uses session storage to manage uploaded files.

It reads frames from video/webcam and sends them as MJPEG stream to the front end.

Object detection runs in a generator for smooth streaming.

🙌 Contributing
Feel free to fork the repo, make changes, and create a pull request. Contributions are welcome!
