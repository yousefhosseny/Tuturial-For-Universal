
## **1. What is a Point in Computer Graphics?**

A **point** is the smallest unit in computer graphics. Think of it like a tiny dot on the screen.

### **How does a computer show a point?**

The computer does not "draw" like a human. Instead, it uses a **coordinate system** to decide where to place a point.

- A **coordinate** is just a pair of numbers like (X, Y) that tells us the location of the point on the screen.
    
- Example: If the screen is a grid, (5,10) means “move 5 steps right and 10 steps up” and place a dot there.
    

### **How does a screen display a point?**

- On an **old CRT monitor**, an **electron beam** moves to the correct position and lights up that tiny area.
    
- On a **modern raster display**, the screen has a **frame buffer** (a type of memory) where every pixel has a value:
    
    - **0 → Off (black, no light)**
        
    - **1 → On (white, full brightness)**
        
- If the computer marks a pixel as **1**, that spot on the screen lights up.
    

### **Vector vs Raster Systems**

- **Vector display**: The computer remembers instructions for each point and moves the electron beam exactly there.
    
- **Raster display**: The computer updates the **frame buffer**, and the screen follows those instructions to light up pixels.
    

### **📌 الشرح بالعربي:**

النقطة هي أصغر وحدة في الرسومات الحاسوبية. الكمبيوتر بيحدد أماكن النقاط باستخدام **نظام الإحداثيات** (X,Y)، وكل نقطة بتمثلها إحداثيين يحددوا موقعها على الشاشة.

#### **إزاي الشاشة بتعرض النقطة؟**

- في **الشاشات القديمة (CRT)**، الشعاع الإلكتروني بيتحرك للنقطة وبيشعل الفوسفور في المكان ده.
    
- في **الشاشات الحديثة (Raster Display)**، كل بكسل في الشاشة ليه قيمة في **ذاكرة الصورة (Frame Buffer)**:
    
    - **0 = مطفي (أسود)**
        
    - **1 = مضيء (أبيض)**
        
- لما الكمبيوتر يخلي قيمة البكسل "1"، النقطة بتنور على الشاشة.
    

#### **أنظمة رسم النقاط:**

- **نظام المتجهات (Vector Display)**: الكمبيوتر بيخزن الإحداثيات وبيتحكم مباشرة في الشعاع الإلكتروني لرسم النقطة.
    
- **نظام الراستر (Raster Display)**: الكمبيوتر بيحدد النقاط داخل ذاكرة الصورة، والشاشة بتعرضها بناءً على القيم المخزنة.
    

### **📝 الزتونة:**

النقطة هي أصغر جزء من الصورة، وتظهر على الشاشة بناءً على إحداثياتها. في الأنظمة القديمة (Vector)، الكمبيوتر بيتحكم مباشرة في الشعاع الإلكتروني. أما في الأنظمة الحديثة (Raster)، الكمبيوتر بيخزن النقاط في الذاكرة وبيتحكم في إضاءتها.


---
# اختبر حفظك :[[What is a Point in Computer Graphics (Q)]]