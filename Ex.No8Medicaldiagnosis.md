# Ex.No: 8  Logic Programming –  Medical Diagnosis Expert System
### DATE:  26/03/2024                                                                         
### REGISTER NUMBER : 212221040089
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

![image](https://github.com/Lingasri/AI_Lab_2023-24/assets/143391929/78a40476-5b27-4269-9f45-7eea35dd9c5c)
![image](https://github.com/Lingasri/AI_Lab_2023-24/assets/143391929/7ce5c4bf-51b2-4999-ba1a-521e93aa5603)
![image](https://github.com/Lingasri/AI_Lab_2023-24/assets/143391929/75884f12-6bfa-4039-b041-519c495e8715)
![image](https://github.com/Lingasri/AI_Lab_2023-24/assets/143391929/c1fb7768-96ec-4353-baae-22b993d1139d)




### Result:
Thus the simple medical diagnosis system was built sucessfully.
