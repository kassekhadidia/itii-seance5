# itii-seance5


                                                               TP5 python

Exercice1


def cal_tauxvariation(f,a,h):
    tauxvariation=(f(a+h)-f(a))/h
    return tauxvariation

from sympy.utilities.lambdify import lambdify
from sympy.abc import x, y, z

f = lambdify(x, 3*x**3 +x**2 -5)
a=0
h=1
print(cal_tauxvariation(f,a,h))


Exercice2
def coefdirecteur(fn, a, b,p):
    coef = []
    for i in range(a,b,p):
        return coef
def fn(x):
return (1+x)/(x-4)
coef(fn, 0, 1, 2)


Exercice4

def T(n):
    return (n**2-((n-1)**2))

def S(n):
    res = 0
    for i in range(1, n+1):
        res = res + T(i)
    return res

S(3)

Exercice¬6
def val_app(epsilon): 
    elm1=1
    elm2=elm1-1/(3**2)
    signe=1
    val=5
    while abs(elm2-elm1)>epsilon:
       elm1=elm2
       elm2=elm1+signe*(1/(val**2))
       val+=2
       signe*=(-1)
    return elm2

EXERCICE 5
 def deter(e, u0):
    b = 1;
    un = u0
    n = 0;
    while ( b == 1 ):
        un = uN(un)
        print(un)
        if(un < e):
            b = 0
        else:
            n+=1

    return n;

def uN(un):
    return 0.5*un

deter(5, 2)

exercice 7
def limite(epsilon):
    U0 = 2
    Un = U0+2/U0
    while abs(Un-U0) > epsilon:
        U0 = Un
        Un = U0+2/U0
    return Un
 
 
print(limite(0.05)
