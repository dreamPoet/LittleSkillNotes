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

$d(g(h(x))/dx = g'(h(x))*h'(x)$


![](Calculus_3blue1brown_4.png)



## Chapter 5 Derivatives of exponentials

$e^x$

![](Calculus_3blue1brown_5.png)

So, we can get $2^t * (2^{dt} - 1) / dt$
For $(2^{dt} - 1) / dt$ which has no relation with time t, it tends to a constant $0.6931472...$

In fact for all $n^t$ we can find a different constant * itself as the derivative

the number $e$ is defined to make $(e^{dt} - 1) / dt$ equal to 1.

so, $\frac{d}{dt}(e^t) = e^t$

For those constant, we use chain rule to related to $e$.
$2 = e^{ln(2)}$

$2^t =e^{ln(2)t}$

so, the derivative of $2^t = ln(2) * e^{ln(2)t} = ln(2)*2^t$

![](Calculus_3blue1brown_6.png)

In fact there can be many different ways to express, we use $e$ since it is the proportionality constant btw **the size of changing variable and the rate of change**. 


## Chapter 6 Implicit differentiation

implicit curve: not simply y = f(x), x and y are correlated via some relashionship. It's just the set of all points(x,y) that satisfy some property written in terms of the two variables x and y.

![](Calculus_3blue1brown_7.png)

we just regard them as (x,y), and the changing on these components will cause on changes on the whole pair.

Another example to use this:
![](Calculus_3blue1brown_8.png)

so, $\frac{dy}{dx}=\frac{1}{e^y}=\frac{1}{x}$



## Chapter 7 Limits

![](Calculus_3blue1brown_9.png)

RHS is the formal derivative definition.
$h = dx$

introduce h because someone think dx means infinite small, while someone think dx is just a value.

To conclude, we are talking about **the size of change approaches to zero** instead of **infinitely small changes**.


so, we need  to understand the meaning of **approach**

$(\epsilon,\delta)$

$\epsilon$ for the output distance (when trying to approach the limit), it may cannot be smaller when limit does not exist.

![](Calculus_3blue1brown_10.png)


for second case, the $\epsilon$ is too small, no matter how small the $\delta$ is, the output is always bigger.
![](Calculus_3blue1brown_11.png)

how to comput limit?
"L' Hopital's rule"

In the case of $\frac{0}{0}$, the limit can be calculated via

![](Calculus_3blue1brown_12.png)

There are other cases for L' Hopital's rule.


## Chapter 8 Integration and the fundamental theorem

Inverse of the derivatives

![](Calculus_3blue1brown_13.png)

as we can see, the added area $ds = v(t)*dt$

so we can get the formula $\frac{ds}{dt} = v(t)$, which means the derivative of the area under the graph equals to the function of this graph. So the area can be calculated via finding the anti-derivative function.



Then, use lower bound to make sure the correct constant.

To cancel T=0

![](Calculus_3blue1brown_14.png)


Calculate area:
Fundamental theorem of calculus:

![](Calculus_3blue1brown_15.png)


Negative area: backwards; will be substracted.

Integral == signed area between the graph and the horizontal axis.


## Chapter 9 What does area have to do with slope?

How to find the average of a continous function of a period?

sum of the height / number of points

![](Calculus_3blue1brown_16.png)

when we take points in the gap of dx, we can get numbers of points equals to $\pi/dx$

![](Calculus_3blue1brown_17.png)

![](Calculus_3blue1brown_18.png)

After rearranging, we can get the numerator as the integral.

$average \quad height = \frac{area}{width}$


![](Calculus_3blue1brown_19.png)

<br>

Last chapter shows that in one situation we should use integral: **the problem could be approximated by vreaking it up and then adding up a large number of small things**

Through this video, we should have a second sensation about integral: **for limited number of values, we can simplily use addition to get average, for infinite values, we should use integrals, especially in probability.**

![](Calculus_3blue1brown_20.png)

<br><br>

## Higher order derivatives

notion:

$\frac{d\frac{df}{dx}}{dx} = \frac{d}{dx} * \frac{df}{dx} = \frac{d^2f}{dx^2}$

the derivative of derivative of $f$

take the car as example:

![](Calculus_3blue1brown_21.png)


<br><br>

## Chapter 10 Taylor series

Polynomial is much easy when computing.


![](Calculus_3blue1brown_22.png)

To approximate the curve around zero, we need to satisfy left conditions.

Finally, we can get $cos(x)=1-\frac{1}{2}x$

To be more accurate, we can add more polynomials like $x^3$ meeting third derivatives, etc.

<br>

Some tips:

1. there will be a factorial as chains of derivatives
2. later terms coeffecients' calculation will not influence previous ones. As when calculate one item, later higher ordered items with $x$ will be $0$.
3. one term corresponding to one order of derivative.
4. to approximate on other point $a$, just use $(x-a)$ to replace $x$ get a easier computation.

![](Calculus_3blue1brown_23.png)

![](Calculus_3blue1brown_24.png)

![](Calculus_3blue1brown_25.png)

![](Calculus_3blue1brown_26.png)


What we do is to transform **derivative information at a point** to **output information near that point**

![](Calculus_3blue1brown_27.png)


general term:

![](Calculus_3blue1brown_28.png)

![](Calculus_3blue1brown_29.png)


<br>

Geometric view to display second term of Taylor polynomial:


![](Calculus_3blue1brown_30.png)

Height is calculated as $slop * (x-a)$ where the slop is the changing(derivative) of the speed($d'(a)$) on point $a$, so finally it equals to $d''(x-a)$.


<br>
In math **Infinite sum** == **series**

So we call these terms **Taylor series** .

**convergence** (equal) to the needed value.

The series of some functions **only converge within a certain range around the input whose derivative information used** 

![](Calculus_3blue1brown_31.png)


Most important intuition for Taylor series:
*What we do is to transform **derivative information at a point** to **output information near that point***


<br><br>
End. 2018/04/13. London.