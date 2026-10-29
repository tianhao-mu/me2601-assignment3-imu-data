# ME2601 Assignment 3: Raw IMU Data

Raw smartphone sensor data for the IMU logging and dead-reckoning experiment.

## Recording

- Application: phyphox 1.2.1.
- Requested sampling rate: 100 Hz.
- Observed sampling rate: approximately 100.1427 Hz.
- Accelerometer record duration: 36.2283 seconds between first and last samples.
- Primary movement direction: the phone's longitudinal Y axis.

## Original CSV files

- [Accelerometer.csv](Accelerometer.csv): 3,629 samples, with time in seconds and X/Y/Z specific-force readings in m/s². These readings include gravity.
- [Gyroscope.csv](Gyroscope.csv): 3,628 samples, with time in seconds and X/Y/Z angular rates in rad/s.

The CSV files are unchanged copies of the original export. Each file retains its own timestamps; the two sensor streams are not resampled or merged.

The recording includes stationary intervals at its beginning and end. Velocity estimation requires gravity handling and sensor-offset treatment before integrating acceleration.
