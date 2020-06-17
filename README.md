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

