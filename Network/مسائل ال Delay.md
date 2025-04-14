
# 1.  اولا تعديل الوحدات
#### لازم تكون المساله كلها بالوحدات دي :
![[Pasted image 20250409233637.png]]

##### يعني لو عندك ال Packet Size بال bytes

حولها لل bits عن طريق = $8 * Packet Size$


##### يعني لو عندك ال Transmission Rate بال Mbps

حولها لل bps عن طريق = $10⁶ * Transmission Rate$


##### يعني لو عندك ال Transmission Rate بال Gbps

حولها لل bps عن طريق = $10⁹ * Transmission Rate$


##### عموما ده جدول تحويلات قديم :
![[Pasted image 20250409235932.png]]


# ثانيا هو استخدام القوانين علشان اجيب المطلوب
#### قوانين  :

###### Propagation Delay: 
$$d(prop) = D/S= \frac {DistanceBetween Two Hosts (m)} { Propagation Speed (m/s)}$$

###### Transmission Time:
$$d(trans)=L/R = \frac {Packet Size In Bits} { Transmission Rate in Bps}$$

###### End-to-End Delay:

$$End-to-End Delay=d(Proc)+d(queue)+d(trans)+d(Prop)$$
## Note: 
==Nodal delay== = ==Total transmission delay== = ==End-to-End delay==


# 3. فيه تركات مختلفه
##### 1. ال ==Bandwidth== هو هو ال ==(R) Transmission Rate==
##### 2. لو ادالك ال  عدد الCircuits  في المساله 
ساعتها هتقدر تجيب ال Transmission Rate (R) =
$$Transmission Rate (R) = \frac{ Link Transmission Rate}{NumCircuits}$$

##### 3.  لو ادالك ال   ==Circuit Establishment Time==  في المساله ابقي زوده في الاخر مع ال ==Total time==

##### 4. لو قالك ان في سلكين في المساله واداك ال Packet Size بتاعت كل سلك واداك Transmission Rate (R)  واحد للسلكين اذا هتجيب ال
$$d(trans)= 2 * \frac {Packet Size In Bits} { Transmission Rate in Bps}$$
##### 5.  لو قالك ان في سلكين في المساله واداك الPacket Size بتاعت كل سلك واداك لكل سلك Transmission Rate (R) مختلف اذا هتعمل الاتي : 
![[Pasted image 20250410004734.png]]
