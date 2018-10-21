# requirement more detail
## History Patient [need reason for transfer money]
#### Descrition [rewrite description follow business]
1. A patient go to hospital for checking his/her heath
2. The hospital will lookup his information in heath record and see all history information of patient about
    - Where did he/she check before?
    - What kind of sickness?
    - What was the treatment?

#### Requirement: Build an application has GUI and use blockchain to do the following task
1. The hospital create heath records for patient include information such as(name, age, gender)
2. The patient must be transfer money to electronic heath records
3. Then the hospital write treatment and sickness into the electronic heath record. 
4. The electronic heath record with update history of hospital and patient will approve heath record and then transfer money to hospital
5. Notify patient and hospital if there are some changes in there account balance in that transaction.

## Crowd fund
#### Descrition:

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
    the data structure:
        - reciept_id 
        - person address
        - hospital_address
        - treatment
        - money
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
