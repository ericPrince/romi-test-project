# Romi Test Project 2023

Project created from the `RomiReference` example project [as outlined in WPILib's docs](https://docs.wpilib.org/en/stable/docs/romi-robot/programming-romi.html#creating-a-new-wpilib-romi-project).

## To Use This Project

- Install WPILib, clone this repo, and open it in WPILib's installed VSCode
- Make sure the right team number is set in `.wpilib/wpilib_preferences.json`
- Make sure `wpi.sim.envVar` is set correctly in `build.gradle` (only matters if you changed the Romi's network settings - [see here](https://docs.wpilib.org/en/stable/docs/romi-robot/programming-romi.html#running-a-romi-program))
- Install the Spotless Gradle plugin for VSCode (should be recommended for install when you open this project)

## Differences from RomiReference Example

The following changes were made to the example project:

- Added a CI pipeline that runs for pull requests to the `main` branch
- Added Spotless for code style checking and apply-on-save [as outlined in WPILib's  docs](https://docs.wpilib.org/en/stable/docs/software/advanced-gradlerio/code-formatting.html)

## Useful Resources

- [WPILib documentation for Romi](https://docs.wpilib.org/en/stable/docs/romi-robot/index.html)
- [WPILib installation guide](https://docs.wpilib.org/en/stable/docs/zero-to-robot/step-2/wpilib-setup.html)
- [Romi product page on Pololu](https://www.pololu.com/product/4022)
