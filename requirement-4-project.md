# requirement more detail
## History Patient [need reason for transfer money]
#### Descrition [rewrite description follow business]
Introduce: 
The treatment history of the patient is very important. But it is mainly write and read from the book. The doctor hard to review the treatment history of the patient so that he can provide the best and suitable treatment. Although from hospital to hospital, the patient have to do the medical examintaion again and and again for the same sickness because the hospials don't trust each other.
Apply blockchain to transperant the patient's treatment history to solve the problem.

Business desciption
1. When a peron goes to hospital for checking his heath or sickness, the hospital create a patient contract for him, or lookup the patient contract of him in blockchain system if there is existing one.
2. The hospital has to retrieve the treatment history of this patient in order to have an overview.
3. The hospital provide the medical examination request. The patient has to pay money for that before getting the result.
4. When the examination result is returned, the system send the notification to the patient.
5. The hospital provides the treatment only if there is a examination result.

data structure for examination request:
        - patient_id
        - hospital_address
        - examination_name
        - examination_result
        - money
data structure for patient:
        - patient_id
        - person_address
        - hospital_address
        - doctor_name
        - sickness_diagnose
        - examination_address
        - treatment

#### Requirement: Build an application has GUI and use blockchain to do the following task
1. The hospital create heath records for patient include information such as(name, age, gender)
2. The patient must be transfer money to electronic heath records
3. Then the hospital write treatment and sickness into the electronic heath record. 
4. The electronic heath record with update history of hospital and patient will approve heath record and then transfer money to hospital
5. Notify patient and hospital if there are some changes in there account balance in that transaction.



## Crowd fund
#### Descrition:
Nowsaday, a crowd fund project is a secret for every people, even for the sponsors. Because one sponsor just know how much he contributes and does not know the others. Also all the sponsors does not know what the project owner does with their fund.
Apply blockchain to transparent the income and outcome money. Also grant the right to the sponsors so that they know their money is using for what, and can stop it if they want.

### Business description
1. A person create his own the crowd fund project.
2. everyone can fund for this project to become a sponsor
3. The project owner use the money for some reason, such as buy the materials, hiring the labour ... That means he transfer the money to someone else. Let say he creates a request to transfer the money to another account
4. The sponsors can approve or reject the request. If the request has enough approvement, the money will be transfer
5. Every sponsor is nofified that the request is executed or canceled

data structure for project contract...
data structure for request contract...


1. Prevent founder of project create request transfer money to someone without confirmation sponsor of the project.
#### Requirement: Build an application has GUI and use blockchain to do the following task
1. A founder create project
2. Project must be funded by sponsor(at least 1eth) before can create request transfer money to someone
3. After create request, sponsor must approve that request
4. If the number of sponsor approved greater than 50% of total number sponsor. Then system will transfer money to someone that already setup before.
5. After trasfer money create notifycation to inform account balance of sender and reciever

## Insurrance:
#### Descrition:
- In order to reduce the time the claim process. With the normal process the insured persons have to wait days or weeks or even months to get back the money. 
- In order to reduce effort for the insurer companies to verify the claim.
- Preventing chect from their customers.
- Make process more safety
#### Requirement: Build an application has GUI and use blockchain to do the following task
1. the hospital has the responsibility to do the medical examination and treatment, and store them to blockchain so that the insurer can access these information to verify later. Let say 'receipt'.
2. the patient (insured person) claim the money by giving the receipt id.
based on the receipt id, the insurer verifies it, and then approve or reject.
3. If receipt is rejected then inform the reason to the patient.
4. if approve then transfer the money to the patient and inform approve. 
5. the patient receives claim result automatically(e.g. a popup message, give hint).
  
## Supply chain: need transfer money
#### Descrition:
- In order to provide customers have more information about product history, such as:
    - when is it created?
    - who created it?
    - who are distributions?
    - Distribution vendor can resell fake products which come from unknown sources.
#### Requirement: Build an application has GUI and use blockchain to do the following task 
1. The producer can make new products and put them into blockchain.
2. The distribution vendor can buy products from producer or other vendor. The changing owner information will be update into blockchain as well.
3. Customers can view history of their products based on product identifiers.
4. Changing owner event will be raised to other related persons.
