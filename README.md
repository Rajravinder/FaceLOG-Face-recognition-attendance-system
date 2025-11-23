# FaceLOG – Face Recognition Attendance System

FaceLOG is a Python plus OpenCV based attendance system that recognises faces via webcam and automatically records attendance in CSV format with timestamps.

![UI Preview](background.png)

## Features
- Register faces once
- Real time recognition using webcam
- Attendance saved as Name + Time in CSV
- Streamlit UI dashboard (`app.py`)
- Direct webcam script for capturing attendance (`test.py`)

## Project Structure
- add_faces.py - register faces  
- app.py - Streamlit dashboard (To view attendance)
- test.py - webcam attendance + evaluation  
- data/ - saved face encodings + labels + haarcascade  
- Attendance/ - generated CSV logs

## Installation
- git clone https://github.com/Rajravinder/FaceLOG-Face-recognition-attendance-system.git  
- cd FaceLOG-Face-recognition-attendance-system  
- pip install -r requirements.txt

### Create folders if missing:
- mkdir data  
- mkdir Attendance

## Usage
- Add faces (run once per person):
python add_faces.py

- Streamlit dashboard:
python app.py

- Webcam attendance capturing:
python test.py

- Attendance CSV files will appear in `Attendance/` automatically:
Attendance_DD-MM-YYYY.csv

## Tech Stack
- Python • OpenCV • Streamlit • scikit-learn • NumPy • Pandas  
- Model: KNN classifier  
- Detection: Haarcascade

## Future Improvements
- Switch to deep learning face embeddings
- Deploy online
- Admin login panel for institutions
- Cleaner UI for adding faces

## Author
Rajravinder Singh - https://github.com/Rajravinder
