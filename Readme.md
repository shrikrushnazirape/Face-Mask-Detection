# Face Mask Detection

### Task 1 Detecting Masks
1. Detect faces using cvlib.detect_faces
2. Apply model to classifiy if the face is masked or not 


### Task 2 Detections of social distancing
3. Detect bounding boxes of person using cvlib.detect_common_objects 
4. calculate centroid for all boxes
5. feed these centroid to sklearn.DBSCAN to get the clusters.

### Multithreading 
Run both these tasks in 2 different threads.

### Display processed frames on Browser(Flask)
use streaming to stream the final frame from the app to the browser



## A Glimpse of the User Interface
#### Main Page
<img src="https://github.com/shrikrushnazirape/Face-Mask-Detection/blob/master/SS/ss1.png" height="350" width="800"/>
<img src="https://github.com/shrikrushnazirape/Face-Mask-Detection/blob/master/SS/ss2.png" height="350" width="800"/>

<p> 
So, here is a quick guide for setup on your PC and host run this project locally

### 1)Clone the project onto your local Machine (From the appropriate branch)
### 2)Create a virtual environment and install the required dependancies

install python3-env and pip for creating a environment

        sudo apt-get install python3-venv python3-pip


create a virtual envirnoment

        python3 -m venv env

activate this virtual environment

        source env/bin/activate

installing all required packages which are present in requirement.txt:

	    pip install -r requirements.txt


To run the program 

        FLASK_APP=stream.py flask run

