### 2. Packet Switching

#### - **What’s happening?**:
- This is how the internet sends stuff—like breaking a big letter into tiny notes and mailing them separately.
#### - **How does it work?**:
 - Imagine you’re sending a huge story to your friend. Instead of mailing one big book, you rip it into little pages (called **packets**).
    - Each packet has an address on it, saying where it’s going (like “To: Friend’s House”).    - These packets travel through the internet, hopping from one **router** to another. A router is like a mailman who looks at the address and picks the next stop.
     - **==Routing==**: The mailman figures out the best path (“Go left, then right”).
     - **==Forwarding==**: The mailman hands the packet to the next mailman on that path.
   - Each router waits until the whole packet arrives before sending it to the next one. This is called ==**store-and-forward**==. It’s like waiting for all the words on a page before passing it along.
   - Example: If a packet is 7.5 million bits (a big page) and the mail truck moves at 1.5 million bits per second (pretty slow), it takes 5 seconds to send it one hop (7.5 ÷ 1.5 = 5).
#### - **What can go wrong?**:
  - If too ==many packets== show up at once, they line up (**==queueing==**). It’s like a bunch of letters piling up at the post office.
- If the line gets too long and there’s no more room (==the mailbox is full==), some packets get thrown away ==(**lost**)==. You might lose part of your story!
#### - **Why it’s cool**:
- Packets can take different paths, so if one road is blocked, they find another way.

## **الشرح بالعربي**:

### - **إيه اللي بيحصل؟**:
- دي الطريقة اللي الإنترنت بيبعت بيها الحاجات—زي ما تكون بتكسر جواب كبير لوريقات صغيرة وتبعتهم لوحدهم.
### - **بيشتغل إزاي؟**:
- تخيل إنك بتبعت قصة كبيرة لصاحبك. بدل ما تبعت كتاب كبير، بتقطعها لوريقات صغيرة (اسمها **باكيتس**).
- كل ورقة عليها عنوان، بيقول رايحة فين (زي “لـ: بيت صاحبي”).
- الوريقات دي بتسافر في الإنترنت، بتقفز من **راوتر** لراوتر. الراوتر زي ساعي البريد اللي بيبص على العنوان ويقرر المحطة الجاية.
    - **الروتينج**: الساعي بيحسب أحسن طريق (“روح شمال، بعدين يمين”).
    - **الفورواردينج**: الساعي بيدي الورقة للساعي اللي بعده في الطريق.
- كل راوتر بيستنى لحد ما الورقة توصل كلها قبل ما يبعتها للي بعده. دي اسمها **ستور أند فوروارد**. زي ما تكون بتستنى كل الكلام في الورقة قبل ما تمررها.
- مثال: لو الورقة 7.5 مليون بت (ورقة كبيرة) وعربية البريد بتمشي 1.5 مليون بت في الثانية (بطيئة شوية)، هتاخد 5 ثواني عشان تبعتها محطة واحدة (7.5 ÷ 1.5 = 5).
- **إيه ممكن يحصل غلط؟**:
    - لو ورق كتير وصل مرة واحدة، بيصفوا في طابور (**كيوينج**). زي ما يكون جوابات كتير متكدسة في البريد.
    - لو الطابور زاد جدًا وما فيش مكان (الصندوق اتملى)، الورق بيتحدف (**ضايع**). ممكن جزء من قصتك يضيع!
### - **ليه حلو؟**:
-الورق ممكن ياخد طرق مختلفة، فلو طريق اتسد، بيلاقي غيره.

## **الزتونة**: 
الإنترنت بيقطع الحاجات لوريقات صغيرة بتسافر لوحدها، ممكن تتأخر أو تضيع لو الزحمة كتير.