sys module contains getrefcount() function for this purpose.
sys.getrefcount(objectreference)

import sys
class Test:
    pass
         
t1=Test()
t2=t1
t3=t1
t4=t1
print(sys.getrefcount(t1))
