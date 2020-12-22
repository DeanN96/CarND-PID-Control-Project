## Describe the effect each of the P, I, D components had in your implementation.

The P component (proportional) is used to get a value that is proportional to the current error value. This helps modulate the speed. However, it can also cause oscillation. The I component (integral) is proportional to the magnitude of the error. It is also proportional to the magnitude of the duration of the error. This helps with bias error accumated over time. Since I did not have bias error accumate over time, I did use this component. The D component (derivitive) is proptional to the slope of the error over time. This component helped control the oscillation caused by the P component. 

## Describe how the final hyperparameters were chosen.

The values were found with trial and error. Starting at 0, I increased Kp until I had a problem with oscillation. Next I increased Kd until the oscillation was solved. 