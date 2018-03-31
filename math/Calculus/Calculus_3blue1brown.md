# The Essence of Calculus



## Chapter 1

Start point: calculate the area of a circle.

hard problem -> sum of many small values

We can get the idea that at high level, many problem can be regarded as finding the area under some graph.


The function trying to find this area is called Integral of the original function.

![](Calculus_3blue1brown_1.png)

so, 

$$ dA / dx = x^2 $$

which can be called **Derivative**, which measures how sensitive a function is to small changes in input. (It is also a key to solve integral)


when dx becomes smaller, this formular become more accurate.




## Chapter 2 The paradox of the derivative.

paradox:  instantaneous rate of change?

but change requires multiple points in time (to measure), while Instantaneous = one point in time

can be calculated as the slope of **two points** when gap (dt) is infinitely small.

$ds(t)/dt = (s(t+dt) -s(t)) / dt$ 

BUT, pure math derivative: tangent at a **single point**. which makes dt very close to 0

regard this tangent as **Best constant approximation around a point (range)** instead of instantaneous change

The process of calculate $s(t) = t^3$. When dt is tent to 0, the item contains dt can be ignored and finally we can get $3t^2$

![](Calculus_3blue1brown_2.png)





## Chapter 3 Derivative formulas through geometry.

visualise $x^2$ and $x^3$ as square and cube, see how area or volume changed when add small $dx$


The point: most of the complication can be ignored and the bigest one is reserved.





## Chapter 4 Chain rule


add:  $d(g(x)+h(x)) / dx = dg/dx + dh/dx$

product:  $d(g(x)*h(x)) / d(x) = g(x)*dh/dx+ h(x)*dg/dx$

![](Calculus_3blue1brown_3.png)


***Chain rule** - composition: 

$d(g(h(x))/dx = d(g(h(x)))/dh * dh(x)/dx = dg/dh * dh/dx = dg/dx$

![](Calculus_3blue1brown_4.png)



## Chapter 5 Derivatives of exponentials

$e^x$




## Chapter 6 Implicit differentiation