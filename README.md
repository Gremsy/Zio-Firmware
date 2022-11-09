# Zio-Firmware
Gremsy Zio payload firmware

# What's new?

## Gimbal working mode
- Follow mode
- Lock mode
- Mapping mode

## Gimbal mounting position
- Normal: Gimbal works in Lock Mode/Follow Mode/Mapping Mode
- Inverted: Gimbal works in Lock Mode/Follow Mode
- Front: Gimbal works in Follow Mode

## Control gimbal with LightBridge 2 with DJI's Remote Control.
- In Single mode
  + C1 button switch mode (LOCK --> FOLLOW --> MAPPING)
  + C2 button switch control between TILT and PAN axis.
  + C2 button press hold > 2 seconds. Turn off Gimbal.
- In Dual Mode
  + C1 button switch mode (LOCK --> FOLLOW --> MAPPING)
  + C2 button press hold > 2 seconds. Turn off Gimbal.

## Control gimbal with Herelink with Pixhawk Flight Controller.
Use S.Bus signal output from the Herelink for simultaneous control of Autopilot, Gimbal and camera as well.
- In Single mode
  + Scroll wheel controls the TILT or PAN axis (Channel 10)
  + Top button (Right) controls the Gimbal mode including 3 states (Toggle PAN or TILT and Reset Position) (Channel 9)
  + C button controls zoom in for camera (Channel 14)
  + D button controls zoom out for camera (Channel 14)
  + Trigger Camera (Channel 7)

## Go to home position when switching the gimbal mode automatically.

## Control gimbal with gSDK.
- Gremsy SDK to meet the requirements of those building solutions for
various industrial applications.
- Adjust the speed, smooth and direction control of each axis. 
- Adjust Data Transmission Rates of each message.

## Detect errors when initialization.
- Gimbal will dectect automatically when initialization and pop-up error on the
new gTune with troubleshooting guide.

## Start-up at a random position.
