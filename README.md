# Compilation

## CRITERIA
## MEETS SPECIFICATIONS
* Code compiles without errors with cmake and make

# Implementation

## CRITERIA
## MEETS SPECIFICATIONS
* I used what I learned in the lessons to build a PID loop and optimized hyperparameters to it. 
# Reflection

## CRITERIA
## MEETS SPECIFICATIONS
* Describe the effect each of the P, I, D components had in your implementation.

* The porportional part of the controller steers to car to the center of the road. It does this by steering against the CTE. When using only the porportional part of the controller the car tends to overshoot the center of the road, causing it to crash.
* The Differential part of the controller takes into account any bias in the steering. If there is no bias (In this simulation this is minimal) it won't have any effect. If there is a bias you can correct it by implementing a differential.

* The Integral part of the controller helps smoothen the approach to the center by taking into acount the sum of the CTEs. It will cause the car to gradually change the angle porportional to the distance it is to the center. 

* I used a manual version of Twiddle, adding 1.0 until the parameter had a negative effect of the car. I would then decrease the value by .5 and see if it had a positive or negative effect on the car. I repeated these steps until I fine tuned the parameters. 


# Simulation

## CRITERIA
## MEETS SPECIFICATIONS
* The vehicle successfully drives a lap around the track without leaving the track.
