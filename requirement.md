Private Network
Create Account
Create simple smart contract
Deploy smart contract
Build UI for Dapp

==== Pratices 
Ganache
====

layout
Description business, workflow, introduction
	+ Userstory
		Requirement
		Acceptance test
		include hint
	
	

History Patient 
	- Create account(Hospital), account(person)
	- Create patient(Contract) {person info, history treatment[]}
	- Transfer money to patient Contract
		- Only create treat if it has money
		- Create treatment(History of patient) Contract  + Create history + transfer money to hospital
	- View Patient info and history (notify)
Crowd fund
	- Create accounts(can be founder || can be sponsor)
	- Create project(Smart contract) => defined founder
	- Sponsor can sponse for project(transfer money to project)
	- Create request for project(Spend money to someone to do something)
	- Sponsor must approve before transfering money
	- View project info include balance, 
	
Insurance
Descripton:
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
	
	- EOA: patient, insurer owner, hospital owner
	
	- Create hospital, insurer(contract)
	- Deposit money to insurer;
	- Additional steps(put money to insurer)
	- Hospital create receipt(Type struct in hospital smart contract)
	{
		idReceipt
		patient_address
		money
		treatment
		hospital_Address
	}
	- Patient call claim(idReceipt, hospital_address, msg.sender) in insurer contract
	- Owner of insurer call approve after that money will be sent to patient
	- Mark receipt is paid
	- Otherwise mark reject;
	
Supply chain
	- EOA : producer owner, vender owner 
	- Create producer(contract) buyProduct(transfer money, addr_prod) -> update new owner product
	- Create distribution vendor(Smart contract)] buyProduct(transfer money, addr_prod) -> update new owner product
	- Producer create product(Smart contract){price, include history};
	- Producer sellto distribution vendor => update history of product and owner
	- Distribution vender sell to another distribution vendor => add history and update owner of product
	==
	View history of product
	-- Withdraw money from contract owner product
	
	
	
	
