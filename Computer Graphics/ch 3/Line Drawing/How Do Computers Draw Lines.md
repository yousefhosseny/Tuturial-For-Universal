## 1. How Do Computers Draw Lines?

A **line** is just a series of points placed close together. But computers do not see smooth lines like humans do. They see a set of **pixels** arranged in a stepwise manner.

### **How does a computer decide where to place points for a line?**

- The computer calculates **all the positions** between two endpoints, (X₁, Y₁) and (X₂, Y₂).
    
- It **fills in** those positions to make it look like a continuous line.
    

### **How does an analog (vector) system draw lines?**

- In older devices (like **vector pen plotters**), a pen smoothly moves from the start to the end of the line.
    
- The computer generates signals that smoothly vary in both **X** and **Y directions**, ensuring the line looks perfect.
    

### **How does a raster system draw lines?**

- Unlike smooth movement, **a raster system must choose exact pixels** to represent the line.
    
- The computer calculates the positions using the **line equation**:
    
    y=m⋅x+by = m \cdot x + b
    
    where:
    
    - **m** = slope (how steep the line is)
        
    - **b** = y-intercept (where it crosses the y-axis)
        

### **📌 الشرح بالعربي:**

الخط في الكمبيوتر هو مجرد مجموعة نقاط قريبة من بعضها، لكن الكمبيوتر مش بيشوف الخط زي ما الإنسان بيشوفه، لأنه بيتمثل عنده كسلسلة من البكسلات.

#### **إزاي الكمبيوتر بيحدد أماكن النقاط؟**

- الكمبيوتر بيحسب كل الإحداثيات بين النقطتين (X₁, Y₁) و(X₂, Y₂).
    
- بعد كده بيحط نقاط في الأماكن دي علشان الخط يظهر متصل.
    

#### **إزاي الأنظمة القديمة بترسم الخطوط؟**

- في الأجهزة القديمة زي **أجهزة الرسم بالقلم (Vector Plotters)**، القلم بيتحرك بسلاسة بين النقطتين.
    
- الكمبيوتر بيولد إشارات تحكم تتحكم في حركة القلم في الاتجاهين X و Y.
    

#### **إزاي نظام الراستر بيرسم الخطوط؟**

- الكمبيوتر ما يقدرش يرسم خط ناعم، فلازم **يحدد البكسلات اللي تمثل الخط**.
    
- بيستخدم معادلة الخط المستقيم:
    
    y=m⋅x+by = m \cdot x + b
    
    حيث:
    
    - **m** = الميل (انحدار الخط)
        
    - **b** = التقاطع مع المحور y.
        

### **📝 الزتونة:**

الكمبيوتر بيرسم الخطوط عن طريق حساب كل النقاط بين نقطتين، لكن في **أنظمة المتجهات** بيتحرك القلم بسلاسة، أما في **أنظمة الراستر** الكمبيوتر لازم يحدد بكسلات معينة لتمثيل الخط.

---

# [[How Do Computers Draw Lines (Q)]] : اختبر حفظك