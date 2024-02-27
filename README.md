# Unity Raycast Navigation Project

This Unity project demonstrates a simple navigation behavior using Raycast. The main idea is to navigate towards a target (player) using the Unity NavMeshAgent while avoiding obstacles using Raycast detection.

## Features

- NavMeshAgent is used to move the object towards the player when within a certain range.
- Raycast detection is employed to avoid obstacles and change the direction of movement.
- Visualization of the detection range with a wireframe sphere (Gizmo).
- Rigidbody is used for forward movement when not navigating towards the player.

## Usage

1. Clone or download the project to your local machine.
2. Open the project in Unity.
3. Open the scene named `MainScene` in the `Scenes` folder.
4. Attach the script `Raycast.cs` to a GameObject in the scene.
5. Ensure the GameObject has a Rigidbody and NavMeshAgent component.
6. Set the target player by assigning the `player` variable in the inspector.
7. Tweak the `force` and `rotationSpeed` variables for movement behavior.
8. Run the scene (press the Play button) and observe the navigation behavior.

## Script Explanation

- **force**: Forward movement force when not navigating towards the player.
- **rotationSpeed**: Rotation speed when avoiding obstacles.
- **back**: Flag to determine if the object should move backward.
- **front**: Flag to determine if there is an obstacle in front of the object.
- **agent**: NavMeshAgent component for navigation towards the player.
- **player**: Target player's Transform.
- **OnDrawGizmosSelected()**: Draws a blue wireframe sphere around the object to visualize the detection range.
- **FixedUpdate()**: Handles the main logic for navigation and obstacle avoidance using Raycast.

## Contributing

Feel free to contribute to the project by opening issues or submitting pull requests.

## License

This project is licensed under the [MIT License](LICENSE).
