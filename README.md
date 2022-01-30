# Python_project
#code
class customer:
    def __init__(self,c1,c2,c3,c4):
        self.customer_1= c1
        self.customer_2= c2
        self.customer_3= c3
        self.customer_4= c4
    def name(self):
        self.name=input('Enter your name: ')   
    def phone_number(self):
        self.phone_number=input('Enter your phone number: ')
    def email(self):
        self.email=input('Enter your Email: ')
    def address(self):
        self.address=input('Enter your address')
    def password(self):
        self.password=input('Enter your password')
username=[]
password=[]
username.append(name)
password.append(password)
if name in (username):
    print('you can login')
else:
    print("Register yourself")


li=[]
yes_condition='y'
while yes_condition=='y':
    print("LIST OPERATIONS")
    print("1. Add FoodItems")
    print("2. Edit the list")
    print("3. Remove an item from the list")
    print("4. Insertion of new fooditem into the list")
    print("5. View the final list of fooodItem")

    ch=int(input("Enter your choice:"))
    if ch==1:
        size=int(input("Enter the size of List:"))
        for x in range(size):
            val=(input("Enter the name of foodItem:"))
            li.append(val)
        print(li)
    if ch==2:
        print(li)
        pos=int(input("Enter the position to be updated:"))
        val=(input("Enter updated value:"))
        li[pos]=val
        print("Record updated:")
        print(li)
    if ch==3:
        print(li)
        pos=int(input("Enter the position to be deleted:"))
        li.pop(pos) 
        print("After deletion list is:",li)
    if ch==4:
        print(li)
        pos=int(input("Enter the position:"))
        val=(input("Enter the FoodId:"))
        li.insert(pos,val)
        print("After insertion list is ",li)
    if ch==5:
        print("Final list of foodItems are:")
        for x in li:
            print(x)
    yes_condition=input("Do you want to continue?[y/n]:")
Full_Name=input("Enter your full Name: ")
Phone_No=int(input("Enter your Conatct Number: "))
Email=input("Enter your email Id: ")
Address=input("Enter your address: ")
Password=input("Save your unique password, for future use")
login_info={'Naman':'#123',
            'krunal':'3333',       #AdminInfo
            'Kartik':'3322'}
Log_In_Admin=input("Enter your AdminId: ")
Password_Admin=input("Enter your password")
def log_in(Log_In_Admin,Password_Admin):
    pw=login_info.get(Log_In_Admin)
    if pw!=Password_Admin:
        print('wrong username or password')
        return False
    else:
        return True


print("1.Add new food items.\n2.Edit food items using FoodID.\n3.View the list of all food items.\n4.Remove a food item from the menu using FoodID.")

Log_In_User=input("Enter your UserId: ")
Password_User=input("Enter your password")
    

        
print("1.Place New Order.\n2.Order History\n3.Update Profile\n4.Update Profile\n5.Order History")
input_1 = str(input("Please Select Your Operation: ")).upper()

List_of_food_items=[{'Name':'Tandoori Chicken',
                     'Quantity':'4 pieces',
                     'Price': 'INR 240',
                     'Id':'A101',
                     'discount_rate_1':0.05},
                    {'Name':'Vegan Burger',
                        'Quantity':'1 piece',
                     'Price': 'INR 320',
                     'Id':'A102',
                      'discount_rate_2':0.10},
                    {'Name':'Truffle Cake',
                    'Quantity':'500 gms',
                     'Price': 'INR 900',
                     'discount_rate_3':0.15,
                     'Id':'A103'}]
foods=['Tandoori Chicken','Vegan Burger','Truffle Cake']
def choose_foods():
    for food in foods:
        print(foods)
        food=input('Which food do you like to order')
        zomato.make_order(food)
choose_foods()

discount_rate_1 = 0.05                
discount_rate_2 = 0.10               
discount_rate_3 = 0.15


def get_order():
    current_order = li
    while True:
        print("What can I get for you?")
        order = input()
        if order in li:
            print("Ok sure, and anything else")
            current_order.append(order)
        else:
            print("I'm sorry, we don't serve that.")
order = get_order()
