In a sentence, explain the behavior you expected.
In a sentence, explain the observed behavior.
Formulate a hypothesis about what might be causing the mismatch: what part of your code or what part of your circuit is behaving in a way you don't expect?
Test your hypothesis: what action can you take you determine if your hypothesis is true?
What is the result of your test?
Repeat steps iii-v above until you resolve your "bug".

1
Expected the servo to move smoothly from current position to the position set by the light sensor. The servo is moving too fast, making the pannel shake a lot. The angle set by the light sensor changes too fast, making the servo move too fast. Create an intermediate value that acts as a target angle. 

2
Expected the servo to move by one degree at a time to the target angle. Servo is not moving. There might be a problem with the if function that sets the movement according to the difference of angle and targetAngle. Change the if statement to consider s1.read instead. It says 'Invalid use of member function'. That was because function s1.read was without ().

