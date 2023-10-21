<center>
<h1>COMP4680: Advanced Topics in Machine Learning</h1>
<h2>ASE: Total Variation Denoising</h2>
Semester 2, 2023<br>
</center>

This project involves the investigation of problems in deep declarative networks [Gould et al., 2021]. 
We will specifically be focused on the problem of differentiating the solution of a total variation reconstruction problem [Boyd and Vandenberghe, 2004, §6.3.3]. 
Concretely the total variation problem can be stated as

$$
x^* = \arg\min_x \frac{1}{2}\|Ax - b\|_2^2 + \lambda \|Dx\|_1
$$