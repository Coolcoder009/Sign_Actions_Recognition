# Sign Actions Recognition<br>

Sign language recognition is a technology that aims to interpret and understand sign language gestures performed by individuals, typically those who are deaf or hard of hearing. This technology involves the use of computer vision and machine learning algorithms to analyze and interpret the movements and positions of a person's hands, fingers, and other relevant body parts during sign language communication. By capturing and processing these gestures, sign language recognition systems can convert them into text or spoken language, enabling communication between individuals who use sign language and those who may not be familiar with it. This technology plays a crucial role in bridging communication gaps and promoting inclusivity for the deaf and hard of hearing communities.<br>




## Installation

1. Clone the repository 
```bash 
git clone <repository-url>
cd <repository-directory>
```

2. Create a virtual environment and activate it:
```bash
python -m venv venv
source venv/bin/activate   # On Windows, use `venv\Scripts\activate`
``` 

3. To install the required dependencies, run the following command:
```bash
pip install -r requirements.txt
```

## How It Works
### Algorithms Used
Using mediapipe framework the keypoints are captured in the form of .npy file and then it is fed into LSTM model. LSTM model is used here to recognize sequential actions.<br>

### Libraries Used

The project utilizes several Python libraries for image processing, machine learning, and deep learning:

<ul>
<li><strong>cv2 (OpenCV):</strong> For capturing video streams and image processing.</li>
<li><strong>numpy:</strong> For numerical operations.</li>
<li><strong>matplotlib:</strong> For plotting images and graphs.</li>
<li><strong>mediapipe:</strong> Provides holistic and hand tracking models for landmark detection.</li>
<li><strong>tensorflow:</strong> For building and training deep learning models.</li>
<li><strong>sklearn:</strong> For data preprocessing and model evaluation.</li>
</ul>

### Model Training

The project employs LSTM (Long Short-Term Memory) networks to classify sequences of hand gesture keypoints extracted from video frames.

### Example Usage
Running the Live Camera Prediction
To predict hand gestures in real-time using the trained model, execute:

```bash 
python Sign_Action_Recognition.py
```


### Results
 When inference done on live camer, the classes are predicted and printed on the window.