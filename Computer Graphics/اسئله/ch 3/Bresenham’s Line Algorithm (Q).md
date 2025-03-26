Here’s a complete set of **exam-style study questions** based on **Bresenham’s Line Algorithm**, following your requested formats:

---

## **📌 Quick Recall Questions**

#### **1. What is Bresenham’s Line Algorithm used for?**

✅ **Answer:** It is used for drawing straight lines on raster displays using only integer calculations.

---

#### **2. Why is Bresenham’s Algorithm efficient?**

✅ **Answer:** Because it avoids floating-point calculations and uses only integer arithmetic.

---

#### **3. What is the main decision made at each step in Bresenham’s Algorithm?**

✅ **Answer:** Whether to move to the next pixel in the same row or move diagonally to the next row.

---

#### **4. What is the purpose of the decision variable (p) in Bresenham’s Algorithm?**

✅ **Answer:** It helps decide whether the next pixel should be on the same row or move up to the next row.

---

#### **5. How does Bresenham’s Algorithm keep a line smooth?**

✅ **Answer:** By selecting the closest pixel to the theoretical line at each step.

---

## **✅ True or False Questions**

#### **6. Bresenham’s Algorithm uses floating-point arithmetic for better accuracy.**

❌ **False** (It uses only integer calculations for efficiency.)

---

#### **7. The algorithm always moves in the X-direction at each step.**

✅ **True**

---

#### **8. The decision variable (p) is updated at each step based on its previous value.**

✅ **True**

---

#### **9. If p is negative, the algorithm moves the pixel diagonally (x+1, y+1).**

❌ **False** (If p is negative, y remains the same.)

---

#### **10. Bresenham’s Algorithm is only used for lines with a slope between 0 and 1.**

❌ **False** (It can be modified to work for any slope.)

---

## **🔄 Compare Questions**

#### **11. Compare Bresenham’s Algorithm with older floating-point-based line-drawing methods.**

✅ **Answer:**

- **Older Methods:** Use floating-point calculations, which are slow and complex.
    
- **Bresenham’s Algorithm:** Uses only integer arithmetic, making it faster and more efficient.
    

---

#### **12. Compare how the algorithm handles different values of the decision variable (p).**

✅ **Answer:**

- **If p < 0**, the next pixel is (x+1, y).
    
- **If p ≥ 0**, the next pixel is (x+1, y+1).
    

---

## **🛠️ Reason and Order Questions**

#### **13. Why does Bresenham’s Algorithm avoid floating-point operations?**

✅ **Answer:** Because floating-point calculations are slower and more complex for computers than integer operations.

---

#### **14. Arrange the following steps in order for how Bresenham’s Algorithm works:**

1. Start at the initial point.
    
2. Compute the initial decision variable.
    
3. At each step, determine the next pixel using p.
    
4. Update the decision variable.
    
5. Repeat until reaching the final point.
    

✅ **Answer:** 1 → 2 → 3 → 4 → 5

---

#### **15. Why does the algorithm always increase x at each step?**

✅ **Answer:** Because the line is assumed to be moving from left to right.

---

## **🎯 Multiple Choice Questions (MCQs)**

#### **16. What is the key advantage of Bresenham’s Algorithm?**

A) It uses floating-point arithmetic.  
B) It only works for vertical lines.  
C) It avoids gaps in the line.  
D) It requires large memory storage.

✅ **Answer:** C) It avoids gaps in the line.

---

#### **17. What does Bresenham’s Algorithm decide at each step?**

A) The best pixel to turn on  
B) The thickness of the line  
C) The color of the line  
D) The position of the last pixel

✅ **Answer:** A) The best pixel to turn on

---

#### **18. What happens if the decision variable (p) is negative?**

A) The next pixel is (x+1, y).  
B) The next pixel is (x, y+1).  
C) The next pixel is (x+1, y+1).  
D) The algorithm stops.

✅ **Answer:** A) The next pixel is (x+1, y).

---

#### **19. What is the formula for updating p when p < 0?**

A) p = p + 2Δy  
B) p = p + 2Δx  
C) p = p - 2Δy  
D) p = p - 2Δx

✅ **Answer:** A) p = p + 2Δy

---

## **💡 Concept Questions**

#### **20. What role does the slope (m) play in Bresenham’s Algorithm?**

✅ **Answer:** It determines how frequently the algorithm increases y along with x.

---

#### **21. How does the algorithm determine whether to move the pixel up or keep it at the same y level?**

✅ **Answer:** By checking the value of the decision variable (p).

---

#### **22. What does the decision variable p represent?**

✅ **Answer:** The difference between the actual line position and the closest pixel.

---

## **✏️ Complete the Sentence Questions**

#### **23. Bresenham’s Algorithm is designed for drawing __________.**

✅ **Answer:** straight lines using integer calculations.

---

#### **24. The decision variable p helps determine whether to __________.**

✅ **Answer:** stay on the same y or move up to y+1.

---

#### **25. If p is greater than or equal to zero, the next pixel is chosen at __________.**

✅ **Answer:** (x+1, y+1).

---

#### **26. Bresenham’s Algorithm is more efficient than older methods because it avoids __________.**

✅ **Answer:** floating-point calculations.

---

#### **27. The initial value of p is computed using the formula __________.**

✅ **Answer:** p = 2Δy - Δx.

---

This set of **27 questions** fully covers the text while matching your exam format! Let me know if you need any modifications or additional questions. 🚀