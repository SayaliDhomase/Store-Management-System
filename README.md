## your code goes here ##
class Bikerental:
  stock=100
  def __init__(s):
    print("Welcome to rental bike shop")

  def displaystock(s):
    print("Total number of stock available",s.stock)


t=Bikerental()
t.displaystock()
## your code goes here ##
bike_shop=Bikerental()
bike_shop.displaystock()## your code goes here ##
bike_shop.displaystock()

bike_shop.stock
bike_shop.displaystock()

class Customer(Bikerental):
  bill=0
  def __init__(s,number_of_bikes,rentalBasis,number_of_days_or_weeks):
    # super().__init__(number_of_bikes,rentalBasis,number_of_days_or_weeks)
    s.number_of_bikes=number_of_bikes
    s.rentalBasis=rentalBasis
    s.number_of_days_or_weeks=number_of_days_or_weeks

def rentBike(s,number_of_bikes,rentalBasis,number_of_days_or_weeks):
  if s.number_of_bikes<=0:
    print("Number of bikes should be positive!")
  elif s.number_of_bikes>Bikerental.stock:
    print("number_of_bikes available to rent")
  else:
    updated_stock=Bikerental.stock-s.number_of_bikes
    print("Total number_of_bikes rented by the customer",updated_stock)

updated_stock=10
rentBike(5, updated_stock,6,10)
# m=Customer()
# m.rentBike(2,"daily",3)
def returnBike(s,):
  if s.rentalBasis=='daily':
    total_bill=100*s.number_of_bikes
  elif s.rentalBasis=='weekly':
    total_bill=500*s.number_of_bikes
  elif 3<=s.number_of_bikes<=5:
    discount=0.3*total_bill
    total_bill=total_bill-discount
    print("You are eligible for Family rental promotion of 30% discount")
  else:
    print(total_bill)
class Customer(Bikerental):
  bill=0
  def __init__(s,number_of_bikes,rentalBasis,number_of_days_or_weeks):
    # super().__init__(number_of_bikes,rentalBasis,number_of_days_or_weeks)
    s.number_of_bikes=number_of_bikes
    s.rentalBasis=rentalBasis
    s.number_of_days_or_weeks=number_of_days_or_weeks

  def rentBike(s):
    if s.number_of_bikes<=0:
      print("Number of bikes should be positive!")
    elif s.number_of_bikes>Bikerental.stock:
      print("number_of_bikes available to rent")
    else:
      updated_stock=Bikerental.stock-s.number_of_bikes
      print("Total number_of_bikes rented by the customer",updated_stock)

  def returnBike(s):
    if s.rentalBasis=='day':
      total_bill=100*s.number_of_bikes*s.number_of_days_or_weeks
    elif s.rentalBasis=='week':
      total_bill=500*s.number_of_bikes*s.number_of_days_or_weeks
    elif 3<=s.number_of_bikes<=5:
      discount=0.3*total_bill
      total_bill=total_bill-discount
      print("You are eligible for Family rental promotion of 30% discount")
    # else:
    print(total_bill)

w=Customer(5,'week',3)
w.rentBike()
w.returnBike()
w.displaystock()

