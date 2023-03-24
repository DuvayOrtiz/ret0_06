# ret0_06
haciendo esto antes de las 10 :O

## Mero power
### Ejercicios
#### 1
ejercicio de las masas y la fuerza entre ellas(se hizo en clase pero ahi está) 

```ruby
def calcularFuerza (m1:float, m2:float, G:float, r:float) -> float:    
  fuerzaEjercida = G*m1*m2/(r**2)
  return fuerzaEjercida
if __name__ == "__main__":
  m1 = float(input("Ingrese masa de cuerpo 1:"))
  m2 = float(input("Ingrese masa cuerpon 2:"))
  r = float(input("Ingrese la distancia entre los cuerpos en metros:"))
  G: float = 6.67384e-11 
  fuerzaFinal = calcularFuerza(m1, m2, G, r )
  print("la fuerza entre los cuerpos es  " + str(fuerzaFinal))


```
#### 2
```ruby
import math        #importo "math"
def valorAbs(x:float):    
    return math.fabs(x)
def techo(X):
    return math.ceil(x)      
def suelo(X):
    return math.floor(x)      
def gamma(X):
    return math.gamma(x)       
def lgamma(X):
    return math.lgamma(x)       

if __name__ == "__main__":
    x=float(input("ingresar valor: "))
    
    valorAbsoluto=valorAbs(x)
    numeroTecho=techo(x)
    numeroSuelo=suelo(x)
    gammaa=gamma(x)
    lgammaa=lgamma(x)
        
    print("la distancia del punto al origen es  " + str(valorAbsoluto))
    print("el numero mas proximo entero por derecha es  " + str(numeroTecho))
    print("el numero mas proximo entero por izquierda es  " + str(numeroSuelo))
    print("el valor en esa x de la funcion gamma es " + str(gammaa))
    print("el ln  del valor absoluto de la funcion gamma  " + str(lgammaa))```

```

### punto 01
```ruby
import math
Pi=math.pi
def volumen(r1:float, r2:float, h:float): 
    return ((r1**3)*Pi*(4/3))+((r2**2)*Pi*h)
def areaSup(r1, r2, h):
    return (4*Pi*(r1**2))+((Pi*h*r2)+((r2**2)*Pi))
if __name__ == "__main__":
    r1=float(input("ingresar radio de la esfera: "))
    r2=float(input("ingresar radio de la base del cono : "))
    h=float(input("ingresar altura del cono : "))
    volumenFig = volumen(r1, r2, h)
    areaSupFig = areaSup(r1, r2, h)
    print("el volumen de la figura es " + str(volumenFig))
    print("el area supericial de la figura es  " + str(areaSupFig))
```


### punto 2
```ruby
import math
pi = math.pi
def areaFig(a:float, b:float, r1:float, r2:float):
    return (a*b)+((r1**2)*pi)+((r2**2)*pi)
def periFig(a, b, r1, r2):
    return (2*a)+(2*b)+(2*pi*r1)+(2*pi*r2)

if __name__ == "__main__":
    r1=float(input("ingresar radio del circulo 1: "))
    r2=float(input("ingresar radio del circulo 2: "))
    a=float(input("ingresar un lado del rectangulo : "))
    b=float(input("ingresar un lado del rectangulo (que no sea el lado paralelo al anterior) : "))
    perimetroFig = periFig(r1, r2, a, b)
    areaFigu = areaFig(r1, r2, a, b)
    print("el area de la figura es  " + str(areaFigu))
    print("el perimetro es  " + str(perimetroFig))
```



### punto 3
```ruby
#Ejerpollos
def pollos(a:float, b:float, c:float):
    return (a*6)+(b*7)+(c)
if __name__ == "__main__":
    a=float(input("ingresar numero de gallinas en Kg: "))
    b=float(input("ingresar numero de gallos en Kg: "))
    c=float(input("ingresar numero de pollos en Kg: "))
    numeroAves=pollos(a,b,c)
    print("el peso de todas las aves en Kg es  " + str(numeroAves))
```
### punto 4
```ruby
def vueltos(a:float, b:float, c:float):
    return (a*300)+(b*3300)+(c*350)
if __name__ == "__main__":
    a=float(input("ingresar numero de panes: "))
    b=float(input("ingresar numero de bolsas de leche "))
    c=float(input("ingresar numero huevos: "))
    plata=int(input("ingresar el billete que dió la cucha: "))
    vueltas=vueltos(a,b,c)
    def sobra(plata, vueltas):
        return plata-vueltas
    
    if sobra(plata, vueltas) >= 0:
        print("los vueltos son ", sobra (plata, vueltas))
    else:
        print("faltan ", abs(sobra (plata, vueltas)))
```
### punto 5
```ruby
def interes(ci, i, nm):
    return ci*(1+i)**nm
if __name__ == "__main__":
      ci=float(input("¿cuanta plata pidió? : "))
      i=float(input("¿cual es el interes?: "))
      nm=float(input("meses que se le subio eso: "))
      cf=interes(ci, nm, i)
      print("usted debe "+ str(cf))

```
### punto 6
```ruby
---> en este codigo queria verificar si era necesario definir funcion principal.
def contagiados(c:float, n:float):
    return c*(2**n)      
c=float(input("numero de contagiados : "))
n=float(input("numero de dias : "))
print("el numero de vagos contagiados es ", contagiados(c,n))


```
### el import
```ruby
import  statistics
def mediana(numeritos):
    return statistics.median(numeritos)
def prom(numeritos):
    return statistics.mean(numeritos)

def menMay(numeritos):
    return sorted(numeritos)
def mayMen(numeritos):
    return sorted((numeritos), reverse=True)
def pot(numeritos):
    return (max(numeritos))**(min(numeritos))
def raiz(numeritos):
    return (min(numeritos))**(1/3)
```

### punto 7
```ruby
from ejerci import*
def promMul(numeritos):
    return (n1*n2*n3*n4*n5)**0.5
n1 = float(input("Ingresar número 1: "))
n2 = float(input("Ingresar número 2: "))
n3 = float(input("Ingresar número 3: "))
n4 = float(input("Ingresar número 4: "))
n5 = float(input("Ingresar número 5: "))
numeritos = [n1, n2, n3 , n4 , n5]
print("el promedio aritmetico es  ", prom(numeritos))
print("el promedio multiplicativo es ", promMul(numeritos))
print("la mediana es ", mediana(numeritos))
print("de menor a mayor son ", menMay(numeritos))
print("de menor a mayor son ", mayMen(numeritos))
print("el mayor elevado al menor es ", pot(numeritos))
print("la raiz cubica del menor es ", raiz(numeritos))
```

## puntos 8
El pip es un sistema instalador y de gestión de paquetes utilizado para paquetes de software de python.

paquetes usuales: (segun google)
+ TensorFlow
+ Scikit-Learn
+ Numpy
+ Keras
+ PyTorch
+ LightGBM
+ Eli5
+ SciPy
+ Theano
+ Pandas

Es facil instalar dichos paquetes unicamente se pone
```
pip install "nombre del paquete"

```



















































































