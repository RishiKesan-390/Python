import matplotlib.pyplot as plt
import numpy as np

# Actual human distance data (in cm)
actual_distance = np.array([20, 40, 60, 80, 100, 120, 140, 160, 180, 200])

# Measured ultrasonic sensor distance data (in cm)
measured_distance = np.array([22, 39, 63, 78, 105, 118, 142, 158, 185, 198])

# Create the plot
plt.figure()

# Ideal line (Actual vs Actual)
plt.plot(actual_distance, actual_distance, marker='o', label="Actual Distance")

# Sensor measured line
plt.plot(actual_distance, measured_distance, marker='s', label="Measured Distance")

# Labels and title
plt.xlabel("Actual Human Distance (cm)")
plt.ylabel("Distance (cm)")
plt.title("Ultrasonic Sensor Measured Distance vs Actual Human Distance")

# Grid and legend
plt.grid(True)
plt.legend()

# Show plot
plt.show() 
