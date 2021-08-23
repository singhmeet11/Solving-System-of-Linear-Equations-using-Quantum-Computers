# Solving-System-of-Linear-Equations-using-Quantum-Computers

Linear equations can be found in almost all fields. As the size of data which defines the equation set is increasing at an exponential rate, classical computers are getting overwhelmed. For N linear equations with N unknown variables the best classical algorithms(conjugate gradient method) have a complexity of the form $O(Nk)$ where $k$ is the condition number of the matrix(it shows how far the image is from being inverted).  \\
The Quantum Algorithm that we discuss will be able to solve the given equations in $poly(log N, k)$ , which is an exponential speed up over the classical algorithms.
The problem of N linear equations can be expressed by using  matrix representation,

<a href="https://www.codecogs.com/eqnedit.php?latex=\begin{equation}&space;\begin{bmatrix}&space;A_{11}&space;&&space;A_{12}&space;&&space;...&&space;...\\&space;A_{21}&space;&&space;...&&space;\\&space;...&space;&&space;&\\&space;A_{N1}&space;&&space;A_{N2}&space;&...&space;&A_{NN}&space;\end{bmatrix}&space;\begin{bmatrix}&space;x_{1}&space;\\&space;..&space;&\\&space;\\&space;x_{N}&space;\end{bmatrix}&space;=&space;\begin{bmatrix}&space;b_{1}&space;\\&space;..\\&space;\\&space;b_{N}&space;\end{bmatrix}&space;\end{equation}" target="_blank"><img src="https://latex.codecogs.com/gif.latex?\begin{equation}&space;\begin{bmatrix}&space;A_{11}&space;&&space;A_{12}&space;&&space;...&&space;...\\&space;A_{21}&space;&&space;...&&space;\\&space;...&space;&&space;&\\&space;A_{N1}&space;&&space;A_{N2}&space;&...&space;&A_{NN}&space;\end{bmatrix}&space;\begin{bmatrix}&space;x_{1}&space;\\&space;..&space;&\\&space;\\&space;x_{N}&space;\end{bmatrix}&space;=&space;\begin{bmatrix}&space;b_{1}&space;\\&space;..\\&space;\\&space;b_{N}&space;\end{bmatrix}&space;\end{equation}" title="\begin{equation} \begin{bmatrix} A_{11} & A_{12} & ...& ...\\ A_{21} & ...& \\ ... & &\\ A_{N1} & A_{N2} &... &A_{NN} \end{bmatrix} \begin{bmatrix} x_{1} \\ .. &\\ \\ x_{N} \end{bmatrix} = \begin{bmatrix} b_{1} \\ ..\\ \\ b_{N} \end{bmatrix} \end{equation}" /></a>

or 

<a href="https://www.codecogs.com/eqnedit.php?latex=\begin{equation}&space;A\vec{x}&space;=&space;\vec{b}&space;\end{equation}" target="_blank"><img src="https://latex.codecogs.com/gif.latex?\begin{equation}&space;A\vec{x}&space;=&space;\vec{b}&space;\end{equation}" title="\begin{equation} A\vec{x} = \vec{b} \end{equation}" /></a>

The above equation can be solved by multiplying both the sides with $A^{-1}$ which provides us with the solution vector which is given by $\vec{x}$ .

<a href="https://www.codecogs.com/eqnedit.php?latex=\begin{equation}&space;\vec{x}&space;=&space;A^{-1}\vec{b}&space;\end{equation}" target="_blank"><img src="https://latex.codecogs.com/gif.latex?\begin{equation}&space;\vec{x}&space;=&space;A^{-1}\vec{b}&space;\end{equation}" title="\begin{equation} \vec{x} = A^{-1}\vec{b} \end{equation}" /></a>

we aim to use this in order to solve our system of linear equations.

For a more detailed look into the project look into the pdf and you can also take a look at our preseantation here - https://docs.google.com/presentation/d/19uko5Az0RzpE3irMWIIv89JcvvqazJwXc6ozBz7XtVk/edit?usp=sharing
