# Autonomous Maze-Solving Robot

An intelligent autonomous robot capable of navigating and solving mazes using the LSRB (Left-Straight-Right-Back) algorithm, with additional manual control capabilities via Bluetooth.

## 🚀 Features

- **Autonomous Navigation**: Implements the LSRB algorithm for efficient maze-solving
- **Manual Control**: Bluetooth-enabled remote control capability
- **Adaptive Decision Making**: Real-time sensor-based navigation
- **Efficient Pathfinding**: Minimizes travel time through optimized routing
- **Multiple Operation Modes**: Switch between autonomous and manual control

## 🛠️ Hardware Requirements

- Arduino Uno (Central Control Unit)
- 3x Ultrasonic Sensors (HC-SR04)
- Motor Driver (L298N)
- DC Motors (2x)
- Bluetooth Module (HC-05)
- Power Supply
- Chassis and Wheels

## 📋 Prerequisites

- Arduino IDE
- Basic understanding of Arduino programming
- Bluetooth Serial Terminal App (for manual control)

## 🔧 Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/Maze-Solving-Bot.git
   ```

2. Open the Arduino IDE

3. Navigate to `src/LSRB_Algorithm_Robot.ino`

4. Install required libraries (if any)

5. Upload the code to your Arduino Uno

## 🎮 Usage

### Autonomous Mode
1. Power on the robot
2. Place it at the start of the maze
3. The robot will automatically:
   - Map the maze during first run
   - Calculate the shortest path
   - Execute the solution

### Manual Control Mode
1. Connect to the robot via Bluetooth
2. Use the Bluetooth Serial Terminal App
3. Send commands to control the robot manually

## 📐 Circuit Diagram

The complete circuit diagram can be found in the `docs` folder.

## 🤖 How It Works

The robot uses the LSRB algorithm for navigation:

1. **Left**: Turn left if possible
2. **Straight**: If left is blocked, move straight
3. **Right**: If both left and straight are blocked, turn right
4. **Back**: If all paths are blocked, reverse (dead end)

The decision-making process is based on real-time sensor readings from three ultrasonic sensors (front, left, and right).

## 📝 Code Structure

- `src/LSRB_Algorithm_Robot.ino`: Main Arduino code
  - Sensor initialization and reading
  - Motor control functions
  - Decision-making logic
  - Bluetooth communication

## 🎯 Applications

- Search and Rescue Operations
- Industrial Automation
- Security and Defense
- Underground Exploration
- Educational Robotics

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👥 Authors

- Your Name - Initial work

## 🙏 Acknowledgments

- Thanks to the Arduino community
- Inspired by various maze-solving algorithms
- Built for educational and practical purposes 