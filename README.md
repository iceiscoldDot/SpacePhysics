# **Dimentii Algorithm**

I am Khalish, a 14-year-old student from Malaysia. I created this algorithm for fun to explore pattern recognition and numerical "healing." Dimentii unzips a number sequence and finds its hidden root frequency.

---

## **A to Z Calculation Example (Input: 2312)**

### **A. Recursive Extraction (γ')**
*Unzip the original number by adding its digits in sequences.*
*   γ'₁ = 2 + 3 + 1 + 2 = **8**
*   γ'₂ = 3 + 1 + 2 = **6**
*   γ'₃ = 1 + 2 = **3**
*   γ'₄ = 1 + 3 + 2 = **6**
*   γ'₅ = 1 + 3 = **4**

### **B. Index Collision**
*If two answers are exactly the same, fuse them by adding their index numbers.*
*   **Match:** γ'₂ = 6 and γ'₄ = 6
*   **Fuse Index:** 2 + 4 = 6
*   **Result:** The new coordinate is **6_γ'₆**

### **C. Ordered Mapping (ℕγ')**
*Sort the unique values and their specific indices from smallest to largest.*
*   **Array:** [ **3_γ'₃**, **4_γ'₅**, **6_γ'₆**, **8_γ'₁** ]

### **D. The Fusion Calculation (Index + Number)**
*Add each base number to its index to reveal where the patterns cross.*
*   3 + 3 = **6**
*   4 + 5 = **9** *(Collision)*
*   6 + 6 = **12**
*   8 + 1 = **9** *(Collision)*

### **E. State Grouping**
*Separate the numbers based on whether they are stable or tangled in a collision.*
*   **Lining (γ°): [3, 6]** — *Stable. They have a clean mathematical link (3 x 2 = 6).*
*   **Not Lining (ℕi): [4, 6, 8]** — *Tangled. 4 and 8 both crashed into the number 9 during Fusion.*

### **F. Root Stabilization**
*Find the Greatest Common Factor (GCF) of the tangled numbers to heal them and find the hidden frequency.*
*   GCF of 4, 6, 8 = **2**

---

## **Final Diagnostic Answer: 2312**
*   **Lining (γ°):** [3, 6]
*   **Not Lining (ℕi):** [4, 6, 8]
*   **Root Frequency (GCF):** **2**
