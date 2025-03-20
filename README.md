# Assignment1py
while True:

    try:
        
	num1=float(input("Enter the first number:"))
       
	num2=float(input("Enter the second number:"))
    
    except ValueError:
        
	print("Invalid input.Please enter numbers only.")
        
	continue
  
    while True:
        
	operation=input("Enter the operation(+,-,*,/):")
     
	if operation=="back":
           
	    break
        
	if operation == '+':
           
	    result = num1 + num2
        
	elif operation == '-':
           
	    result = num1 - num2
        
	elif operation == '*':
           
	    result = num1 * num2
      
	elif operation == '/':
           
	    if num2 == 0:
               
		print("Error!")
               
		continue
            result = num1 /num2
        else:
	        print("Invalid operation!Please try again.")
	        continue
        print("Result:",result)
        break
