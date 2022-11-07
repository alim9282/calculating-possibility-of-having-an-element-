# calculating-possibility-of-having-an-element-
import itertools 
from itertools import product
e = ['a','c','v','d','f']
b = [1,4,5,]
d = ['true','false']
c = list(itertools.product(e,b,d))
k = len(c)
#print(c)
i = 0
x = 0
y = 0
while i<k:
    if "a" in c[i]:
        x = x+1
    else:
        y = y+1
    i = i +1   
percent = (x/k)*100   
print(percent,"%")
