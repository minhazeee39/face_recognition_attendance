# Face Recognition Attendance System
This project implements a face recognition-based attendance system using Python, OpenCV, and machine learning techniques. The system captures and recognizes faces in real-time, marking attendance in a CSV file with timestamps. This is an ideal solution for environments like classrooms or offices where automatic and reliable attendance tracking is needed.

# Features
Real-time Face Detection: Uses OpenCV's Haar Cascades to detect faces in a live video stream.
Face Recognition: Identifies registered faces using a K-Nearest Neighbors (KNN) classifier.
Automated Attendance Logging: Logs attendance in a CSV file with the person's name and timestamp.
Voice Notification: Confirms attendance with a voice message.
Data Persistence: Saves face encodings and names for future recognition.
Project Structure
README.md: Documentation for the project.
add_faces.py: Script to add new faces to the system.
attendance_<date>.csv: CSV files where attendance records are saved.
faces_data.pkl: Serialized file containing face encodings.
names.pkl: Serialized file containing names associated with face encodings.
haarcascade_frontalface_default.xml: Haar Cascade model for face detection.
test_face_recognition.py: Main script to run the face recognition attendance system.
Installation
Clone the repository:
git clone https://github.com/minhazeee39/face_recognition_attendance.git
cd face_recognition_attendance
Install the required packages:
pip install opencv-python numpy scikit-learn pywin32
Ensure the Haar Cascade model is in the correct directory.

The haarcascade_frontalface_default.xml file should be placed in the same directory as your scripts.
Usage
# Adding Faces to the System:
Run add_faces.py to capture and store face encodings in faces_data.pkl.  
Follow the on-screen instructions to add a new person’s face and name.  
python add_faces.py  
Running the Attendance System:  
Execute test_face_recognition.py to start the live face recognition system.  
The system will detect, recognize, and log attendance when the 'o' key is pressed. 
python test_face_recognition.py  
Viewing Attendance Records:  
Attendance is saved in CSV format (e.g., attendance_<date>.csv).
Open the CSV files to view attendance records for specific dates.
Voice Notification
The system uses Windows' built-in text-to-speech functionality to announce that attendance has been taken successfully. This feature requires the pywin32 package.

# Future Enhancements
Improve Recognition Accuracy: Incorporate deep learning models for better accuracy.
GUI Interface: Develop a graphical user interface for easier interaction.
Email Notifications: Send email notifications for attendance records.
Database Integration: Store attendance records in a database for better management.
# License
This project is licensed under the MIT License - see the LICENSE file for details.

