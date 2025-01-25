# Apple-Inspired AI Calculator using Computer Vision and Generative AI

**Introduction**

The Apple-Inspired AI Calculator is an advanced project designed to tackle mathematical problems using cutting-edge technology. By leveraging Computer Vision through OpenCV and Generative AI via Google's Gemini AI, this calculator allows users to draw mathematical expressions directly on the screen. The AI model interprets these visual inputs to deliver accurate and detailed solutions, making complex calculations intuitive and accessible. Inspired by the functionality of the Apple iPad calculator, this project enhances user experience with sophisticated AI capabilities, providing both precision and ease of use.

<br />

**Table of Contents**

1. Key Technologies and Skills
2. Installation
3. Usage
4. Features
5. Contributing
6. License
7. Contact

<br />

**Key Technologies and Skills**
- Python
- Computer Vision
- OpenCV
- Pillow
- MediaPipe
- Google Gemini AI
- Numpy
- Streamlit

<br />

**Installation**

To run this project, you need to install the following packages:

```python
pip install opencv-python
pip install pillow
pip install mediapipe
pip install google-generativeai
pip install numpy
pip install streamlit
pip install streamlit_extras
```

<br />

**Usage**

To use this project, follow these steps:

1. Clone the repository: ```git clone https://github.com/gopiashokan/Apple-Inspired-AI-Calculator.git```
2. Install the required packages: ```pip install -r requirements.txt```
3. Add your Google API key to the `.env` file.
4. Run the Streamlit app: ```streamlit run app.py```
5. Access the app in your browser at ```http://localhost:8501```

<br />

**Features**

#### Live Webcam Feed:

   - **Webcam Initialization:** Utilizes OpenCV to initialize and access the webcam, enabling continuous capture of live video feed. This setup ensures real-time interaction with the user's input.

   - **Image Frame Processing:** Captures each image frame in the default BGR format and applies essential preprocessing steps. This includes resizing for uniformity, flipping for correct orientation, and converting to RGB format to align with the AI model’s input requirements.


#### Gesture Control with MediaPipe:

   - **Hand Gesture Detection:** Utilizes MediaPipe to identify and track hand gestures in real-time. This library enables precise detection of hand landmarks, allowing the system to interpret various finger movements and positions.

   - **Landmark Visualization and Extraction:** Draws landmarks on the detected hand and extracts the origin coordinates of each landmark. These coordinates are crucial for accurately recognizing gestures, which in turn control different functionalities within the application.


#### Gesture-Based Controls:

   - ✍️ **Draw Math Problems:** Draw mathematical problems by lifting the Thumb and Index fingers.
   - 🖱️  **Move Around:** Navigate the screen by lifting the Thumb, Index, and Middle fingers.
   - 🧽 **Erase Content:** Erase any mistakenly drawn content by activating erase mode by lifting the Thumb and Middle fingers.
   - 🗑️ **Reset Canvas:** Clear the entire drawing canvas by lifting the Thumb and Pinky fingers.
   - 📤 **Send to AI Model:** Submit the drawing for analysis by lifting the Index and Middle fingers.


#### Drawing and Blending:

   - **Canvas Management:** Establishes a dedicated drawing canvas that overlays the live video feed. This canvas allows users to draw mathematical problems directly onto the screen, providing a seamless and interactive experience.

   - **Image Blending:** Integrates the drawn content with the live video feed by blending both images. This process ensures that the user’s drawings are accurately displayed on top of the live feed, maintaining a clear and cohesive visual presentation.


#### Generative AI Integration:

   - **API Setup and Model Initialization:** Configures the Google Generative AI library by integrating it with a valid API key. Initializes the `Gemini 1.5 Flash` model, setting it up to process and analyze input data from the drawing.

   - **Solution Generation:** Sends the processed image along with the input prompt to the AI model. It generates detailed solutions for the mathematical problems depicted, providing accurate and comprehensive results based on the visual input.


#### Streamlit Application: 

   - **Interactive Interface:** Developed using Streamlit, this application offers a user-friendly and interactive interface. It seamlessly integrates all the project’s features, allowing users to easily interact with the AI calculator and perform tasks like drawing, gesture control, and viewing solutions.

   - **Real-Time Interaction:** The Streamlit application provides real-time feedback and updates, ensuring that users can see their drawings and results immediately. This dynamic interface enhances the overall user experience, making it intuitive and efficient to use the AI-powered calculator.

🎬 Project Demo Video: [https://youtu.be/HXFBbLOpn6I](https://youtu.be/HXFBbLOpn6I)


#### References:

   - Streamlit: [https://docs.streamlit.io/](https://docs.streamlit.io/)
   - OpenCV: [https://docs.opencv.org/4.x/d6/d00/tutorial_py_root.html](https://docs.opencv.org/4.x/d6/d00/tutorial_py_root.html)
   - Pillow: [https://pillow.readthedocs.io/en/stable/](https://pillow.readthedocs.io/en/stable/)
   - Mediapipe: [https://ai.google.dev/edge/mediapipe/solutions/vision/hand_landmarker](https://ai.google.dev/edge/mediapipe/solutions/vision/hand_landmarker)
   - Google Gemini AI: [https://ai.google.dev/](https://ai.google.dev/)

<br />

**Contributing**

Contributions to this project are welcome! If you encounter any issues or have suggestions for improvements, please feel free to submit a pull request.

<br />

**License**

This project is licensed under the MIT License. Please review the LICENSE file for more details.

<br />

**Contact**

📧 Email: gopiashokankiot@gmail.com 

🌐 LinkedIn: [linkedin.com/in/gopiashokan](https://www.linkedin.com/in/gopiashokan)

For any further questions or inquiries, feel free to reach out. We are happy to assist you with any queries.

