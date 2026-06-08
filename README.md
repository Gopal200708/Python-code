product=[]

total=0

bill=0

while 1:


    name=input('Enter name:- ')

    if name!='stop':

    
        product.append(name)
    
        price=int(input("Enter price:- "))
    
        total+=price

    else:
    
        print('Total Quantity= ',len(product))
    
        print("Total Price= ",total)
    
        cash=int(input('enter cash: '))
    
        bill+=cash
    
    
    
        if cash<total:
        
            print("insufficient money give more: ",total-cash)
        
            cash=int(input("enter more cash: "))
        
            bill+=cash
        
            print("received: ",bill)
        
            print("Return: ",bill-total)
        
         
        
        else:
        
            print("received: ",bill)
        
            print("Return: ",bill-total)
    
        break
