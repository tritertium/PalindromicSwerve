May 18th: Planning and Basic Design | **Time Spent this Session: 4 hours**

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


--------------------------------
May 19th: Continued Design and changes | **Time Spent this session: 2 hours**

I've finished most of the parts for the pod and will start prototyping the wheel soon! :)

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

--------------------------------------------------
May 24/25th: Finalized Plan | **Time Spent this session: 6 hours**
I've now finalized the geometry, using belts for the 2nd stage instead of gears to allow for an easy way to change gear ratio and to save costs. Addtionally, I can run a 25% thicker wheel, improving traction! (16mm vs 20mm)
I've also cut down costs by a good bit by using 3d printed gears (mod 1.5) instead of expensive aluminum ones.
![image](https://github.com/user-attachments/assets/f64d5e95-5569-4184-85aa-3ff498dcfed1)
![image](https://github.com/user-attachments/assets/6ad358b7-a117-4b23-8ad4-e7274b13df6b)
![image](https://github.com/user-attachments/assets/a050e4cb-f8a4-4dde-af1e-81c2c1276f4c)
After a good bit of research, I've found all the parts I'll need. I plan to use modified DS3225SG servos for the rotation as they have good torque and speed, and I tested the modification with a same brand servo a few days ago (Though the firmware makes it slow after around 2s, may need to workaround that somehow)
[Video](https://github.com/user-attachments/assets/cfb90ed9-acf9-4898-8cb2-bad8da67eb40)

----------------------------------------------------
May 25/26th: CAD of Pod and Wheel | **Time spent this session: 4 hours**
I finished the pod and wheel!
The pod is comrpised of many pulleys and 3d printed parts, along with the wheel.
![image](https://github.com/user-attachments/assets/15f35c81-26a6-4d60-84dd-92cfedf942a5)
![image](https://github.com/user-attachments/assets/e410fe10-0e0a-401c-a179-5ef4dc4d6ce3)

Having a mastersketch really helped here, since I just derived in the construction geoemtry and added what was needed. Most of the mounting uses m4 into a threaded shaft or M3 into ruthex inserts, making sure I keep the whole project robust while mainly being 3d printed.
![image](https://github.com/user-attachments/assets/71e3b4b4-121d-4368-a0a0-5bc7049c0cfd)

The wheel will be molded out of 60a polyurethane, this is my favorite part of making swerve as I can make a really grippy wheel with just a 2 part mix :).
![image](https://github.com/user-attachments/assets/ef01eb55-ebcf-4246-84f5-5d25c6e608dc)

That's all the cadding I did today, and I had to change alot of parts due to me messing up some dimensions, primarily the use of a 4mm shaft instead of 5mm, and the change of bearings from MF125ZZ to MF124ZZ.
After some rough math, the cost for a single pod is only around 10$ or so, which is much better than ~60$ for most other swerve drives in FTC due to using 30$ bearings and 25$ bevel gears. I'm not too sure how well the mod 1.5 3dp bevel gears will work in this case, but we'll have to see.




