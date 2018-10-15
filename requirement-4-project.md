History Patient 
	+ Descrition
		- A patient go to hospital for checking his/her heath
		- The hospital will lookup his information in electronic heath record and see all history information of patient about
			-- Where did he/she check before?
			-- What kind of sickness?
			-- What was the treatment?
	+ Requirement: Build an application has GUI and use blockchain to do the following task
		- The hospital create electronic heath records for patient include information such as(name, age, gender)
		- The patient must be transfer money to electronic heath records
		- Then the hospital write treatment and sickness into the electronic heath record. 
		- The electronic heath record with update history of hospital and transfer money to hospital
		- Notify patient and hospital if there are some changes in there account balance in that transaction.

Crowd fund
	+ Descrition:
		- Problem: A founder of project can perform some request transfer money to someone without inform sponsor of the project
		- Idea: Using blockchain. a founder of project must create request and must be approved by sponsor so that the request can transfer money to someone.
	+ Requirement
		- A founder create project
		- Project must be sponed by sponsor before can create request transfer money to someone
		- After create request, sponsor must approve that request
		- If the number of sponsor approved greater than 50% of total number sponsor
		- Then system will transfer money to someone that already setup before.
		- After trasfer money create notifycation to inform account balance of sender and reciever

Insurrance:
	- Problem:
		-- the claim process takes time. The insured persons have to wait days or weeks or even months to get back the money. 
		-- the insurer companies have to spend a lot of effort and time to verify the claim.
		-- but they cannot avoid the cheat from their customers.
	- Idea: apply blockchian to:
		-- verify the claim form easier and faster.
		-- transfer money faster.
		-- prevent the cheat.
Requirement:
	short description: 
		- the hospital has the responsibility to do the medical examination and treatment, and store them to blockchain so that 		the insurer can access these information to verify later. Let say 'receipt'.
		- the patient (insured person) claim the money by giving the receipt id.
		- based on the receipt id, the insurer verifies it, and then approve or reject.
		- if approve then transfer the money to the patient and inform approve.
		- if reject, inform the reason to the patient.
		- the patient recieves claim result automatically.
	action:
  
Supply chain:
	+ Description:
		- Problem: 
			-- Customers have less information about product history, such as: 
			---- when is it created?
			---- who created it?
			---- who are distributions?
			-- Distribution vendor can resell fake products which come from unknown sources.

		- Idea: apply blockchain to:
			-- Identify issues faster.
			-- Increase consumer and partner trust in good transparency.
	+ Requirement:
		- The producer can make new products and put them into blockchain.
		- The distribution vendor can buy products from producer or other vendor. The changing owner information will be update into blockchain as well.
		- Customers can view history of their products based on product identifiers.
		- Changing owner event will be raised to other related persons.
