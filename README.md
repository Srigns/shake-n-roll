# Shake N'Roll

This GitHub repository hosts an innovative integration of facial keypoint estimation with an endless runner game using TensorFlow in Python and Unity in C#. The project leverages a ResNet50 architecture for facial keypoint detection, trained on the MPII dataset, to extract crucial facial landmarks. With these landmarks, the game interprets the player's facial movements and translates them into control signals for character movement within the endless runner environment.

## Project Highlights:

### Facial KeyPoint Estimation: 
  The repository includes Python scripts for preprocessing data, training the ResNet50 model, and demonstrating its effectiveness in detecting top head and chin keypoints.
### WebSocket Communication: 
  Python scripts enable real-time communication between the trained model and the Unity game engine through WebSocket, facilitating seamless integration of facial data into the game.
### Endless Runner Game: 
  Complete Unity project showcasing the endless runner game, where the character's movement is controlled based on the detected facial keypoints. Players can navigate the game environment by moving their head left, right, or keeping it centered.
### MPII Dataset Training: 
  Details of the MPII dataset used for training the facial keypoint estimation model are provided, ensuring transparency and reproducibility of the results.
### Comprehensive Documentation: 
  Detailed documentation guides users through setting up the project, training the model, integrating WebSocket communication, and running the Unity game. Additionally, explanations of the algorithm and its implementation are included to aid understanding.

## Documentation:

### Model Documentation (mode/README.md): 
  Details of data preprocessing, model architecture, training process, and model performance evaluation.
### Game Documentation (game/README.md): 
  Overview of the Unity project structure, implementation of character control using facial keypoints, and instructions for running and customizing the game.4
