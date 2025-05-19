May 18th: Planning and Basic Design
I started my project by choosing constraints and the optimal materials / gear ratios for my project.

I decided on utilizing 67102RS, MF126ZZ, and MF128ZZ bearings, and the use of DIN 965 and DIN 9647 (Hex socker countersink/button head) M3 and M4 screws, as all these parts are cheap and can be obtained off of Amazon and AliExpress.

I then needed to decide what electronics to use, and went with the FIRST Tech Challenge (FTC) architecture as I have experience with these parts and already own some of the electronics needed. Using [goBILDA YellowJacket motors](https://www.gobilda.com/modern-robotics-12vdc-motor/) along with [DSSERVO Coreless Servos](https://tinyurl.com/aliexpresdsservo) in conjunction with [mt6701 encoders](https://tinyurl.com/mt6701aliexpress) made sure I keep my project affordable while having the similar power as other swerve drives that use brushless servos.

After knowing what main parts were necessary, I simulated the optimal gear ratio using a modifed FRC drivetrain calculator to determine that a 9:1 gear ratio on a 64mm wheel has the perfect balance between speed, acceleration, and traction on the FTC field.
![image](https://github.com/user-attachments/assets/fef51ce7-05be-407b-9c91-cc009dd0da71)

However, I could not find good traction wheels online that matched the size I wanted (64mm), and decided to mold my own tread out of [VytaFlex 60](https://www.smooth-on.com/products/vytaflex-60/), a 60a durometer urethane. I've molded wheels in the past out of 30a silicone, but had little success since the tread easily peeled off of the wheel.
![IMG_1714](https://github.com/user-attachments/assets/3f99dbbb-0c45-48a0-9b2d-6a07b2cb0b24)

I now had to choose where to obtain the pulleys and gears to reduce the motor from 6000 to 666, and used AliExpress for the first stage (pulleys), both Aliexpress and Fabworks gears for the 2nd (spur gears), and [Axon Robotics bevel gears](https://axon-robotics.com/products/bevels) for the final stage (bevel gears). For the azimuthal (wheel swivel), I decided to use HTD-3M 1:1 to ensure proper accuracy and load-handling.

Now I moved on to CAD, where I used Onshape to make a master-sketch, a full construction diagram of the swerve pod so I can easily change one dimension that affects all the others quickly using variables and relations.
![image](https://github.com/user-attachments/assets/9dff0b21-d7e2-4af9-a94f-c2ddb10212c8)
![image](https://github.com/user-attachments/assets/0556fab5-e69b-4893-9509-846fcb65aa8c)
![image](https://github.com/user-attachments/assets/92ce9aae-08d4-4492-9612-48c15bddb90b)


**Time Spent this Session: 4 hours**
--------------------------------
May 19th: Continued Design and changes
I've finished most of the parts for the pod and will start prototyping the wheel soon!
I've decided to change some aspects, mainly the gear ratio and gears. Instead of 9:1, im using **8:1** as it allows the robot to drive faster and use only aliexpress and goBILDA instead of neededing custom gears, ensuring accuracy and saving money. Below are images of the new simulation and aliexpress + goBILDA gears (goBILDA gears will be cut down to fit)
![image](https://github.com/user-attachments/assets/fff9da39-adc7-45e3-be87-5349de8db86a)
![image](https://github.com/user-attachments/assets/ca195e9b-de7a-47ff-81e3-fa0fd8d2e0dd)
![image](https://github.com/user-attachments/assets/8c3e21ec-5579-4371-b5fd-404d97c9044d)

The pod consists of 2 major parts: The **Motor section** (Drive), and the **Servo section** (Azimuthal/Swivel)
The Motor section is the main view, consisting of the spur reduction, bevel reduction, and the "**Grease Trap**".
The spur and bevel reductions allows for the motor to drive the wheel no matter the swivel position because the driven gear will spin around the driving gear without adding in additional motion to the wheel itself.
![image](https://github.com/user-attachments/assets/45e13076-033a-428f-9599-7d5e5a4d1df8)
The Grease Trap is a simple cover for the spur reduction, allowing me to use grease to keep the motion smooth at a high rpm while keeping out dust, and mounts with the same screws the forks do to minimize complexity. The use of heat set inserts makes for a secure fit while keeping the pod sleek and low-profile.
![image](https://github.com/user-attachments/assets/f2c33ac0-868c-4c5d-8793-eb16b04d7c66)






