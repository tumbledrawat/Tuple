#16. Consider a tuple t1=(1,2,5,7,9,2,4,6,8,10). Write a program to perform following operations: 
#a. Print half the values of tuple in one line and the other half in the next line.
#b. Print another tuple whose values are even numbers in the given tuple. 
#c. Concatenate a tuple t2=(11,13,15) witht1. 
#d. Return maximum and minimum value from this tuple.
t1=(1,2,5,7,9,2,4,6,8,10)

#a
t1=(1,2,5,7,9,2,4,6,8,10)
a= int(len(t1)/2)
print(t1[ :a])
print (t1[a: ])

#b
t1=(1,2,5,7,9,2,4,6,8,10)
t2= []
for i in range(len(t1)+1):
   if(i%2==0):
     t2.append(i)
   else:
     continue
t2=tuple(t2)
print(tuple(t2))

#c
t1=(1,2,5,7,9,2,4,6,8,10)
t2= (11,13,15)
a= t1+ t2
print (t1+t2)

#d
a=(1, 2, 5, 7, 9, 2, 4, 6, 8, 10, 11, 13, 15)
b=max(a)  
c=min(a)
print(b)
print(c)
