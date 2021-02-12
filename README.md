# mathrry
  [![Issues](https://img.shields.io/github/issues/SHI3DO/mathrry?style=for-the-badge)](https://github.com/SHI3DO/mathrry/issues)
  [![Stars](https://img.shields.io/github/stars/SHI3DO/mathrry?style=for-the-badge)](https://github.com/SHI3DO/mathrry)
  [![Forks](https://img.shields.io/github/forks/SHI3DO/mathrry?style=for-the-badge)](https://github.com/SHI3DO/mathrry/network/members)
  [![Downloads](https://img.shields.io/npm/dt/mathrry?style=for-the-badge)](https://www.npmjs.com/package/mathrry)
  [![License](https://img.shields.io/github/license/SHI3DO/mathrry?style=for-the-badge)](https://github.com/SHI3DO/mathrry)  
  
Simple Math Module

## Usage
### Basic arithmetic operations
```js
Addition: mathrry.add
Subtraction: mathrry.sub
Multiplication: mathrry.multi
Division: mathrry.divi
```  
### Extra
```js
mathrry.revdivi
mathrry.revmulti
```
```mathrry.revdivi``` is calculated by inverting the value. Think of it as the opposite of ```mathrry.divi```.  
  
```mathrry.revmulti``` also same as above.  

# 2D
## Coordinate things

### Points
#### The Distance between two points
```js
mathrry.Dbtp(x1,y1,x2,y2)
```  
`x1, x1` are the coordinates of the first point, `x2, y2` are the coordinates of the second point.

#### The Distance between point and line
```js
mathrry.Dbptl(x,y,exp-a,exp-b,exp-c)
```
`x,y` are the coordinates of the point, `exp-a, exp-b exp-c` are from `ax+by+c=0`. Put it in order.

### Triangle
#### Centroid of Triangle
```js
mathrry.CoT(x1,y1,x2,y2,x3,y3)
```
##### Extra
```js
mathrry.CoTx(x1,y1,x2,y2,x3,y3)
mathrry.CoTy(x1,y1,x2,y2,x3,y3)
```  
`mathrry.CoTx` returns the x-coordinate value of the centroid of triangle.  
`mathrry.CoTy` returns the y-coordinate value of the centroid of triangle.  
  
`x1, y1` are the coordinates of the first point, `x2, y2` are the coordinates of the second point, and `x3, y3` are the coordinates of the third point.  

## Area things
### Triangle
#### The Area of triangle with 3 points
```js
mathrry.Aotw3p(x1,y1,x2,y2,x3,y3)
```
`x1, y1` are the coordinates of the first point, `x2, y2` are the coordinates of the second point, and `x3, y3` are the coordinates of the third point.  
#### The Area of triangle with 3 line segments
```js
mathrry.Aotw3ls(l1, l2, l3)
```
`l1, l2, and l3` are the lengths of the sides of the triangle, respectively.  
### Circle
#### Area of Circle
```js
mathrry.AoC(r)
```
`r` is the radius of the circle for which you want to know the area.

# 3D
## Coordinate things
### Points
#### The Distance between two points in 3D
```js
mathrry.TDbtp(x1,y1,z1,x2,y2,z2)
```
`x1, x1, z1` are the coordinates of the first point, `x2, y2, z2` are the coordinates of the second point.  
### Cube
#### The Diagonal of the cube
```js
mathrry.TdoC(l)
```
`l` is the length of one side of the cube.  

#### Volume of Cube
```js
mathrry.TVoC(l)
```
`l` is the length of one side of the cube.

### Sphere
#### Volume of Sphere
```js
mathrry.TVoS(r)
```
`r` is the radius of Sphere.

# Physics
## Force
### F = ma
```js
mathrry.F(m,a)
```
`m` is the mass of an object. `a` is the Acceleration of an object. 
#### Extra
##### m = F/a
```js
mathrry.Fm(f,a)
```
Finding the mass of an object by force and acceleration.
##### a = F/m 
```js
mathrry.Fa(f,m)
```
Finding the acceleration of an object by force and mass.  
### S = V0t + 1/2at^2
```js
mathrry.S(v,a,t)
```
`v` is the initial velocity of an object. `t` is the time of the force was applied to the object. `a` is the Acceleration of an object.  
#### Extra
##### V0 = (S - 1/2at^2)/t
```js
mathrry.Sv(s,a,t)
```
`s` is the moving space of the object. `a` is the Acceleration of an object. `t` is the time of the force was applied to the object.  
##### a = (s - v0t)/(0.5t^2)
```js
mathrry.Sa(s,v,t)
```
`s` is the moving space of the object. `v` is the initial velocity of an object. `t` is the time of the force was applied to the object.  

### 2as = v^2 - v0^2
```js
mathrry.A(v0,v,s)
```
`v0` is the initial velocity of an object. `v` is the later speed of the object. `s` is the moving space of the object.
