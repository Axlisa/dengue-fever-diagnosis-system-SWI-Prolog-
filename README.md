### Dengue Fever Diagnosis System (SWI-Prolog)

#### **Overview**  
A simple Prolog program to diagnose dengue fever based on user-input symptoms.

---

#### **Code Structure**  

1. **Facts**:  
   - Defines symptoms and their corresponding queries.  
   ```prolog
   symptom(fever, 'Do you have fever? (yes/no)').
   symptom(headache, 'Do you have headache? (yes/no)').
   symptom(joint_pain, 'Do you have joint pain? (yes/no)').
   symptom(rash, 'Do you have rash? (yes/no)').
   ```

2. **Rules**:  
   - **`has_symptom/1`**: Checks if a symptom exists by prompting the user for input.  
   - **`has_dengue_fever/0`**: Verifies if all symptoms of dengue fever are present.  

3. **Diagnosis**:  
   - **`diagnose_disease/0`**:  
     - If all symptoms match, displays:  
       _"Based on the symptoms, you may have dengue fever."_  
     - Otherwise:  
       _"Based on the symptoms, it is unlikely that you have dengue fever."_  

---

#### **How to Run**  
1. Load the file in SWI-Prolog:  
   ```prolog
   ?- [filename].
   ```  
2. Start the diagnosis:  
   ```prolog
   ?- diagnose_disease.
   ```  
3. Answer the symptom prompts (`yes` or `no`) to get the result.  

---

#### **Key Features**  
- Interactive user input for symptom analysis.  
- Simple rule-based logic for disease diagnosis.  
- Demonstrates the use of facts, rules, and queries in Prolog.  

> **Note**: Replace `filename` with the actual file name containing the code.
