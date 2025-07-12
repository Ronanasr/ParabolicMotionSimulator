# Projectile Motion Plotter

## Description
This Python script visualizes the trajectory of a projectile motion for a given initial velocity. It plots:
- The parabolic trajectory of the projectile at a fixed angle (45 degrees).
- The locus of the peak points of parabolas for varying launch angles, forming an ellipse.
- The peak point of the specific parabolic trajectory.

The script uses `numpy` for calculations and `matplotlib` (via `pylab`) for plotting.

## Features
- Calculates and plots the parabolic path of a projectile.
- Visualizes the envelope of maximum heights for different launch angles as an ellipse.
- Highlights the peak point of the projectile's trajectory.
- Uses a gravitational constant of 10 m/s² for simplicity.

## Requirements
- Python 3.x
- Required libraries:
  - `numpy`
  - `matplotlib`

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/your-repo-name.git
   ```
2. Navigate to the project directory:
   ```bash
   cd your-repo-name
   ```
3. Install the required libraries:
   ```bash
   pip install numpy matplotlib
   ```

## Usage
1. Save the script as `projectile.py`.
2. Run the script with a specified initial velocity (e.g., `v0 = 10`):
   ```bash
   python projectile.py
   ```
3. The script will generate a plot showing:
   - The projectile's parabolic trajectory (green line).
   - The envelope of peak points for varying angles (red line with dots).
   - The peak point of the specific trajectory (blue dot).

## Example Output
For an initial velocity `v0 = 10` m/s and a launch angle of 45 degrees, the script produces a plot like this:

![Example Plot](example_plot.png) *(Note: You can add a screenshot of the plot here by saving it and uploading it to the repository.)*

## Code Explanation
- **Function**: `projectile_cordinates(v0)`
  - Takes the initial velocity `v0` as input.
  - Computes the projectile's trajectory using kinematic equations.
  - Plots the parabolic path for a fixed angle (π/4 radians or 45 degrees).
  - Calculates and plots the locus of peak points (xm, ym) for angles from 0 to π radians.
  - Marks the peak of the specific trajectory.
- **Key Parameters**:
  - `g = 10`: Gravitational acceleration (m/s²).
  - `theta = pi/4`: Launch angle for the parabolic trajectory.
  - `t_total`: Total flight time, calculated as `2 * vy / g`.
  - `t`: Time array generated using `numpy.linspace` for smooth plotting.

## Contributing
Contributions are welcome! Please follow these steps:
1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Make your changes and commit (`git commit -m 'Add new feature'`).
4. Push to the branch (`git push origin feature-branch`).
5. Create a pull request.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contact
For questions or feedback, feel free to open an issue on GitHub or contact [your-email@example.com](mailto:your-email@example.com).