# PYTHON PRACTICE CODES

50. Functions Within functions:

def electricity_charges(previous_month_arrears):
    if previous_month_arrears>10000:
        return previous_month_arrears*3.5
    elif previous_month_arrears>7500:
        return previous_month_arrears*2.5
    elif previous_month_arrears>4500:
        return previous_month_arrears*1.75
    else:
        return 0
    
def KESC(current_bill, previous_month_arrears):
    overall = current_bill + electricity_charges(previous_month_arrears)
    print(f"Dear User Your Bill Is {overall}")
    
 51. While Loops:
 
 #1 
order = True
today_menu = []
while order:
    userinput= input("Kindly book your order")
    if userinput == "next":
        order = False
    else:
        today_menu.append(userinput)
today_menu

#2
flag = True
favdish= []
while flag:
    userinput = input("Enter Your Favourite Dish")
    if userinput =="stop":
        flag = False
    else:
        favdish.append(userinput)
favdish

52. Classes

class Car():
    # attributes >>>>>> are variables in programming
    #################################################
    def __init__(self, brand, engine_cc, year, transmission, color):
        self.brand = brand
        self.engine_cc = engine_cc 
        self.year = year
        self.transmission = transmission
        self.color = color
        self.battery = "400V" # Default Attributes
        
    # behaviour >>>>>>> are functions in programming
    ###############################################
    def car_details(self):
        print(f"Your car is {self.brand}")
        print(f"Your car Engine Power has {self.engine_cc}")
        print(f"Your car has been manufactured in {self.year}")
        print(f"Your car is {self.transmission}")
        print(f"Your car is {self.color}")
        
    def move(self):
        print(f"{self.brand} is moving with high speed")
    def applying_break(self):
        print(f"{self.brand} has applied break")
    def car_battery(self):
        print(f"Your car battery power is {self.battery}")
        
        # changing via Functions
        
    def setbatterysize(self, new_size):
        self.battery = new_size
    def getbatterysize(self):
        print(f"Your car battery size is {self.battery}")
        
    Changing an Attributes values
1) Direct hit the attributes
2) Via function (get set)
    

