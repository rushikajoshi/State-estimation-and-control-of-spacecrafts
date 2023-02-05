# Enhancing the performance of attitude control of spacecraft using state estimation
The specified problem is of practical consideration when real attitude and angular
velocity sensors are applied to the spacecraft attitude control system. The angular
velocity sensors (rate gyros) have unknown biases and very small measurement noises.
The attitude sensors (sun sensors, horizon sensors) are the type of sensors with
large measurement noise and are free of biases. These sensors are widely used in
spacecraft missions. Different types of sensor errors lead to attitude errors in the
controlled spacecraft when these sensors are directly applied to the attitude control
system without any treatments. In practical applications, a state estimator can be applied to estimate the unknown bias of the rate gyro and filter out the
measurement noise of the attitude sensor. The performance of the attitude controller is improved by applying the state estimator.

### Simulation
![GIF](https://user-images.githubusercontent.com/64770588/216806338-61281669-eb98-45e8-a3c4-0dc38dd1e8ab.gif)
### Results
As shown in the graph below, a noisy output is observed from the sensors
that result in inaccurate control. The spacecraft oscillates between the practically
undesirable values.

<img src="https://user-images.githubusercontent.com/64770588/216806599-29e8bfa2-6ade-4ea3-8401-e87c64274282.png" width=65% height=65%>

The graph below contains attitude values with noise and bias from the sensors vs. the
filtered values after using the Kalman Filter. Therefore, state estimation using a filter
removes the noise and bias and enhances the performance of the attitude controller.

<img src="https://user-images.githubusercontent.com/64770588/216806631-674de9d4-95ee-4d53-b59b-3fddca01a737.png" width=65% height=65%>
