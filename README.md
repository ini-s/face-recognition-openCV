Face Detection Project 👨‍💻


This project demonstrates face detection in both static images and real-time video streams using Python's OpenCV library. It employs a pre-trained Haar Cascade classifier to accurately identify and draw bounding boxes around faces.

🖼️ Face Detection in Images
The first part of the script identifies faces in a static image file named multiple_faces.jpg. It performs the following key steps:

Loads the image: The image is read into the program using cv2.imread().

Converts to grayscale: The image is converted to grayscale to simplify the detection process, as the Haar Cascade classifier works best with grayscale images.

Detects faces: The cv2.CascadeClassifier is used with the pre-trained haarcascade_frontalface_default.xml model to detect face coordinates.

Draws bounding boxes: A green rectangle is drawn around each detected face to highlight its location.

Displays the result: The final image with the bounding boxes is displayed using matplotlib.

🎥 Real-Time Face Detection
The second part of the script enables real-time face detection using a device's default camera. This is a more dynamic application of the same core technology and follows these steps:

Initializes video capture: The script accesses the default camera (cv2.VideoCapture(0)) to read video frames.

Processes frames continuously: A while loop continuously reads frames from the video stream.

Detects and draws: For each frame, the detect_bounding_box() function is called. This function converts the frame to grayscale, detects faces, and draws a red bounding box around each one.

Displays the live feed: The modified video frame with the bounding boxes is displayed in a window titled 'Face detection project'.

Exits gracefully: The program can be exited by pressing the 'q' key.

⚙️ Requirements
Python 3.x

OpenCV (cv2)

Matplotlib (matplotlib)
