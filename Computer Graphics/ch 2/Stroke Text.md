
## **1. Stroke Text (Vector Text)**

### **What is Stroke Text?**

- **Stroke text** is a type of text where each letter is made up of **lines and curves**, just like drawing with a pen.
- It is **not stored as pixels**, but rather as **geometrical instructions** for drawing the shape of each character.
- Think of it like writing letters using a **connect-the-dots method**, where each letter is formed by a set of points connected by lines or curves.
- This means that stroke text **can be scaled (zoomed in or out) without losing quality**, making it perfect for applications where text needs to be resized.

### **How is Stroke Text Constructed?**

- Each letter is drawn using **vertices (points)**, and these points are connected by:
    - **Straight lines** (for letters like "L" or "T")
    - **Curved lines** (for letters like "S" or "O")
- If a character is **fully enclosed**, we can **fill it with color** to make it solid.

---

### **شرح Stroke Text بالعربي**

- النص المتجهي هو نوع من النصوص يتم **رسمه باستخدام خطوط ومنحنيات** بدلاً من أن يكون مجرد مجموعة من النقاط (Pixels).
- يتم تمثيل كل حرف على شكل **مجموعة من النقاط المتصلة بخطوط أو منحنيات**.
- هذا يجعله **قابلًا للتكبير والتصغير بدون فقدان الجودة**، على عكس النص النقطي (Raster Text).

#### **الزتونة:**

النص المتجهي هو نص يتم رسمه بخطوط ومنحنيات بدلاً من البكسلات، مما يجعله قابلًا للتكبير بدون تشويش.

---
# اختبر حفظك :[[(Q)Stroke Text]]