# alpha
Crowd Funding Farmers practising Natural Farming methods

## Objective
* Crowd fund farmers to save them from huge debts.
* Create platform for consumers to fund/buy products grown without pesticides and other chemical

## Design
### UI Pages

	1) Welcome page ( stat, about the project)
	2) User Login
	3) User dashboard
	4) Project list
	5) Project page
  6) Payment page
  
### DB Design
	1) User details
		a. Name, mail id, phone , password, uid
	2) Former details
		a. Name, phone , mail id , pan card , aadhard , address , experience, land , uid
	3) Project
		a. Farmer_uid, type, crop , uid, start mon, end mon, current stage, target fund, price, units, quantity , geo location, blog and gallery , comments.
	4)  fund
		a. Project_uid, user_uid, prices, units , status
			i. Shipping related details
	5) Journal
		a. Date, p_uid , u_uid , price, payment id , payment type, credit
			i. Payment type
				1) Paytm
				2) Goods
			ii. Credit
				1) Yes ( from former)
				2) No ( from user)

### API
	1) POST /login 
		a. userid : Phoneno or email id
		b. Pass : Password
		c. Return :
			i. Cookie(optional)
			ii. Status
			iii. Username
			iv. userid
	2) GET /logout
	3) GET /projects
		a. Crop
		b. Period
		c. Current state
		d. Target
		e. Price, unit, quantity,
		f. Geo location,
		g. Current accumulation
		
		
	4) GET /project/id
		a. Farmer Details
		b. Blog , gallery
		c. Project details
		
		
	5) GET /journal/user
	6) GET /journal/user/project_id
	7) GET /journal/project_id
	
### Stack
Backend:
	1) Nodejs - Expressjs
	2) Database - MySQL

FrontEnd:
	1) JS, Bootstarp
	
	
Interface:
	1) REST API

