# collazt-with-out-value-error
def collatz(n):
    if n %2 == 0:
        print(int(n/2))
        return(int(n/2))
        
    else:
        print(int(n*3+1))
        return(int(n*3+1))
    
    
    
print('Please enter a number and the Collatz sequence')
try:
    x = int(input())
except ValueError:
    print('Error invalid value plz enter integers only.')
    
while x != 1:
    x = collatz(x)
