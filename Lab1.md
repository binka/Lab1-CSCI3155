# Lab 1

# Lincoln Samelson
# Collaborators: Brian Gaydon
# Principles of Programming: CSCI 3155

##Question 1  
  #a The pi at line 4 is bound by line 3 as it is declared within a function one line above it.  
    It's scope is only limited to within the circumfrence function.  The pi at line 7 is bound by line 1 as it declared
    within a function but since there is no re-decleration of pi within the area function, it has to get it's value from 
    line 1.
  
  
  
  #b The x on line 3 is bound by line 2.  This is where the the value x is passed into the function and then used.  
	 The x on line 6 is bound by 5. 
	 The x on line 10 is bound by line 5. 
	 The x on line 13 is bound by line 1 because it is outside the scope of the function.  It will use value 3. 
	 Bound by line 1, 2, 5, 8 for different scopes.  


##Question 2 

The body of 'g' is well-typed since:

>`def g(x: Int): ((Int, Int), Int)` because
>>`(b, 1): ((Int, Int), Int)` because
>>>`b: (Int, Int)` because
>>>>`x: Int`
>>>>`1: Int`
>>>`1: Int`
>>`(b, a+1): ((Int,Int),Int)` because
>>>`b: (Int,Int)`
>>>`a+1: Int` because
>>>>`a: Int`
>>>>`1: Int`
	
This function returns either (b, 1) or (b, a+2) they are both of type `((Int, Int), Int)`