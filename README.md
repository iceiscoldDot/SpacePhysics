# **Dimentii Algorithm**

I am Khalish, a 14-year-old student from Malaysia. I created this algorithm for fun to explore pattern recognition and numerical "healing." Dimentii unzips a number sequence and finds its hidden root frequency.

---

## **A to Z Calculation Example (Input: 2312)**

### **A. Recursive Extraction ($\gamma'$)**
*Unzip the original number by adding its digits in sequences.*
*   $\gamma'_{1} = 2 + 3 + 1 + 2 = \mathbf{8}$
*   $\gamma'_{2} = 3 + 1 + 2 = \mathbf{6}$
*   $\gamma'_{3} = 1 + 2 = \mathbf{3}$
*   $\gamma'_{4} = 1 + 3 + 2 = \mathbf{6}$
*   $\gamma'_{5} = 1 + 3 = \mathbf{4}$

### **B. Index Collision**
*If two answers are exactly the same, fuse them by adding their index numbers.*
*   **Match:** $\gamma'_{2} = 6$ and $\gamma'_{4} = 6$
*   **Fuse Index:** $2 + 4 = 6$
*   **Result:** The new coordinate is $\mathbf{6_{\gamma'_{6}}}$

### **C. Ordered Mapping ($\mathbb{N}\gamma'$)**
*Sort the unique values and their specific indices from smallest to largest.*
*   **Array:** [ $\mathbf{3_{\gamma'_{3}}}$, $\mathbf{4_{\gamma'_{5}}}$, $\mathbf{6_{\gamma'_{6}}}$, $\mathbf{8_{\gamma'_{1}}}$ ]

### **D. The Fusion Calculation (Index + Number)**
*Add each base number to its index to reveal where the patterns cross.*
*   $3 + 3 = \mathbf{6}$
*   $4 + 5 = \mathbf{9}$ *(Collision)*
*   $6 + 6 = \mathbf{12}$
*   $8 + 1 = \mathbf{9}$ *(Collision)*

### **E. State Grouping**
*Separate the numbers based on whether they are stable or tangled in a collision.*
*   **Lining ($\gamma^\circ$):** $[3, 6]$ — *Stable. They have a clean mathematical link ($3 \times 2 = 6$).*
*   **Not Lining ($\mathbb{N}i$):** $[4, 6, 8]$ — *Tangled. The numbers 4 and 8 both crashed into the number 9 during Fusion.*

### **F. Root Stabilization**
*Find the Greatest Common Factor (GCF) of the tangled numbers to heal them and find the hidden frequency.*
*   $GCF(4, 6, 8) = \mathbf{2}$

---

## **Final Diagnostic Answer: 2312**
*   **Lining ($\gamma^\circ$):** $[3, 6]$
*   **Not Lining ($\mathbb{N}i$):** $[4, 6, 8]$
*   **Root Frequency (GCF):** **2**

---

### **License**
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
