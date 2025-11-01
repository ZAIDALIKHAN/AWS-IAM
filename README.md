🧠 TL;DR — Mental Model

Role = Identity

Policy = Power

Instance Profile = Bridge between EC2 and IAM

Trust Policy = Door that allows EC2 to enter the role



-----------------------------------------------------------


⚙️ Putting It All Together
Component	Purpose	Without It
IAM Role	Defines who Terraform is (its identity)	Terraform has no permissions
IAM Policy	Defines what Terraform can do	Role has no power
Trust Policy	Defines who can use the role (EC2 in our case)	Role can’t be assumed
Instance Profile	Lets EC2 actually attach the role	EC2 can’t use the role
