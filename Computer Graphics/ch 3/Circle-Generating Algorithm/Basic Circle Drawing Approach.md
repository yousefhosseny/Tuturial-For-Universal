
### **Basic Circle Drawing Approach**

- We can calculate points on the circle by stepping along the x-axis from $x_c - r$ to $x_c + r$ and calculating the corresponding y-values.
    
- The formula used:
    
$$
    y = y_c + \sqrt{r^2 - (x - x_c)^2}
$$
- **Problems with this approach:**
    
    - It requires a **lot of calculations** (square roots).
        
    - The pixels are **not evenly spaced**, which can make the circle look distorted.
        
    - Adjusting spacing increases complexity.
        

#### **شرح بالعربي**

- طريقة مباشرة لرسم الدائرة هي التحرك على محور **x** وحساب **y** من المعادلة.
    
- المشكلة في الطريقة دي إنها تحتاج عمليات **حسابية معقدة** (الجذر التربيعي) وبتؤدي لعدم **انتظام المسافات بين النقاط** المرسومة.
    

#### **الزتونة**

استخدام المعادلة العادية لرسم الدايرة مكلف حسابيًا ومش دقيق في توزيع النقاط.

---
# اختبر حفظك :[[(Q)Basic Circle Drawing Approach]]