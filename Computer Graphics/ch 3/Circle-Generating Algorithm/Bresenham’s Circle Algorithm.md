حاضر، هشرح كل جزء بالإنجليزي وبعده العربي، وفي النهاية هحط **الزتونة** بتاعته.

---

## **Bresenham’s Circle Algorithm - A Simple & Deep Explanation**

### **Why Do We Need This Algorithm?**

We want to draw a circle on a screen made up of pixels (raster display). The problem is:

1. **Basic circle equation** (x−xc)2+(y−yc)2=r2(x - xc)^2 + (y - yc)^2 = r^2 needs square roots, which are slow.
    
2. **Using trigonometry (cos, sin)** is also slow.
    
3. We need **efficient calculations** to determine which pixel is closest to the actual circle path.
    

So, Bresenham’s algorithm **avoids complex math** and uses simple addition and subtraction to decide the best pixel to plot.

### **ليه بنحتاج الخوارزمية دي؟**

إحنا عاوزين نرسم **دائرة على شاشة بيكسلز (Raster Display)**، لكن عندنا مشاكل:

1. المعادلة الأصلية للدائرة (x−xc)2+(y−yc)2=r2(x - xc)^2 + (y - yc)^2 = r^2 فيها **جذور تربيعية** ودي بطيئة جدًا في الحساب.
    
2. **استخدام حساب المثلثات (Sin و Cos)** برضه بطيء ومكلف.
    
3. محتاجين **طريقة أسرع** تحدد أي بيكسل هو الأقرب للمسار الحقيقي للدائرة.
    

علشان كده **خوارزمية بريزنهام** بتجنبنا كل الحسابات المعقدة وبتستخدم **الجمع والطرح فقط** لاختيار البيكسل الصحيح.

### **🟢 الزتونة:**

- المعادلة الأصلية للدائرة بطيئة لأنها فيها جذور تربيعية.
    
- حساب المثلثات (Sin و Cos) مش عملي.
    
- خوارزمية Bresenham بتوفر طريقة أسرع باستخدام **الجمع والطرح بس**.
    

---

## **Core Idea of Bresenham’s Algorithm**

Instead of using the complex circle equation, we:  
✅ Start from the **top (0, r)** and move towards the right.  
✅ Decide the **next pixel** using a simple decision formula.  
✅ Use **symmetry** to generate the full circle with minimal calculations.

### **الفكرة الأساسية لخوارزمية Bresenham**

بدل ما نستخدم المعادلة الأصلية المعقدة، بنعمل التالي:  
✅ نبدأ من **أعلى نقطة في الدائرة (0, r)** ونتحرك ناحية اليمين.  
✅ نختار **البيكسل التالي** بناءً على **معادلة بسيطة** تقرر أي نقطة أقرب لمسار الدائرة.  
✅ نستخدم **التناظر (symmetry)** علشان نحسب ربع الدائرة بس، وننسخ الباقي تلقائيًا.

### **🟢 الزتونة:**

- بنبدأ من فوق الدائرة عند النقطة (0,r)(0, r).
    
- بنختار البيكسل الجديد باستخدام **معادلة سهلة وسريعة**.
    
- بنستخدم **التناظر** علشان نحسب جزء صغير من الدائرة ونكرر الباقي.
    

---

## **How It Works (Step-by-Step)**

1. **Start with the first point:** (0,r)(0, r) because a circle at the origin is symmetric.
    
2. **Use a decision parameter PkP_k** to choose between two possible pixels:
    
    - The one **directly right (x + 1, y)**
        
    - The one **diagonally down-right (x + 1, y - 1)**
        
3. **Update PkP_k based on which pixel is closer to the circle.**
    

### **إزاي بتشتغل خطوة بخطوة؟**

1. **بنبدأ من النقطة الأولى:** (0,r)(0, r) لأن الدائرة **متناظرة حول المركز**.
    
