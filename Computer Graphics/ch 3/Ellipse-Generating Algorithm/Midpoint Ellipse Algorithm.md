سأعيد كتابة الشرح مع إضافة الترجمة العربية بعد كل جزء، متبوعة بالزتونة (الخلاصة).

---

### **Understanding the Midpoint Ellipse Algorithm**

### **(فهم خوارزمية النقطة الوسطى لرسم القطع الناقص - الإهليلج)**

#### **1. Basic Concept of Drawing an Ellipse**

- An **ellipse** is like a stretched or squished circle.
    
- It is defined by **two radii (rx, ry)** and a **center (Xc, Yc)**.
    
- To draw an ellipse, we calculate **points** that lie on its boundary.
    
- The ellipse can be shifted and rotated to fit different positions.
    

#### **(1. المفهوم الأساسي لرسم القطع الناقص)**

- القطع الناقص (الإهليلج) هو شكل يشبه الدائرة لكنه ممدود أو مضغوط.
    
- يتم تعريفه بواسطة **نصف القطر الأفقي rx ونصف القطر الرأسي ry** ومركزه عند **(Xc, Yc)**.
    
- لرسمه، نحسب **النقاط** التي تقع على حدوده.
    
- يمكننا أيضًا **تحريكه أو تدويره** ليناسب أي موضع على الشاشة.
    

🟢 **الزتونة:**  
نحدد مركز القطع الناقص ونصف القطرين، ثم نحسب النقاط التي تشكل حدوده.

---

#### **2. How the Midpoint Algorithm Works**

- The method **divides the first quadrant** of the ellipse into two regions based on slope:
    
    - **Region 1:** Slope < 1 → Move step by step in the **x-direction**.
        
    - **Region 2:** Slope > 1 → Move step by step in the **y-direction**.
        

#### **(2. كيف تعمل خوارزمية النقطة الوسطى؟)**

- تقسم هذه الطريقة **الربع الأول** من القطع الناقص إلى منطقتين حسب الميل:
    
    - **المنطقة الأولى:** الميل أقل من 1 → نتحرك تدريجيًا في **الاتجاه الأفقي (x)**.
        
    - **المنطقة الثانية:** الميل أكبر من 1 → نتحرك تدريجيًا في **الاتجاه الرأسي (y)**.
        

🟢 **الزتونة:**  
نبدأ بالرسم في الربع الأول، ونقسمه إلى جزئين، جزء نتحرك فيه أفقيًا، والآخر رأسيًا.

---

#### **3. Choosing the Starting Point**

- We start at **(0, ry)**, which is the **topmost** point of the ellipse.
    
- Alternatively, we could start at **(rx, 0)** (rightmost point) and process counterclockwise.
    

#### **(3. اختيار نقطة البداية)**

- نبدأ عند **(0, ry)**، وهي **أعلى نقطة في القطع الناقص**.
    
- أو يمكننا البدء عند **(rx, 0)** (أقصى نقطة على اليمين) ونتحرك عكس اتجاه عقارب الساعة.
    

🟢 **الزتونة:**  
يمكننا البدء من الأعلى أو اليمين والتحرك حول الشكل.

---

#### **4. Decision Parameters for Region 1**

- A **decision parameter (P1)** helps decide whether to move **right** (increase x) or **diagonally down** (increase x, decrease y).
    
- The formula for **P1** is:
    
    P1=ry2−rx2ry+14rx2P1 = r_y^2 - r_x^2 r_y + \frac{1}{4} r_x^2
- If **P1 < 0**, move **horizontally** (increase x).
    
- Otherwise, move **diagonally** (increase x, decrease y).
    

#### **(4. معاملات اتخاذ القرار في المنطقة 1)**

- يتم استخدام **معامل اتخاذ القرار (P1)** لتحديد ما إذا كنا سنتحرك **يمينًا (زيادة x)** أو **قطريًا لأسفل (زيادة x وتقليل y)**.
    
- المعادلة لحساب **P1** هي:
    
    P1=ry2−rx2ry+14rx2P1 = r_y^2 - r_x^2 r_y + \frac{1}{4} r_x^2
- إذا كان **P1 < 0**، نتحرك أفقيًا (نزيد x فقط).
    
- خلاف ذلك، نتحرك **قطريًا لأسفل** (نزيد x ونقلل y).
    

🟢 **الزتونة:**  
نستخدم معادلة P1 لتحديد ما إذا كنا سنتحرك أفقيًا أو قطريًا أثناء الرسم.

---

#### **5. Transition to Region 2**

- When the slope reaches -1, we switch to **Region 2**.
    
- A new **decision parameter (P2)** helps decide whether to move **down** (decrease y) or **diagonally down** (increase x, decrease y).
    

#### **(5. الانتقال إلى المنطقة 2)**

- عندما يصبح الميل -1، ننتقل إلى **المنطقة 2**.
    
- يتم استخدام **معامل اتخاذ قرار جديد (P2)** لتحديد ما إذا كنا سنتحرك **لأسفل (نقلل y فقط)** أو **قطريًا لأسفل (نزيد x ونقلل y)**.
    

🟢 **الزتونة:**  
بعد الوصول إلى المنطقة 2، نستخدم معامل P2 لاتخاذ القرار بين التحرك عموديًا أو قطريًا.

---

### **Final Summary (الزتونة النهائية)**

✅ **الخطوة 1:** نبدأ من النقطة العلوية للقطع الناقص **(0, ry)**.  
✅ **الخطوة 2:** نستخدم **P1** لتحديد إذا كنا سنتحرك **يمينًا** أو **قطريًا** في **المنطقة 1**.  
✅ **الخطوة 3:** عندما يصبح الميل -1، ننتقل إلى **المنطقة 2**.  
✅ **الخطوة 4:** نستخدم **P2** لتحديد إذا كنا سنتحرك **لأسفل** أو **قطريًا لأسفل**.  
✅ **الخطوة 5:** نكرر العملية مع عكس النقاط لإنهاء رسم القطع الناقص بالكامل.

🟢 **الخلاصة النهائية:**  
هذه الطريقة تحسب النقاط بكفاءة عالية لرسم القطع الناقص **دون الحاجة إلى حسابات معقدة عند كل خطوة!** 🚀

---
# اختبر حفظك :[[(Q)Midpoint Ellipse Algorithm]]