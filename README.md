# dictinareies

#1. Write a program that repeatedly asks the user to enter product names and prices. Store all
#of these in a dictionary whose keys are the product names and whose values are the prices.
#When the user is done entering products and prices, allow them to repeatedly enter a product
#name and print the corresponding price or a message if the product is not in the dictionary.


no_of_prods=eval(input("Enter number of products: "))
prods={}
for i in range(no_of_prods):
    p= input("Enter product name: ")
    prods[p]= int(input("Enter product price:"))
while True:
    p= input("Enter product name:")
    if p in prods:
        print("Price is", prods[p])
    else:
        print("This product is not in dictionary.")
        break
        
#2. Using the dictionary created in the previous problem, allow the user to enter a dollar amount
#and print out all the products whose price is less than that amount.


no_of_prods=eval(input("Enter number of products: "))
prods={}
for i in range(no_of_prods):
    p= input("Enter product name: ")
    prods[p]= int(input("Enter product price:"))
amount=eval(input("Enter amount:"))
if amount>prods[p]:
  print(prods[p])
  