2. **بنستخدم متغير قرار PkP_k** علشان نختار بين **بيكسلين محتملين**:
    
    - البيكسل **اللي على اليمين (x + 1, y)**
        
    - البيكسل **اللي تحت بزاوية (x + 1, y - 1)**
        
3. **بنحدث قيمة PkP_k** بحيث نختار البيكسل الأقرب لمسار الدائرة.
    

### **🟢 الزتونة:**

- عند كل خطوة، عندنا اختيار بين نقطتين.
    
- نختار النقطة الأقرب بناءً على قيمة **PkP_k**.
    
- الحسابات بتتم بدون جذور أو ضرب، مجرد **جمع وطرح**.
    

---

## **Decision Parameter Calculation**

We define a **decision variable** PkP_k to decide which pixel to choose:

- **Initial decision parameter:**
    
    P0=1−rP_0 = 1 - r
- **If Pk<0P_k < 0:** Choose the **right pixel (x+1, y)** and update PkP_k as:
    
    Pk+1=Pk+2xk+3P_{k+1} = P_k + 2x_k + 3
- **If Pk≥0P_k \geq 0:** Choose the **diagonal pixel (x+1, y-1)** and update PkP_k as:
    
    Pk+1=Pk+2xk−2yk+5P_{k+1} = P_k + 2x_k - 2y_k + 5

### **حساب متغير القرار PkP_k**

بنعرف متغير القرار PkP_k علشان يحدد أي بيكسل نختار:

- **القيمة الأولية لمتغير القرار:**
    
    P0=1−rP_0 = 1 - r
- **لو Pk<0P_k < 0:** بنختار البيكسل اللي **على اليمين (x+1, y)** ونحدث PkP_k كالتالي:
    
    Pk+1=Pk+2xk+3P_{k+1} = P_k + 2x_k + 3
- **لو Pk≥0P_k \geq 0:** بنختار البيكسل **المائل (x+1, y-1)** ونحدث PkP_k كالتالي:
    
    Pk+1=Pk+2xk−2yk+5P_{k+1} = P_k + 2x_k - 2y_k + 5

### **🟢 الزتونة:**

- بنبدأ بـ P0=1−rP_0 = 1 - r.
    
- لو PkP_k صغير، نتحرك **يمين**.
    
- لو PkP_k كبير، نتحرك **يمين وتحت** معًا.
    
- الحسابات كلها **سريعة جدًا** لأنها مجرد **جمع وطرح**.
    

---

## **Using Symmetry for Faster Calculation**

- A circle is **the same in all directions**, so we only calculate **one part** and then reflect the values.
    
- If we calculate pixels for **one-eighth (45° section)**, we can mirror them to fill the whole circle.
    

### **استخدام التناظر لحساب أسرع**

- الدائرة **متناظرة**، فبدل ما نحسب كل نقطة، نحسب **جزء صغير بس** وننسخه لباقي الدائرة.
    
- لو حسبنا البيكسلات لجزء **1/8 من الدائرة (من 0° لـ 45°)**، نقدر نستخدم التناظر ونرسم باقي الدائرة بسهولة.
    

### **🟢 الزتونة:**

- بنحسب **جزء صغير من الدائرة بس** علشان نوفر وقت.
    
- بنستخدم **التناظر** لرسم باقي الدائرة **أوتوماتيكيًا**.
    

---

## **Final Summary (الزتونة الكبيرة)**

✅ Bresenham’s Algorithm **سريعة جدًا** وبتستخدم **الجمع والطرح فقط**.  
✅ بتبدأ من **أعلى الدائرة** وبتختار البيكسل المناسب باستخدام **معادلة قرار بسيطة**.  
✅ بتستخدم **التناظر** لرسم الدائرة بالكامل بدون حسابات زيادة.

💡 **بمعنى تاني:** مش بنرسم كل البيكسلات، إحنا بس **بنحسب جزء صغير ونكرر الباقي بالتماثل**. 😊

---
# اختبر حفظك :[[(Q)Bresenham’s Circle Algorithm]]