### 4. Delays

### - **What’s happening?**:
- Delays are all the waiting that happens when your packets travel from you to your friend.
- **How does it work?**:
    - Picture a packet as a little car driving through the internet. It hits four kinds of stops:
        1. **Processing Delay**: The router (mailman) checks the car for problems (like “Is the address right?”). This is super quick, like a second or less.
        2. **Queuing Delay**: The car waits in line if other cars are ahead of it. If the internet’s busy, this can take longer—like waiting at a busy stoplight.
        3. **Transmission Delay**: The time it takes to push the car out of one router to the next. If the car is big (lots of bits) and the road is slow (low speed), it takes more time. Formula: Size ÷ Speed (L/R). Example: 7.5 million bits ÷ 1.5 million bits per second = 5 seconds.
        4. **Propagation Delay**: The time it takes the car to drive the actual distance. Depends on how far it is and how fast the signal moves (like light speed, super fast). Formula: Distance ÷ Speed (d/s). Usually tiny, like microseconds.
    #### - **Total Delay**:
    - Add all these waits together. If everything’s smooth, it’s fast. If there’s traffic, it slows down.
#### - **Loss**: 
- If too many cars show up and there’s no parking ==(router’s memory is full)==, some get kicked out. That’s packet ==loss==—part of your story doesn’t arrive.
#### - **Why it matters**: 
- Delays and loss explain why videos buffer or calls drop.

## **الشرح بالعربي**:

- **إيه اللي بيحصل؟**: التأخير هو كل الانتظار اللي بيحصل لما الباكيتس بتسافر منك لصاحبك.
- **بيشتغل إزاي؟**:
    - تخيل الباكيت زي عربية صغيرة بتمشي في الإنترنت. بتقف في أربع محطات:
        1. **تأخير المعالجة**: الراوتر (الساعي) بيفحص العربية لو فيها مشاكل (زي “العنوان صح؟”). ده سريع جدًا، زي ثانية أو أقل.
        2. **تأخير الطابور**: العربية بتستنى في الصف لو في عربيات قدامها. لو الإنترنت زحمة، بياخد وقت أكتر—زي ما تكون بتستنى عند إشارة زحمة.
        3. **تأخير الإرسال**: الوقت اللي بياخده عشان يدفع العربية من راوتر للي بعده. لو العربية كبيرة (بتات كتير) والطريق بطيء (سرعة قليلة)، بياخد وقت أكتر. المعادلة: الحجم ÷ السرعة (L/R). مثال: 7.5 مليون بت ÷ 1.5 مليون بت في الثانية = 5 ثواني.
        4. **تأخير الانتشار**: الوقت اللي العربية بتاخده عشان تمشي المسافة. بيعتمد على المسافة بعيدة قد إيه والإشارة بتمشي بسرعة قد إيه (زي سرعة الضوء، سريعة جدًا). المعادلة: المسافة ÷ السرعة (d/s). عادةً صغير جدًا، زي ميكروثانية.
    - **التأخير الكلي**: اجمع كل الانتظارات دي. لو كل حاجة تمام، بيبقى سريع. لو في زحمة، بيبطأ.
- **الضياع**: لو عربيات كتير وصلت وما فيش مكان للركن (ذاكرة الراوتر اتملت)، في عربيات بتترمي برا. ده اسمه ضياع الباكيت—جزء من قصتك ما بيوصلش.
- **ليه مهم؟**: التأخير والضياع بيفهموا ليه الفيديوهات بتقطع أو المكالمات بتقع.

## **الزتونة**: 
التأخير بيحصل من فحص وانتظار وإرسال ومسافة، والضياع لو الزحمة كتير.