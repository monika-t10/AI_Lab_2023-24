# Ex.No: 8  Logic Programming –  Medical Diagnosis Expert System
### DATE:   20.09.25                                                                         
### REGISTER NUMBER : 212223060170
### AIM: 
Write a Prolog program to build a medical Diagnosis Expert System.
###  Algorithm:
1. Start the program.
2. Write the rules for each diseases.
3. If patient have mumps then symptoms are fever and swollen glands.
4. If patient have cough, sneeze and running nose then disease is measles.
5. if patient have symptoms headache ,sneezing ,sore_throat, runny_nose and  chills then disease is common cold.
6. Define rules for all disease.
7. Call the predicates and Collect the symptoms of Patient and give the hypothesis of disease.
        

### Program:
```
hypothesis(Patient,german_measles) :-
symptom(Patient,fever),
symptom(Patient,headache),
symptom(Patient,runny_nose),
symptom(Patient,rash).
hypothesis(Patient,flu) :-
symptom(Patient,fever),
symptom(Patient,headache),
symptom(Patient,body_ache),
symptom(Patient,conjunctivitis),
symptom(Patient,chills),
symptom(Patient,sore_throat),
symptom(Patient,runny_nose),
symptom(Patient,cough).
hypothesis(Patient,common_cold) :-
symptom(Patient,headache),
symptom(Patient,sneezing),
symptom(Patient,sore_throat).
hypothesis(Patient,chicken_pox) :-
symptom(Patient,fever),
symptom(Patient,chills),
symptom(Patient,body_ache),
symptom(Patient,rash).
hypothesis(Patient,measles) :-
symptom(Patient,cough),
symptom(Patient,sneezing),
symptom(Patient,runny_nose).
symptom(raju,headache).
symptom(raju,sneezing).
symptom(raju,sore_throat).
```
### Output:
<img width="949" height="359" alt="image" src="https://github.com/user-attachments/assets/91b80fe4-9b95-42f8-9ab3-f49db3131c6c" />
<img width="955" height="358" alt="image" src="https://github.com/user-attachments/assets/508aae2b-f783-4549-a1d1-a3fd04be7eef" />
<img width="953" height="331" alt="image" src="https://github.com/user-attachments/assets/be45cc3d-5433-4912-80dc-3b45f3491068" />

### Result:
Thus the simple medical diagnosis system was built sucessfully.
