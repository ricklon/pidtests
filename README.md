# PID Description and Testing
Step by step walkthrough of PID controls using a servo and potentiometer

# Why test how PID Controllers work?

I've been creating self-driving cars and most of the time instead of purchasing an expensive servo to steer with my team has building servos from scratch using window wiper motors or drill motors. I want to take a step back and look at the fundamentals of the problem. Then with a twist, try to get machine learning to do the same activity as the PID.

# So what is a PID Controller?
Wikipedia definition and tons of details: https://en.wikipedia.org/wiki/PID_controller

A PID is a Proportional-Integral-Derivative Controler. Turns out its a feedback loop that helps a system hold onto a value or position.

How about the math part:
* Proportional (P): If the system changes respond by change a similar amount. Big movements require similar large responses.
* Integral (I): I normally think of the integral as how much work or a measure of work that needs to be done. Change "work" to displacement or area, and you have a standard way of thinking about the Integral. 
* Derivative (D): Rate of change. Acceleration is an example of the rate of change.

So in terms of goals, we want a control loop that measures the distance or error between where we are now and where we want to be. That feedback is used to pick a proportional value in the case of small change is small, and a large change is large. Further, we want to know the trend over time how much work has been done. That would be our integral. The last in the sequence is what's the rate of change or work that's been done. All of this so we can pick a new value that gets the potentiometer to the goal value.


# What about the concept of error? What's the deal?

# Test by having an Arduino control a servo and have it turn and keep a potentiometer at a specific value.

The reason for this test is that it doesn't use any custom parts. These are off the shelf parts you can get from almost any Arduino kit.

# Parts
 1. Arduino
 2. Servo
 3. Potentiometer
 4. Heatshrink
 5. (Something to hold the servo and potentiometer)
 
 #Tests
 
# Case: Servo control move potentionmeter
 ## Issue: there maybe no noise.
## 1. Just move to the goal

## 2. Move to the goal proportionally

## 3. Move to the goal proporitionally and derivatively

## 4. move to the goal full PID

## 5. Tune the values
 
# Case: Machine Learn a PID
# Case: Machine Learn the Tuning of a PID

# Case: new problme via Open AI GYm
The OpenAI Gym has a pole balancing problem. This a classic control system. Thet nicely have them problem outlined. https://gym.openai.com/docs/#environments


## 1. Apply a PID

## 2. Apply machine learning


## 3. Compare results
