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

Ahmed designs solar panels as a hobby.
On April 1st, Ahmed's "Mark I" design begins generating power: 1 KJ/day.
On May 1st, his "Mark II" design begins generating 4 KJ of power per day.

1. What day is it when Ahmed's Mark II design has generated as much total energy as the Mark I design?
2. How much total energy have both generated by that day?
3. What would the solutions to (1.) and (2.) be if Mark II design generated 1KJ of power per day?


<p align="center", font-weight: "bold">Solution</p>

<p align="center">Equation 1: <em>w</em> = <em>t</em>, (where: w for work, t for time, p(slope=1) for power)</p>
<p align="center">Equation 2: <em>w</em> = 4(<em>t</em>-30)</p>

<p align="center"><em>t</em> = 4(<em>t</em>-30)</p>
<p align="center"><em>t</em> = 4<em>t</em>-120</p>
<p align="center"><em>t</em> - 4<em>t</em> = -120</p>
<p align="center">-3<em>t</em> = -120</p>
<p align="center"><em>t</em> = -120/-3 = 40 min</p>
<p align="center"><em>w</em> = <em>t</em> = 40 J</p>
<p align="center"><em>w</em> = 4(<em>t</em> - 30) = 4(40 - 30) = 4(10) = 40 J</p>
