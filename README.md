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
