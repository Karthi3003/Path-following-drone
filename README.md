# Path-following-drone


### Project Title: **Path Following Drone Simulation Using CoppeliaSim**

**Duration**: [MAY 2023 - DEC 2023]  
**Tools & Technologies**: CoppeliaSim (V-REP), Python/Lua (for scripting), PID Controller, Quadrotor Model  
**Domain**: Robotics, Autonomous Systems, Simulation

#### Project Overview:
The goal of this project was to simulate an autonomous drone (quadrotor) capable of following a predefined path using the CoppeliaSim (formerly V-REP) robotics simulation software. The drone was programmed to autonomously navigate through waypoints while maintaining stability and accuracy using control algorithms such as PID (Proportional-Integral-Derivative). This simulation demonstrated the drone’s ability to perform complex navigation tasks, including dynamic obstacle avoidance and waypoint tracking.

#### Key Features:
1. **Quadrotor Model**:
   - Used the built-in quadrotor model in CoppeliaSim, which simulates the dynamics and control of a real drone.
   - The drone was equipped with four propellers that were modeled according to real-world aerodynamics and physics.

2. **Path Planning**:
   - A set of waypoints was defined as the drone’s flight path.
   - The drone followed a predefined path, where each waypoint represented a location in 3D space (X, Y, Z coordinates).
   
3. **PID Control System**:
   - A PID controller was implemented to manage the drone's orientation and speed, ensuring smooth and stable flight.
   - Tuned the PID parameters to minimize errors in altitude and lateral movements for accurate path tracking.

4. **Real-time Feedback Control**:
   - Used real-time feedback from the drone’s simulated sensors (e.g., position, orientation, velocity) to adjust its path and maintain stability.
   - Implemented correction algorithms that adjusted the drone’s velocity and orientation based on its deviation from the desired path.

5. **Obstacle Avoidance** (Optional Extension):
   - Dynamic obstacles were introduced into the simulation environment, and the drone was programmed to detect and avoid them.
   - Simple collision detection algorithms ensured that the drone adjusted its trajectory when encountering an obstacle.

6. **Simulation Environment**:
   - The simulation environment included 3D structures such as buildings and trees, mimicking real-world scenarios for testing drone behavior.
   - The terrain and wind effects were optionally simulated to test the drone’s ability to handle different environmental conditions.

#### Workflow:

1. **Defining the Path**:
   - A series of waypoints was defined in the simulation environment to represent the desired flight path.
   - The waypoints were programmed in a Lua or Python script, defining the 3D coordinates of each point the drone should reach.

2. **Drone Control Algorithm**:
   - The PID control algorithm was responsible for maintaining the drone’s altitude and direction.
   - Real-time sensor data was fed into the control system, which adjusted the drone's propeller speeds to maintain stability and accuracy.
   
3. **Simulation Execution**:
   - Once the simulation started, the drone autonomously navigated through the environment, adjusting its position and speed to follow the waypoints.
   - The drone’s behavior was visualized in real-time using CoppeliaSim’s 3D environment.

4. **Data Logging** (Optional):
   - Logged the position, orientation, and velocity of the drone during the simulation to evaluate its performance and efficiency in path following.
   - Analyzed the data to understand the effectiveness of the PID controller and make necessary adjustments.

#### Challenges and Solutions:
- **Challenge**: Tuning the PID controller for accurate and smooth flight control.
  - **Solution**: Experimented with various PID parameter values and used trial-and-error methods to achieve optimal stability and responsiveness.
  
- **Challenge**: Maintaining stable flight in the presence of obstacles and disturbances (e.g., wind).
  - **Solution**: Integrated obstacle detection and avoidance algorithms to handle dynamic changes in the environment.

#### Outcome:
- The drone successfully followed the predefined path with high accuracy and minimal deviation.
- The simulation demonstrated the drone's ability to autonomously navigate through waypoints, dynamically adjust its path in real-time, and avoid obstacles in a simulated 3D environment.
- This project served as a proof of concept for autonomous drone navigation and control, highlighting the effectiveness of PID controllers in aerial robotics.

#### Future Improvements:
- Implementing more advanced path-planning algorithms such as A* or RRT (Rapidly-exploring Random Tree) for real-time dynamic path adjustments.
- Introducing more realistic drone models with advanced sensors (e.g., LIDAR, GPS) to improve path planning and obstacle detection capabilities.
- Extending the simulation to include swarms of drones cooperating to complete complex tasks.

