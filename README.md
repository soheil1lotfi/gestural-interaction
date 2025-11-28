# Gestural Interaction Web Conference

A web-based video conferencing application that enables gesture-based control using computer vision. Control meeting functions with hand gestures instead of clicking buttons.
Our presentation for the project: [click here!](https://docs.google.com/presentation/d/1H7tZ7pJ5NnbabZnrdReIxsonTODeJKEz8kQgwL_EKTk/edit?usp=sharing)

## 🎯 Goal

Create a web conference application with the possibility of gestural interaction in order to enhance the experience with online meetings.

## 💡 Motivation

After 2019 the use of online meeting services saw a tremendous surge. Online meetings differ from real-life conversations and therefore, specific user interface elements have been designed to be used in order to capture users' reaction to the content they are presented with without actually expressing them physically (through emojis, symbols, icons, etc.). 

We decided to explore the possibility of bringing back the physicality of these reactions through AI and Computer Vision algorithms. The physicality might improve the engagement of the users and also help certain communities to interact easier with these systems.

## Features

- Real-time hand gesture recognition via webcam
- Touch-free interaction for meeting controls
- Supported gestures: 
  - ✋ Open Palm (raise hand)
  - 👍 Thumbs Up
  - ✌️ Victory sign
  - 👎 Thumbs Down
- Local processing - no data sent to external servers

## Tech Stack

- Flask (Python backend)
- Google MediaPipe (gesture recognition)
- OpenCV (video processing)
- HTML/CSS/JavaScript frontend

## Installation

1. Clone the repository:
```bash
git clone https://github.com/soheil1lotfi/Gestural-Interaction.git
cd Gestural-Interaction
```

2. Install dependencies:
```bash
pip install flask opencv-python mediapipe numpy
```

3. Download the MediaPipe gesture recognition model:
   - Get `gesture_recognizer.task` from [MediaPipe Models](https://developers.google.com/mediapipe/solutions/vision/gesture_recognizer)
   - Update `model_path` in `Flask.py` to your model location

4. Run the application:
```bash
python Flask.py
```

5. Open browser to `http://localhost:5000`

## Usage

- Allow camera access when prompted
- Position hands within camera frame
- Hold gestures for 1-2 seconds for detection
- Good lighting improves accuracy

## Project Context

Developed for **HCI922 - Gestural and Mobile Interaction** course. This is a demonstration prototype showing how gesture-based interaction can be implemented in real-world video conferencing applications.

**Real-World Implementation**: After this project's development, similar gesture recognition features were implemented by major platforms:
- **Instagram Stories** (iOS 17, September 2023): Added gesture-based reactions allowing users to trigger effects like hearts, thumbs up/down, and fireworks through hand gestures
- **Apple FaceTime** (iOS 17, September 2023): Introduced gesture-based reactions for video calls with AR effects
- **Meta Video Calling Apps** (2023-2024): Rolled out gesture control features across their platform ecosystem

This project demonstrates the viability and user interest in gesture-based controls for video communication - a concept that has since been validated by mainstream adoption.

## License

MIT License - see [LICENSE](LICENSE) file for details.

## Authors

- Soheil Lotfi
- Alina Sarzhanova

---

*Research prototype developed for educational purposes as part of an HCI course project.*
