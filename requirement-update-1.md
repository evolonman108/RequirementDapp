# requirement more detail
## History Patient
#### Descrition
To provide more history information of patient for hospital so that the hospital can check his/her heath better base on the information of patient like.
- Where did he/she check before?
- What kind of sickness?
- What was the treatment?
And also improve make the payment process of patient automaticly when hospital write treament history.

#### Requirement: Build an application has GUI and use blockchain to do the following task
The hospital and patient are EOA
1. The hospital create heath record contract for patient if not exist otherwise the hospital just input existing contract address of patient to see full information. The heath record contract has attribute such as (name, age, gender, patientAddress, historyInformation)
2. The patient must transfer money to his/her heath record contract. This transaction include some information such as hospital address, money (this money will be paid for hospital address later).
3. The hospital will write treatment and sickness into history of heath record of patient. The contract have to validate this hospital address is match with current hospital address in contract or not before writting down history and transfer money to hospital and update current hospital address in contract to empty.
4. Notify patient and hospital if there are some changes in there account balance in that transaction.

## Crowd fund
#### Descrition:

In order to track information of sponsor, founder of project and make the process transfer money to someone transparency among sponsors and founder.
#### Requirement: Build an application has GUI and use blockchain to do the following task
Founder and Sponsor are EOA
1. A founder create project has some informations such as name, founder address, list of sponsor, list of Request Address.
2. Project must be funded by sponsor(at least 1eth) if project reach 10eth(it can be a property of project or hardcode 10eth) so that project can create request transfer money to someone otherwise project can not create request.
- The request of project has some informations name, money, address of receiver, status, number of sponsor approved.
3. After create request, sponsor must approve that request before that request automatically transfer money to someone. If the number of sponsor approved greater than 50% of total number sponsor. Then system will transfer money to someone that already setup before.
4. After trasfer money create notifycation to inform account balance of sender and reciever

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
