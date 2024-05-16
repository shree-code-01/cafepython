# cafepython
menu={
    'PIZZA':50,
     'PASTA':50,
     'SALAD':70,
     'BURGER':80,
     'COFFEE':30,

}


print("WELCOME TO OUR CAFE")
print("PIZZA: RS50\n PASTA: RS50\n SALAD RS70\n BURGER RS 80\n COFFEE RS30\n")

ORDER_TOTAL=0
#80+70=150
item=input("enter name of item you wanna order")
if item in menu:
    ORDER_TOTAL += menu[item]
    print(f"your item {item} has added in order")
else:
    print(f"ORDERED ITEM {item} IS NOT IN MENU")
 
anotheritem=input("wanna order new item ?(yes/no)")
if anotheritem=="YES":
    item2=input("enter 2nd item")
    if item2 in menu:
     ORDER_TOTAL +=menu[item2]
     print(f"item {item2} is added")
    else:
       print(f"ordered item{item2} not in list")

print(f"order total is {ORDER_TOTAL}")
