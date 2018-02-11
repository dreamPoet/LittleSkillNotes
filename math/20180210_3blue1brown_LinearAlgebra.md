# Essense of Linear Algebra 



Link: https://www.youtube.com/playlist?list=PLZHQObOWTQDPD3MizzM2xVFitgF8hE_ab

Geometric intuition is helpful.

## Vector

physics: direction + length

CS: ordered lists of numbers

Math: generalize both: can be anything where **adding** 2 vectors and **multiplying** with a number is meaningful.



an arrow rooted at origin

the meaning of LA can be regarded as achieving the transformation btw ordered lists and arrow in space

what happned in space? -> to vector



## Vector Space

Consider components of a vector as a scalar which working on two special unit vector, which is along x-axis and y-axis, called i_hat(along x) and j_hat(along y)

i_hat and j_hat are the **basis vectors** of the xy coordinate system. We can choose **different** basis vectors.

**linear combination** of two vectors (Scalars+addition)

why call linear: if you fix one vector and change another vector, you will get a line

( maybe two vectors in one line; or even two zero vectors

The **span** of two vectors is the set of all their **linear combinations**, which is the addition and scalar.

In fact, a vector should be regarded as an arrow. but, it is too crowed when we describe loads of vectors. So when think of sets of vectors, we regard them as **points**. 

three dimensional vector: two vectors form a  plane. the last one can be regarded as moving this plane on its direction. finally form the whole room

Redundant vectors : linearly dependent

if all vectors add dimension to the span: linearly independent

**The basis of a vector space is a set of linearly independent vectors that span the full space.**



## Matrix as Linear transformations



transformation = function

vector input -> vector output

use **transformation** instead of function as it suggests a **movement**.

**Linear** transformations has two properties:

1. all lines must remain lines without getting curved
2. the origin must remain fixed in place

(can be regarded as keeping grid lines parallel and evenly spaced)

How to represent it numerically? Use basis vector.

The linear combination relationship of vectors keep the same after linear transformation

**input vector = x * (i_hat) + y * (j_hat)**

**Transformed vector = x * (Transformed i_hat) + y * (Transformed j_hat)**

For this kind of 2-dimensional linear transformation, we only need to know the transformed i_hat and j_hat, and apply it to any vector we want to transformed (the input vector) to get the output vector. It meets the idea of **scalar the basis and then adding them**

for general:

a b

c d

in fact it should be regard as combination of two basis which are [a; c] and [b; d]

when apply this matrix to some vector like [x; y], that is, time x to [a; c] and y to [b; d]

![a](D:\git\LittleSkillNotes\math\a.png)



apply the transformation matrix [a b; c d] to the input vector [x;y];



Special case : **Shear** : In this transformation, i_hat keep the same: the first column [1; 0]; j_hat becomes [1; 1];

The important idea: **every time when you see a matrix, regard them as a certain transformation of the space.**



## Matrix multiplication as composition

![b](D:\git\LittleSkillNotes\math\b.png)



So, the multiplication of two matrices can be regarded as applying a series of transformation. 

![b](D:\git\LittleSkillNotes\math\c.png)

as when applying functions, it is from right to left, so there is the same.

![b](D:\git\LittleSkillNotes\math\d.png)

So, the really computation is: finding where i_hat lands; then finding where j_hat lands:

For i_hat, the first one is [e; g]; applying M~2~ to [e; g] which meaning finding the transformation with M~2~ of first version basis [e; g]; 



So, is M~1~M~2~ =M~2~M~1~? **NOT**



To prove the associativity: (AB)C = A(BC) without numerically computing:

for LHS: applying C transformation firstly, then B then A;

for RHS: applying C transformation and B transformation, then A;

They are the same! applying 3 transformations in the same order.



## Three dimensional linear transformations

i_hat; j_hat; k_hat(along z axis)

The same idea as before: regarding a matrix as a transformation of the space.

Applying each basis the second transformation.



## The determinant







