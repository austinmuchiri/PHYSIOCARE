# PHYSIOCARE
 A Physical Therapy Exercise Monitor with Fall Detection and Visual Feedback.

Concept:

PhysioCare empowers individuals undergoing physical therapy to perform exercises effectively and safely at home. It tracks movements using the MPU6050 sensor (gyroscope and accelerometer), monitors for falls, and provides real-time feedback through a TFT screen and LEDs.

Components:

STM32 Nucleo F746ZG Board: The development platform for processing sensor data and controlling functionalities.
GY-521 Module (MPU6050 Sensor): Tracks 3D acceleration and orientation for exercise recognition.
Touch Sensor: Serves as a start/stop button for exercise routines and fall detection acknowledgment.
Real-Time Clock (RTC) Module: Keeps track of time for exercise duration monitoring.
TFT Display (Choose a suitable size and resolution): Provides visual feedback on exercise routines, data, and timer information.
Multiple LEDs (Optional): Offer visual cues for exercise guidance and fall alerts.

Additional Considerations (Optional):
Buzzer for audible fall alerts.
Bluetooth Low Energy (BLE) for smartphone app integration (data logging, exercise history, fall notifications).
Pulse oximeter sensor for heart rate monitoring (more comprehensive health data).
Project Functionality:

Exercise Routines:
Pre-programmed exercise routines targeting specific muscle groups are stored in the STM32F746ZG's memory.
Users initiate routines with the touch sensor.
Real-Time Feedback:
The TFT screen displays clear instructions and animated visuals for each exercise.
Live data from the MPU6050 sensor (movement angles, range of motion) is visualized on the TFT screen.
Color-coded feedback or progress bars guide the user's exercise form and performance.
Fall Detection:
Accelerometer data is continuously monitored to detect sudden falls.
Upon fall detection, LEDs flash rapidly (and a buzzer sounds, if included), and a clear message appears on the TFT screen, potentially prompting user action or alerting caregivers.
The RTC module timestamps the fall event for later reference.
Timer Visualization:
The remaining exercise duration or rest periods are prominently displayed on the TFT screen.

BENEFITS:
Independent Exercise Monitoring: Patients can perform physical therapy routines at home while receiving feedback on form and progress.
Enhanced Safety: Fall detection provides an extra layer of security, potentially alerting caregivers or prompting user action.
Visual Guidance: Clear instructions, animated visuals, and real-time data visualization on the TFT screen promote user understanding and adherence.
