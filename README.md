# AI-Enabled Responsive Toy (ART) for Infant Comfort

## Project Overview
AI-Enabled Responsive Toy (ART) is an AI-powered interactive toy designed to respond to a baby’s crying by generating calming sounds, helping to soothe and comfort the baby. The toy utilizes a machine learning model that detects whether a baby is crying and responds accordingly. The project aims to combine technology and child play, creating a smart toy that provides both entertainment and emotional support.

## Features
- **AI-Powered Cry Detection**: Uses a custom-built machine learning model to detect baby cries with high accuracy.
- **Calming Sounds**: Automatically plays soothing sounds, such as lullabies or white noise, to comfort the baby.
- **Real-Time Response**: The toy responds immediately after detecting the baby’s cry, ensuring timely intervention.
- **Interactive Design**: The toy’s body is designed for durability and safety, making it suitable for infants.

## Technologies Used
- **Machine Learning**: Custom Convolutional Neural Network (CNN) model to classify baby crying sounds.
- **Hardware**: Raspberry Pi 4, microphones, speakers, and motors for sound output and movements.
- **Programming Languages**: Python for data processing and machine learning model deployment.
- **Design Tools**: SolidWorks and Blender for designing the toy's structure, ensuring safety and ease of assembly.
- **Development Environment**: TensorFlow Lite for model deployment on Raspberry Pi.

## Project Setup

### Hardware Requirements
- Raspberry Pi 4 Model B
- Speaker/Buzzer
- Microphone Module
- LCD Display
- LED lights
- SD Card (64GB)
- Jumper wires (Male-to-Male, Female-to-Female)

### Software Requirements
- Raspberry Pi OS (64-bit)
- Python 3.x
- TensorFlow Lite
- Libraries: `sounddevice`, `NumPy`, `OpenCV` (for real-time processing)

### Model Training and Deployment
1. **Data Collection**: Collected over 500 samples of baby cries for training the model. Audio data was preprocessed by resampling to 16kHz and converted into spectrograms.
2. **Model Architecture**: Built a CNN using TensorFlow to classify baby cry audio data. The model achieved high accuracy and was compressed into TensorFlow Lite format for deployment.
3. **Deployment on Raspberry Pi**: The model runs on Raspberry Pi with real-time audio processing. The microphone captures sounds, which are processed by the model to determine if the baby is crying.

## Usage Instructions
1. **Set up Raspberry Pi**: Flash Raspberry Pi OS onto the SD card, enable SSH, and configure Wi-Fi. Install required libraries for TensorFlow Lite and audio processing.
2. **Run the Toy**: Connect the microphone and speaker to the Raspberry Pi. Run the Python script to continuously monitor and classify sounds in real-time.
3. **Output**: When the toy detects a baby’s cry, it will immediately play calming sounds and can perform simple movements (e.g., waving or nodding) if motorized.

## Testing
- The toy has been tested with various baby cry samples in different environments, including noisy and quiet settings.
- It performed well under varied conditions, achieving over 90% accuracy in detecting baby cries and delivering a timely response.

## Future Improvements
- **Enhancing Sound Variety**: Adding a library of diverse sounds to keep the baby entertained and comforted.
- **Mobile App Integration**: Allow caregivers to control the toy remotely and monitor its responses via a mobile application.
- **Voice Recognition**: Implementing voice recognition to detect the baby’s name and respond accordingly.

## Contributors
- Krishan Kant
- Sanskar Mittal
- Abhishek Meena
- Manish Kumar Meena

## Supervisor
- Dr. Chandrakant Kumar Nirala, Department of Mechanical Engineering, Indian Institute of Technology, Rupnagar
