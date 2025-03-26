### **Bresenham’s Line Algorithm – Deep and Simple Explanation**

---

## **🔹 What is Bresenham’s Algorithm?**

Bresenham’s algorithm is a **fast and efficient way** to draw a straight line on a computer screen using **only integer calculations**. It is used in **raster graphics**, where everything is made of **pixels**. The goal is to determine **which pixels should be turned on** to make the line look as close to a straight line as possible.

### **📌 الشرح بالعربي**

خوارزمية **بريسنهام** هي طريقة سريعة وفعالة لرسم الخطوط في الكمبيوتر باستخدام **عمليات حسابية صحيحة فقط** (بدون أرقام عشرية). في أنظمة الجرافيكس اللي بتستخدم **البكسلات**، لازم نحدد أي **بكسلات يتم تشغيلها** علشان الخط يظهر مستقيم قدر الإمكان.

### **📝 الزتونة (الخلاصة)**

✅ بريسنهام طريقة ذكية لرسم الخطوط بسرعة ودقة بدون استخدام الأرقام العشرية.  
✅ بتحدد البكسلات المناسبة لتوصيل الخط بدون فراغات أو أخطاء.

---

## **🔹 Why is Bresenham’s Algorithm Important?**

Before Bresenham, line-drawing algorithms **used floating-point arithmetic**, which was slow and inefficient for computers. Bresenham’s approach solves this problem by:  
✅ **Using only integers** (no decimals, so calculations are faster).  
✅ **Making decisions at each step** to choose the best pixel.  
✅ **Keeping the line smooth** without gaps.

### **📌 الشرح بالعربي**

الطرق القديمة لرسم الخطوط كانت **بتستخدم أرقام عشرية**، وده كان بيخلي العمليات الحسابية بطيئة. خوارزمية بريسنهام حلت المشكلة عن طريق:  
✅ استخدام **أرقام صحيحة فقط**، وبالتالي أسرع في التنفيذ.  
✅ **اتخاذ قرارات عند كل خطوة** لتحديد البكسل الأفضل للرسم.  
✅ **الحفاظ على الخط متصل بدون فجوات**، علشان يكون شكله ناعم ودقيق.

### **📝 الزتونة (الخلاصة)**

✅ **بريسنهام أسرع وأدق من الطرق القديمة** لأنها بتستخدم أرقام صحيحة فقط.  
✅ **بتحسب أفضل بكسل كل خطوة علشان الخط يطلع ناعم ومتصل**.

---

## **🔹 How Does It Work?**

Let’s say we want to draw a line from **(x₁, y₁) to (x₂, y₂)**. The basic idea is:

1️⃣ **Start at the first point** (the leftmost pixel of the line).  
2️⃣ **Move pixel by pixel in the X-direction** (since x always increases).  
3️⃣ **At each step, decide which Y-pixel is closer to the actual line**:

- Either keep the same y.
    
- Or move one step up in y (y+1).  
    4️⃣ **Use a decision variable (p) to determine the best choice**:
    
- If **p is positive**, move **up** (increase y).
    
- If **p is negative or zero**, stay on the same y.  
    5️⃣ **Update p** and repeat until reaching the last point (x₂, y₂).
    

### **📌 الشرح بالعربي**

افترض إن عندنا خط عايزين نرسمه بين **(x₁, y₁) و (x₂, y₂)**، والفكرة الأساسية هي:

1️⃣ **نبدأ من أول نقطة** (أقصى يسار الخط).  
2️⃣ **نتحرك بكسل بكسل في اتجاه X**، لأن X بيزيد باستمرار.  
3️⃣ **كل خطوة لازم نحدد البكسل الأفضل في اتجاه Y**:

- إما **نفضل في نفس y**.
    
- أو **نزيد y بواحد** (لو الخط مايل لأعلى).  
    4️⃣ **نستخدم متغير القرار (p) علشان نعرف نختار إيه**:
    
- لو **p موجب** → نحرك y لأعلى.
    
- لو **p سلبي أو صفر** → نفضل في نفس y.  
    5️⃣ **نحدث قيمة p ونكرر العملية لحد ما نوصل لنقطة النهاية (x₂, y₂)**.
    

### **📝 الزتونة (الخلاصة)**

✅ **الخوارزمية بتختار البكسل الأفضل في كل خطوة، بين خيارين فقط**.  
✅ **بتستخدم متغير قرار p علشان تقرر إذا كان Y يزيد ولا يفضل ثابت**.

---

## **🔹 Understanding It Step by Step**

Let’s consider a simple case where the **line slope (m) is between 0 and 1** (meaning the line moves more in the x-direction than in the y-direction).

We define:  
📌 **m = Δy / Δx** (slope of the line).  
📌 **p = 2Δy - Δx** (decision variable).

**At each step:**

- If **p < 0**, plot the pixel **(x+1, y)** and update **p = p + 2Δy**.
    
- If **p ≥ 0**, plot the pixel **(x+1, y+1)** and update **p = p + 2Δy - 2Δx**.
    

### **📌 الشرح بالعربي**

لو كان ميل الخط (m) بين **0 و 1**، يعني بيتحرك أفقيًا أكتر من رأسي. بنحسب:  
📌 **m = Δy / Δx** → ده الميل.  
📌 **p = 2Δy - Δx** → متغير القرار اللي هيحدد كل خطوة.

**عند كل خطوة:**

- لو **p < 0** → نرسم البكسل في **(x+1, y)** و **نحدث p بإضافة 2Δy**.
    
- لو **p ≥ 0** → نرسم البكسل في **(x+1, y+1)** و **نحدث p بإضافة 2Δy - 2Δx**.
    

### **📝 الزتونة (الخلاصة)**

✅ **الخوارزمية بتقرر بين خيارين بناءً على قيمة p**.  
✅ **المعادلة بسيطة وسريعة وبتحدد أفضل بكسل في كل خطوة**.

---

## **🔹 Example: Drawing a Line from (20,10) to (30,18)**

Let’s go step by step:

|Step (k)|Decision (pₖ)|Next Pixel (x, y)|
|---|---|---|
|0|6|(21,11)|
|1|2|(22,12)|
|2|-2|(23,12)|
|3|14|(24,13)|
|4|10|(25,14)|
|5|6|(26,15)|
|6|2|(27,16)|
|7|-2|(28,16)|
|8|14|(29,17)|
|9|10|(30,18)|

### **📌 الشرح بالعربي**

نفترض إننا عايزين نرسم خط من النقطة **(20,10) إلى (30,18)**.

- كل خطوة، الخوارزمية بتقرر البكسل الأفضل بناءً على p.
    
- لو p موجب، بنزيد y، ولو سلبي أو صفر، y بيظل ثابت.
    

### **📝 الزتونة (الخلاصة)**

✅ **كل خطوة، الكمبيوتر بيقرر البكسل المناسب باستخدام حسابات بسيطة وسريعة**.  
✅ **في النهاية، الخط بيظهر ناعم ومتصل بدون أخطاء**.

---

# اختبر حفظك :[[Bresenham’s Line Algorithm (Q)]]
