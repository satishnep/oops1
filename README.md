
class Account:
    def __init__(self,bal, acc):
        self.balance = bal
        self.account = acc


    def debit(self,amount):
        self.balance -= amount
        print("RS.", amount)
        print("total balance", self.get_balance())

    def credit(self,amount):
        self.balance += amount
        print("RS.", amount)
        print("total balance", self.get_balance())


    def get_balance(self):
        return self.balance

acc1 = Account(10000, 1234)

acc1.debit(1000)
acc1.credit(500)

acc1.credit(40000)
