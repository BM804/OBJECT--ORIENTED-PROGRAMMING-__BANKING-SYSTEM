class bank:
    def __init__(self,amount,acc_no):
        print("Thank you for using our bank,")
        
        self.balance = amount
        self.acc_no = acc_no
        print(f"Your account number is {self.acc_no} and your Balance is {self.balance}")
        
    def credit(self,amount):
        self.balance += amount
        print(f"Your updated balancce is {self.balance}")
        
    def debit(self,amount):
        self.balance -= amount
        print(f"Your updated balancce is {self.balance}")
        

Customer = bank(
    int(input("Enter your First debosit Amount >>>>")),
    int(input("Enter your Existing account number .. >>>>"))
    
)
permisiion = input("e for exit or c for continue>>>")
if (permisiion == "e" or permisiion == "E"):
    print("Thank you for using our services ")
else:
     b = input("C for creadit and D FOR DEBIT")
     if(b == "c" or b== "C"):
         Customer.credit(int(input("Enter amount for credit")))
     else:
         Customer.debit(int(input("Enter amount for debit...")))
        
