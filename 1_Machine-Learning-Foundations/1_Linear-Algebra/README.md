<h1 align="center", font-weight: "bold">Linear Algebra</h1>

> - **Linear Algebra** lies at the heart of most *machine learning* approaches and is especially predominant in *deep learning*, the branch of ML at the forefront of today’s *artificial intelligence* advances. 
> * **Linear Algebra** is used to solve for ***unknown values*** in ***high-dimensional spaces***, thereby enabling machines to ***recognize patterns*** and ***make predictions***. 


---------------------------------------------------------------------------------

<h2 align="left", font-weight: "bold">- What Algebra is?</h2>

**'Algebra'** is arithmetic that includes non-numerical entities like *x*, e.g.: 
<p align="center">2<em>x</em> + 5 = 25, then we have determined <strong><em>x</em> must equal 10</strong> because 2(<strong>10</strong>) + 5 = 25</p>

> If it has an exponential term, it isn't linear algebra, e.g.: 2*x*<sup>2</sup> + 5 = 25

---------------------------------------------------------------------------------

<h2 align="left", font-weight: "bold">- What Linear Algebra is?</h2>
<p align="center"><strong>"Solving for unknowns within system of linear equations"</strong></p>

Consider the following example:
+ Ahmed has 180 km/h car.
+ Belal has 150 km/h car and five-minute head start.
+ How long does it take the ahmed to meet the belal?
+ What distance will they have traveled at the point?
+ (For simplicity, let's ignore acceleration, traffic, etc.)

> <p>Problem can be solved <strong><em>graphically</em></strong> with a plot:</p>
![SolvingGraphically](https://user-images.githubusercontent.com/90105797/221732059-47563ce8-86df-406f-b7bf-902f26d95c3f.png)

See: [Appendix-I: Plotting a System of Linear Equations Notebook](https://github.com/omarmamdouhismaiel/Data-Science-Theory/blob/d0895fa3f1e0e4435b6d9649b1f3da6e601c0b6d/Linear-Algebra/Appendix-I_Plotting-a-System-of-Linear-Equations.ipynb)
ـــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــ

> <p>Alternatively, problem can be solved <strong><em>algebraically</em></strong>:
<p align="center">Equation 1: <em>d</em> = 2.5<em>t</em></p>
<p align="center">Equation 2: <em>d</em> = 3(<em>t</em>-5)</p>

<p align="center">2.5<em>t</em> = 3(<em>t</em>-5)</p>
<p align="center">2.5<em>t</em> = 3<em>t</em>-15</p>
<p align="center">2.5<em>t</em> - 3<em>t</em> = -15</p>
<p align="center">-0.5<em>t</em> = -15</p>
<p align="center"><em>t</em> = -15/-0.5 = 30 min</p>
<p align="center"><em>d</em> = 2.5<em>t</em> = 2.5(30) = 75 km</p>
<p align="center"><em>d</em> = 3(<em>t</em> - 5) = 3(30 - 5) = 3(25) = 75 km</p>

<h2 align="left", font-weight: "bold">- Algebraic Solutions:</h2>

![nosolution](https://user-images.githubusercontent.com/90105797/221915601-2da24ccf-c35d-4898-84cf-680f0a934fbe.png)
<p><strong>No solution</strong> if ahmed's car is same speed as belal's.</p>

ـــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــ

![infinitesolutions](https://user-images.githubusercontent.com/90105797/221915549-b0ef13db-b5ee-44e3-83c2-61b3acf7dc25.png)
<p><strong>Infinite solutions</strong> if same speed and same starting point.</p>


> <p><em>These are the only three options in linear algebra</em>: one, no, or infinite solutions.</p>
> <p><strong>It is impossible for lines to cross multiple times.</strong></p>

ـــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــ

<h4 align="left">In a given system of equations:</h4>

- <p>Could be <em>many</em> equations.</p>
- <p>Could be <em>many</em> unknowns in each equation.</p>


<p align="left", font-weight: "bold">As in <strong>Regression Models</strong>:</p>
<p align="center", font-weight: "bold"><strong><em>y</em> = a + b <em>x<sub>1</sub></em> + c <em>x<sub>2</sub></em> + ... + n <em>x<sub>n</sub></em></strong> (where a = y-intercept, and <em>x<sub>1:n</sub></em> = model's features/inputs)</p>
<p align="center", font-weight: "bold">For any house <em>i(=[1:m])</em> in the dataset (has m examples), y<sub>i</sub> = price and x<sub>i,1</sub> to x<sub>i,n</sub> are its features. We solve for parameters <strong>a</strong>, <strong>b</strong>, <strong>c</strong> to <strong>n</strong>.</p>

![RegressionModelMatrixRepresentation](https://user-images.githubusercontent.com/90105797/222003367-06acbe1d-7ffe-4201-a160-26a2f36cfbc2.png)

---------------------------------------------------------------------------------

<h2 align="left", font-weight: "bold">Linear Algebra Applications:</h2>

- <p><strong>Solving for unknowns in ML algos, including deep learning</strong></p>
- <p><strong>Reducing dimensionality (e.g., principal component analysis)</strong></p>
- <p><strong>Ranking results (e.g., with eigenvector)</strong></p>
- <p><strong>Recommenders (e.g., singular value decomposition, SVD)</strong></p>
- <p><strong>Natural language processing (e.g., SVD, matrix factorization)</strong></p>

  - <p><strong>Topic modeling</strong></p>
  - <p><strong>Semantic Analysis</strong></p>

---------------------------------------------------------------------------------

<h2 align="left", font-weight: "bold">Linear Algebra Exercise:</h2>

<p align="left", font-weight: "bold">Ahmed designs solar panels as a hobby.</p>
<p align="left", font-weight: "bold">On April 1st, Ahmed's "Mark I" design begins generating power: 1 KJ/day.</p>
<p align="left", font-weight: "bold">On May 1st, his "Mark II" design begins generating 4 KJ of power per day.</p><br />
<p align="left", font-weight: "bold">1. What day is it when Ahmed's Mark II design has generated as much total energy as the Mark I design?</p>
<p align="left", font-weight: "bold">2. How much total energy have both generated by that day?</p>
<p align="left", font-weight: "bold">3. What would the solutions to (1.) and (2.) be if Mark II design generated 1KJ of power per day?<br /></p>
<br />
<p align="center">Equation 1: <em>w</em> = <em>t</em></p>
<p align="center">Equation 2: <em>w</em> = 4(<em>t</em>-30)</p><br />
<p align="center"><em>t</em> = 4(<em>t</em>-30)</p>
<p align="center"><em>t</em> = 4<em>t</em>-120</p>
<p align="center"><em>t</em> - 4<em>t</em> = -120</p>
<p align="center">-3<em>t</em> = -120</p>
<p align="center"><em>t</em> = -120/-3 = 40 min</p>
<p align="center"><em>w</em> = <em>t</em> = 40 J</p>
<p align="center"><em>w</em> = 4(<em>t</em> - 30) = 4(40 - 30) = 4(10) = 40 J</p>
<h4 align="left", font-weight: "bold">Solutions:</h4>
<p align="left", font-weight: "bold">1. 40 days from April 1st, which is May 10th</p>
<p align="left", font-weight: "bold">2. 40 KJ generated by each design for a total of 80 KJ</p>
<p align="left", font-weight: "bold">3. No solutions, where {equation 1: <em>w</em> = <em>t</em>, and equation 2: <em>w</em> = <em>t</em>-30}<br /></p>
<br />

---------------------------------------------------------------------------------

<h2 align="left", font-weight: "bold">Solving Linear Systems:</h2>

<h3 align="left", font-weight: "bold"> Method 1:Substitution</h3>

+ Use whenever there's a variable in system with coefficient of 1

For example, when solving for *x* and *y* in the following system:
<p align="center"><em>y</em> = 3<em>x</em></p>
<p align="center">-5<em>x</em> + 2<em>y</em> = 2</p>
...we can substitute <em>y</em> with 3<em>x</em> in the second equation.
<br \>
<br \>
<p align="center", font-weight: "bold"><strong>Solution</strong></p>
<p align="center">System of Equations = { <strong>1st-eq</strong>: <em>y</em> = 3<em>x</em>, <strong>2st-eq</strong>: -5<em>x</em> + 2<em>y</em> = 2 }</p>
<p align="center">-5<em>x</em> + 2<em>y</em> = 2,  substitute with <strong>1st-eq</strong> in <strong>2st-eq</strong></p>
<p align="center">-5<em>x</em> + 2<em>(3<em>x</em>)</em> = 2</p>
<p align="center">-5<em>x</em> + 6<em>x</em> = 2</p>
<p align="center"><em>x</em> = 2</p>
<p align="center"><em>y</em> = 3<em>x</em>,  substitute with (<em>x</em>=2) in <strong>1st-eq</strong></p>
<p align="center"><em>y</em> = 3(2)</p>
<p align="center"><em>y</em> = 6</p>
<p align="center">∴ (<em>x</em>, <em>y</em>) = (2, 6)</p>
ـــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــــ

<h3 align="left", font-weight: "bold"> Method 2:Elimination</h3>

+ Typically best option if no variable in system has coefficient of 1
+ Use *addition property* of equations to eliminate variables
  + If necessary, multiply one or both equations to make elimination of a variable possible

For example, solve for the unknowns in the following system:
<p align="center">2<em>x</em> - 3<em>y</em> = 15</p>
<p align="center">4<em>x</em> + 10<em>y</em> = 14</p>
...by multiplying the first equation by -2 and adding the equations.
<br \>
<br \>
<p align="center", font-weight: "bold"><strong>Solution</strong></p>
<p align="center">System of Equations = { <strong>1st-eq</strong>: 2<em>x</em> - 3<em>y</em> = 15, <strong>2st-eq</strong>: 4<em>x</em> + 10<em>y</em> = 14 }</p>
<p align="center">-4<em>x</em> + 6<em>y</em> = -30,  multiply <strong>1st-eq</strong> by -2</p>
<p align="center">4<em>x</em> + 10<em>y</em> = 14,  add to <strong>2st-eq</strong></p>
<p align="center">16<em>y</em> = -16,  divide by 16</p>
<p align="center"><em>y</em> = -1</p>
<p align="center">2<em>x</em> - 3<em>y</em> = 15,  substitute with (<em>y</em>=-1) in <strong>1st-eq</strong></p>
<p align="center">2<em>x</em> - 3(-1) = 15</p>
<p align="center">2<em>x</em> + 3 = 15</p>
<p align="center">2<em>x</em> = 12</p>
<p align="center"><em>x</em> = 6</p>
<p align="center">∴ (<em>x</em>, <em>y</em>) = (6, -1)</p>

See: [Appendix-II: Linear Systems Visualization Notebook](https://github.com/omarmamdouhismaiel/Data-Science-Theory/blob/d25f10ca1f5bab8c7d4a2b8ea56fe2b01d01be5c/Linear-Algebra/Appendix-II_Linear-Systems-Visualization.ipynb)

---------------------------------------------------------------------------------
> <h2 align="center"> So, Let's dive into <strong><strong>"Computational Linear Algebra"</strong></strong> with <strong><em>theory-behind</em><strong> explanation.</h2>
  1. Introductory Linear Algebra.
  2. Affine Transformations.
  3. Matrix Operations for ML.
 ---------------------------------------------------------------------------------
