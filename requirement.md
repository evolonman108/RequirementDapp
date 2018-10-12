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
	
	
	
	
