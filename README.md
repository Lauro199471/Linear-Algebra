# Linear-Algebra

``` python
class colors: 
    reset='\033[0m'
    bold='\033[01m'
    disable='\033[02m'
    underline='\033[04m'
    reverse='\033[07m'
    strikethrough='\033[09m'
    invisible='\033[08m'
    class fg: 
        black='\033[30m'
        red='\033[31m'
        green='\033[32m'
        orange='\033[33m'
        blue='\033[34m'
        purple='\033[35m'
        cyan='\033[36m'
        lightgrey='\033[37m'
        darkgrey='\033[90m'
        lightred='\033[91m'
        lightgreen='\033[92m'
        yellow='\033[93m'
        lightblue='\033[94m'
        pink='\033[95m'
        lightcyan='\033[96m'
    class bg: 
        black='\033[40m'
        red='\033[41m'
        green='\033[42m'
        orange='\033[43m'
        blue='\033[44m'
        purple='\033[45m'
        cyan='\033[46m'
        lightgrey='\033[47m'
       
       
       print(colors.bg.green, "SKk", colors.fg.red, "Amartya") 
print(colors.bg.lightgrey, "SKk", colors.fg.red, "Amartya") 

import numpy as np 
A = np.random.randint(1,13,(5,5)); 
print(A , "\n") 
print(A.shape , "\n") 


print('{}{:2d} {:2d} {:2d} {:2d} {:2d}{}'.format(colors.fg.red,A[0,0],A[0,1],A[0,2],A[0,3],A[0,4],colors.reset));
print('{:2d} {:2d} {:2d} {:2d} {:2d}'.format(A[1,0],A[1,1],A[1,2],A[0,3],A[1,4]))
print('{:2d} {:2d} {:2d} {:2d} {:2d}'.format(A[2,0],A[2,1],A[2,2],A[0,3],A[2,4]))
print('{:2d} {:2d} {:2d} {:2d} {:2d}'.format(A[3,0],A[3,1],A[3,2],A[0,3],A[3,4]))
print('{:2d} {:2d} {:2d} {:2d} {:2d}'.format(A[4,0],A[4,1],A[4,2],A[0,3],A[4,4]))

print('{}{:2d}{} {:2d} {:2d} {:2d} {:2d}'.format(colors.fg.blue,A[0,0],colors.reset,A[0,1],A[0,2],A[0,3],A[0,4]))
print('{}{:2d}{} {:2d} {:2d} {:2d} {:2d}'.format(colors.fg.blue,A[1,0],colors.reset,A[1,1],A[1,2],A[0,3],A[1,4]))
print('{}{:2d}{} {:2d} {:2d} {:2d} {:2d}'.format(colors.fg.blue,A[2,0],colors.reset,A[2,1],A[2,2],A[0,3],A[2,4]))
print('{}{:2d}{} {:2d} {:2d} {:2d} {:2d}'.format(colors.fg.blue,A[3,0],colors.reset,A[3,1],A[3,2],A[0,3],A[3,4]))
print('{}{:2d}{} {:2d} {:2d} {:2d} {:2d}'.format(colors.fg.blue,A[4,0],colors.reset,A[4,1],A[4,2],A[0,3],A[4,4]))

A = np.random.randint(1,13,(5,5));
B = np.random.randint(1,13,(5,5));

print('A = \n')
print('{:2d} {:2d} {:2d} {:2d} {:2d}'.format(A[0,0],A[0,1],A[0,2],A[0,3],A[0,4]));
print('{:2d} {:2d} {:2d} {:2d} {:2d}'.format(A[1,0],A[1,1],A[1,2],A[0,3],A[1,4]))
print('{}{:2d} {:2d} {:2d} {:2d} {:2d}{}'.format(colors.fg.red,A[2,0],A[2,1],A[2,2],A[0,3],A[2,4],colors.reset))
print('{:2d} {:2d} {:2d} {:2d} {:2d}'.format(A[3,0],A[3,1],A[3,2],A[0,3],A[3,4]))
print('{:2d} {:2d} {:2d} {:2d} {:2d}'.format(A[4,0],A[4,1],A[4,2],A[0,3],A[4,4]))

print('\n\n')
print('A(row 3) = {}{:2d} {:2d} {:2d} {:2d} {:2d}{}'.format(colors.fg.red,A[2,0],A[2,1],A[2,2],A[0,3],A[2,4],colors.reset))
As = 'A(row 3) = {}{:2d} {:2d} {:2d} {:2d} {:2d}{}'.format(colors.fg.red,A[2,0],A[2,1],A[2,2],A[0,3],A[2,4],colors.reset);

print('B = \n')
clr1 = colors.fg.blue; 
clr2 = colors.reset; 

print('{:2d} {:2d} {:2d} {}{:2d}{} {:2d}'.format(B[0,0],B[0,1],B[0,2],clr1,B[0,3],clr2,B[0,4]))
print('{:2d} {:2d} {:2d} {}{:2d}{} {:2d}'.format(B[1,0],B[1,1],B[1,2],clr1,B[1,3],clr2,B[1,4]))
print('{:2d} {:2d} {:2d} {}{:2d}{} {:2d}'.format(B[2,0],B[2,1],B[2,2],clr1,B[2,3],clr2,B[2,4]))
print('{:2d} {:2d} {:2d} {}{:2d}{} {:2d}'.format(B[3,0],B[3,1],B[3,2],clr1,B[3,3],clr2,B[3,4]))
print('{:2d} {:2d} {:2d} {}{:2d}{} {:2d}'.format(B[4,0],B[4,1],B[4,2],clr1,B[4,3],clr2,B[4,4]))

print('\n\n')
print('B(col 4) =\n{}{:2d}\n{:2d}\n{:2d}\n{:2d}\n{:2d}{}'.format(colors.fg.blue,B[0,3],B[1,3],B[2,3],B[3,3],B[4,3],colors.reset))
Bs = 'B(col 4) =\n{}{:2d}\n{:2d}\n{:2d}\n{:2d}\n{:2d}{}'.format(colors.fg.blue,B[0,3],B[1,3],B[2,3],B[3,3],B[4,3],colors.reset);

print(As ,'\n*\n',Bs)
C = np.dot(A[2,:],B[:,3]);
print(C)
C = np.dot(A,B);
print(C)

# Matrix Vector Multiplicaiton to get C Matrix
print('A =')
print(colors.fg.red)
print('{:2d} {:2d} {:2d} {:2d} {:2d}'.format(A[0,0],A[0,1],A[0,2],A[0,3],A[0,4]))
print('{:2d} {:2d} {:2d} {:2d} {:2d}'.format(A[1,0],A[1,1],A[1,2],A[0,3],A[1,4]))
print('{:2d} {:2d} {:2d} {:2d} {:2d}'.format(A[2,0],A[2,1],A[2,2],A[0,3],A[2,4]))
print('{:2d} {:2d} {:2d} {:2d} {:2d}'.format(A[3,0],A[3,1],A[3,2],A[0,3],A[3,4]))
print('{:2d} {:2d} {:2d} {:2d} {:2d}'.format(A[4,0],A[4,1],A[4,2],A[0,3],A[4,4]))


print('B = \n')
clr1 = colors.fg.blue; 
clr2 = colors.reset; 

print('{}{:2d}{} {:2d} {:2d} {:2d} {:2d}'.format(clr1,B[0,0],clr2,B[0,1],B[0,2],B[0,3],B[0,4]))
print('{}{:2d}{} {:2d} {:2d} {:2d} {:2d}'.format(clr1,B[1,0],clr2,B[1,1],B[1,2],B[1,3],B[1,4]))
print('{}{:2d}{} {:2d} {:2d} {:2d} {:2d}'.format(clr1,B[2,0],clr2,B[2,1],B[2,2],B[2,3],B[2,4]))
print('{}{:2d}{} {:2d} {:2d} {:2d} {:2d}'.format(clr1,B[3,0],clr2,B[3,1],B[3,2],B[3,3],B[3,4]))
print('{}{:2d}{} {:2d} {:2d} {:2d} {:2d}'.format(clr1,B[4,0],clr2,B[4,1],B[4,2],B[4,3],B[4,4]))
print('\n')
print('{:2d} {}{:2d}{} {:2d} {:2d} {:2d}'.format(B[0,0],clr1,B[0,1],clr2,B[0,2],B[0,3],B[0,4]))
print('{:2d} {}{:2d}{} {:2d} {:2d} {:2d}'.format(B[1,0],clr1,B[1,1],clr2,B[1,2],B[1,3],B[1,4]))
print('{:2d} {}{:2d}{} {:2d} {:2d} {:2d}'.format(B[2,0],clr1,B[2,1],clr2,B[2,2],B[2,3],B[2,4]))
print('{:2d} {}{:2d}{} {:2d} {:2d} {:2d}'.format(B[3,0],clr1,B[3,1],clr2,B[3,2],B[3,3],B[3,4]))
print('{:2d} {}{:2d}{} {:2d} {:2d} {:2d}'.format(B[4,0],clr1,B[4,1],clr2,B[4,2],B[4,3],B[4,4]))
print('\n.\n.')



C1 = np.dot(A,B[:,0]);
C2 = np.dot(A,B[:,1]);
C3 = np.dot(A,B[:,2]);
C4 = np.dot(A,B[:,3]);

print("C[:,1]:");
print(colors.fg.purple);
print('{:2d}\n{:2d}\n{:2d}\n{:2d}\n{:2d}'.format(C1[0],C1[1],C1[2],C1[3],C1[4]));
print(colors.reset);

print("C[:,2]:");
print(colors.fg.purple);
print('{:2d}\n{:2d}\n{:2d}\n{:2d}\n{:2d}'.format(C2[0],C2[1],C2[2],C1[3],C2[4]));
print(colors.reset);

print("C[:,3]:");
print(colors.fg.purple);
print('{:2d}\n{:2d}\n{:2d}\n{:2d}\n{:2d}'.format(C3[0],C3[1],C3[2],C3[3],C3[4]));
print(colors.reset);

print("C[:,4]:");
print(colors.fg.purple);
print('{:2d}\n{:2d}\n{:2d}\n{:2d}\n{:2d}'.format(C4[0],C4[1],C4[2],C4[3],C4[4]));
print(colors.reset);

C = (C1,C2,C3,C4);
C = np.asmatrix(C)
print(C)
```
