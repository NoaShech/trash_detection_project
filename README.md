Trash Classification Web App 🌍🗑️

🇮🇱 סקירה בעברית
זוהי מערכת מבוססת דפדפן לזיהוי ומיון פסולת בזמן אמת בעזרת ראייה ממוחשבת ולמידת מכונה. המשתמש מצלם תמונה של אשפה בעזרת מצלמת הטלפון, והמערכת חוזה את סוג הפסולת ומציגה את התוצאה.

טכנולוגיות שבהן השתמשתי

Python

Flask – ליצירת שרת

YOLOv8 – לזיהוי אובייקטים בתמונה

רשת עצבית מסוג CNN – לסיווג סוגי פסולת

HTML / CSS / JS – לבניית הממשק

DroidCam – לחיבור מצלמת הטלפון לאתר- אפליקציה חינמית שצריך להוריד בכדי להתחבר למצלמה


איך להריץ את המערכת
הורידו את הקבצים או שבטו (clone) את הריפוזיטורי.

ודאו ש־Python 3.8 ומעלה מותקן.

צרו סביבת פיתוח וירטואלית והפעילו אותה:



python -m venv myenv

myenv\Scripts\activate  # Windows

התקינו את כל התלויות:


pip install -r requirements.txt

הורידו את הקבצים הכבדים (ראו למטה) והניחו אותם בתיקיות המתאימות:

TrashNet.zip – דאטה סט לסיווג פסולת

TACO.zip – דאטה סט עם תיוגים לזיהוי אובייקטים

trash_classifier_taco_cropped.h5 – מודל סיווג (CNN) מאומן

yolov8n.pt – מודלי YOLOv8 לזיהוי אובייקטים

הריצו את קובץ app_copy.py: שימו לב שאתם משנים את כתובת הIP לכתובת שלכם.



python app_copy.py

היכנסו בדפדפן לכתובת http://127.0.0.1:5000


🇬🇧 English Overview

This project is a web-based application for real-time trash classification and detection using computer vision and deep learning.
It enables users to capture images of trash using their phone camera and instantly receive predictions about the type of waste, helping sort it into the correct recycling bin.

Technologies Used
Python

Flask – for creating the backend web server

YOLOv8 – for real-time object detection

CNN model – for trash type classification

HTML/CSS/JS – for building the web interface

DroidCam – for connecting a mobile phone camera to the app - a free app you need to download in order to connect the camera

How to Run the Project
Clone the repository or download it as a ZIP and extract it.

Make sure you have Python 3.8+ installed.

Create and activate a virtual environment (recommended):


python -m venv myenv
myenv\Scripts\activate  # Windows

Install dependencies:

pip install -r requirements.txt

Download the missing large files (YOLO weights, .h5 model, datasets) from the links in the section below:

TrashNet.zip – Dataset for trash classification

TACO.zip – Annotated dataset for object detection

trash_classifier_taco_cropped.h5 – Trained CNN classifier model

yolov8n.pt – YOLOv8 detection models

Run the Flask app: make sure you change the IP address to yours


python app_copy.py

Open your browser at http://127.0.0.1:5000

Important Notes
Dataset Files: This repository does not include the full datasets and trained model files due to size limitations. To run the project end-to-end, you will need to download the following files manually:

TrashNet.zip - https://drive.google.com/file/d/16hYv82WGZg-vkeaCiR8z_574xvxjaL6v/view

TACO.zip - https://drive.google.com/file/d/1uiuchu3wh1U3eYxQWiyLfjDpZ8I-2sMG/view



יש לשים לב כי בקוד inference_pipeline_update_copy.py יש נתיבים לקישורים מקומיים. לכן, כדי להריץ את האתר בצורה מיטבית יש ללחוץ על הקישורים הבאים המורידים למחשב את המודלים:

https://drive.google.com/uc?id=1vIIqi_OrwfTcgFP4t6lj-17H-u05id9D

https://drive.google.com/uc?id=1H7asGr2dDOoKYifFS0yao4tmE03CR59O

שימו אותם בספרייה המקומית של הפרויקט שלכם, ותחליפו את השורות בקוד של הקישורים אל הנתיבים החדשים שלכם במקום ששמתם אותו.



Please note that the inference_pipeline_update_copy.py code contains paths to local links. Therefore, to run the site optimally, click on the following links that download the models to your computer:

https://drive.google.com/uc?id=1vIIqi_OrwfTcgFP4t6lj-17H-u05id9D

https://drive.google.com/uc?id=1H7asGr2dDOoKYifFS0yao4tmE03CR59O

Place them in your project's local directory, and replace the lines with the code for the links to your new paths where you put it.

