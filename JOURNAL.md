May 18th: Planning and Basic Design
I started my project by choosing constraints and the optimal materials / gear ratios for my project.

I decided on utilizing 67102RS, MF126ZZ, and MF128ZZ bearings, and the use of DIN 965 and DIN 9647 (Hex socker countersink/button head) M3 and M4 screws, as all these parts are cheap and can be obtained off of Amazon and AliExpress.

I then needed to decide what electronics to use, and went with the FIRST Tech Challenge (FTC) architecture as I have experience with these parts and already own some of the electronics needed. Using [goBILDA YellowJacket motors](https://www.gobilda.com/modern-robotics-12vdc-motor/) along with [DSSSERVO brushless servos](https://tinyurl.com/abacadabaDSSERVO) in conjunction with [mt6701 encoders i got from Melonbotics](https://www.melonbotics.com/products/barecoder-micro) made sure I keep my project affordable while having the same power as other swerve drives, such as FTC teams 16917 and 22105.

After knowing what main parts were necessary, I simulated the optimal gear ratio using a modifed FRC drivetrain calculator to determine that a 9:1 gear ratio on a 64mm wheel has the perfect balance between speed, acceleration, and traction on the FTC field.
![image](https://github.com/user-attachments/assets/fef51ce7-05be-407b-9c91-cc009dd0da71)

However, I could not find good traction wheels online that matched the size I wanted (64mm), and decided to mold my own tread out of [VytaFlex 60](https://www.smooth-on.com/products/vytaflex-60/), a 60a durometer urethane. I've molded wheels in the past out of 30a silicone, but had little success since the tread easily peeled off of the wheel.
![IMG_1714](https://github.com/user-attachments/assets/3f99dbbb-0c45-48a0-9b2d-6a07b2cb0b24)

I now had to choose where to obtain the pulleys and gears to reduce the motor from 6000 to 666, and used AliExpress for the first stage (pulleys), Custom Fabworks gears for the 2nd (spur gears), and [Axon Robotics bevel gears](https://axon-robotics.com/products/bevels) for the final stage (bevel gears). For the azimuthal (wheel swivel), I decided to use HTD-3M 1:1 to ensure proper accuracy and load-handling.

Now I moved on to CAD, where I used Onshape to make a master-sketch, a full construction diagram of the swerve pod so I can easily change one dimension that affects all the others quickly using variables and relations.
![image](https://github.com/user-attachments/assets/9dff0b21-d7e2-4af9-a94f-c2ddb10212c8)
![image](https://github.com/user-attachments/assets/0556fab5-e69b-4893-9509-846fcb65aa8c)
![image](https://github.com/user-attachments/assets/92ce9aae-08d4-4492-9612-48c15bddb90b)


