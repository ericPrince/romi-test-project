# Romi Test Project 2023

Project created from the `RomiReference` example project [as outlined in WPILib's docs](https://docs.wpilib.org/en/stable/docs/romi-robot/programming-romi.html#creating-a-new-wpilib-romi-project).

## To Use This Project

### First Time Setup

- Install WPILib, clone this repo, and open it in WPILib's installed VSCode
- Make sure the right team number is set in `.wpilib/wpilib_preferences.json`
- Make sure `wpi.sim.envVar` is set correctly in `build.gradle` (only matters if you changed the Romi's network settings - [see here](https://docs.wpilib.org/en/stable/docs/romi-robot/programming-romi.html#running-a-romi-program))
- Install the Spotless Gradle plugin for VSCode (should be recommended for install when you open this project)

### Connecting to a Romi

To run this code base on a Romi, it will run in WPILib's simulation mode. For details on running a program, see the [WPILib docs](https://docs.wpilib.org/en/stable/docs/romi-robot/programming-romi.html#running-a-romi-program).

Running a Romi program will not use the FRC Driver Station, but you can connect it to a SmartDashboard or other dashboard instance.

1. Make sure the Romi is powered on and has already been configured (WPILib docs)
2. Connect to the Romi's wifi network (typically named `romi-5684-name`, ask for password)
3. Open the WPILib Command Palette (type `Ctrl+Shift+P`) and select “Simulate Robot Code”, or press `F5`

#### Connecting Joysticks

This program is made to run with an Xbox controller. If you connect a controller to your computer via USB, when you start the Romi program, the simulation GUI window will show up. You can drag the Joystick entry in the sim window to the joysticks area, and then the joystick will be used ([see this](https://docs.wpilib.org/en/stable/docs/software/wpilib-tools/robot-simulation/simulation-gui.html#adding-a-system-joystick-to-joysticks)).

Details on the simulation GUI and where to find joystick entries can be found [here](https://docs.wpilib.org/en/stable/docs/software/wpilib-tools/robot-simulation/simulation-gui.html).

#### Connecting the SmartDashboard

While the simulation window gives access to robot variables and NetworkTables, you can still connect a SmartDashboard instance to the running Romi program to be able to use the dashboard like you would in a real robot program. Do this by opening the SmartDashboard preferences (in the `File` menu) and setting the `Team Number` entry to `localhost`. See [this documentation](https://docs.wpilib.org/en/stable/docs/software/dashboards/smartdashboard/smartdashboard-intro.html#setting-a-custom-networktables-server-location) for details.

For more details on the simulation framework, and on connecting other dashboard types to the simulation, see [this documentation](https://docs.wpilib.org/en/stable/docs/software/wpilib-tools/robot-simulation/introduction.html#running-robot-dashboards).

## Differences from RomiReference Example

The following changes were made to the example project:

- Added a CI pipeline that runs for pull requests to the `main` branch
- Added Spotless for code style checking and apply-on-save [as outlined in WPILib's  docs](https://docs.wpilib.org/en/stable/docs/software/advanced-gradlerio/code-formatting.html)
- Changed the joystick axis numbers

## Useful Resources

- [WPILib documentation for Romi](https://docs.wpilib.org/en/stable/docs/romi-robot/index.html)
- [WPILib installation guide](https://docs.wpilib.org/en/stable/docs/zero-to-robot/step-2/wpilib-setup.html)
- [Romi product page on Pololu](https://www.pololu.com/product/4022)
- [WPILib simulation GUI overview](https://docs.wpilib.org/en/stable/docs/software/wpilib-tools/robot-simulation/simulation-gui.html)
