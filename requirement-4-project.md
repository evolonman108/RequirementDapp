## History Patient 
#### Descrition
1. A patient go to hospital for checking his/her heath
2. The hospital will lookup his information in electronic heath record and see all history information of patient about
    - Where did he/she check before?
    - What kind of sickness?
    - What was the treatment?
#### Requirement: Build an application has GUI and use blockchain to do the following task
1. The hospital create electronic heath records for patient include information such as(name, age, gender)
2. The patient must be transfer money to electronic heath records
3. Then the hospital write treatment and sickness into the electronic heath record. 
4. The electronic heath record with update history of hospital and transfer money to hospital
5. Notify patient and hospital if there are some changes in there account balance in that transaction.

## Crowd fund
#### Descrition:
1. Prevent founder of project create request transfer money to someone without confirmation sponsor of the project.
#### Requirement
1. A founder create project
2. Project must be sponed by sponsor before can create request transfer money to someone
3. After create request, sponsor must approve that request
4. If the number of sponsor approved greater than 50% of total number sponsor
5. Then system will transfer money to someone that already setup before.
6. After trasfer money create notifycation to inform account balance of sender and reciever

## Insurrance:
#### Problem:
- the claim process takes time. The insured persons have to wait days or weeks or even months to get back the money. 
- the insurer companies have to spend a lot of effort and time to verify the claim.
- but they cannot avoid the cheat from their customers.
#### Idea: apply blockchian to:
- verify the claim form easier and faster.
- transfer money faster.
- prevent the cheat.
#### Requirement:
1. the hospital has the responsibility to do the medical examination and treatment, and store them to blockchain so that the insurer can access these information to verify later. Let say 'receipt'.
2. the patient (insured person) claim the money by giving the receipt id.
3. based on the receipt id, the insurer verifies it, and then approve or reject.
4. if approve then transfer the money to the patient and inform approve.
5. if reject, inform the reason to the patient.
6. the patient recieves claim result automatically.
  
## Supply chain:
#### Problem: 
- Customers have less information about product history, such as:
    - when is it created?
    - who created it?
    - who are distributions?
    - Distribution vendor can resell fake products which come from unknown sources.
- Idea: apply blockchain to
	- Identify issues faster.
	- Increase consumer and partner trust in good transparency.
#### Requirement:
1. The producer can make new products and put them into blockchain.
2. The distribution vendor can buy products from producer or other vendor. The changing owner information will be update into blockchain as well.
3. Customers can view history of their products based on product identifiers.
4. Changing owner event will be raised to other related persons.
