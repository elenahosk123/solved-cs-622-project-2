Download Link: https://assignmentchef.com/product/solved-cs-622-project-2
<br>






<strong>Logistics: </strong>You must implement everything stated in this project description that is marked with an <strong>implement </strong>tag. Whenever you see the <strong>write-up </strong>tag, that is something that must be addressed in the project README.txt. Graduate students are required to implement everything including items tagged with <strong>622</strong>. Students in 422 do not need to complete these extra elements. <strong>You cannot import any packages unless specifically noted by the instructor. </strong>In this project, you may import the numpy and math packages. You are welcome to ask about particular packages as they come up. The idea is to implement everything from scratch.




<h1>1           Perceptron (50 points)</h1>

<strong>File name: perceptron.py</strong>

<strong>Implement </strong>a function in python:

perceptron_train(X,Y)

that takes training data as input and outputs the weights w, and the bias b of the perceptron. Your function should handle any real-valued features, with feature vectors in any dimension, and binary labels. <strong>Write-Up</strong>: describe your implementation concisely.

<strong>Implement </strong>a function in python:

perceptron_test(X_test, Y_test, w, b)

that takes testing data, the perceptron weights and bias as input and returns the accuracy on the testing data. <strong>Write-Up</strong>: describe your implementation concisely.

You should get the following output for the perceptron when you run the test script.

<table width="576">

 <tbody>

  <tr>

   <td width="97">Perceptron :</td>

   <td width="479">1.0</td>

  </tr>

  <tr>

   <td width="97">Perceptron :</td>

   <td width="479">0.42857142857142855</td>

  </tr>

 </tbody>

</table>

1

2

<h1>2           Gradient Descent (50 points)</h1>

<strong>Implement </strong>a function in python: <em>gradient descent</em>(∇<em>f,x<sub>init</sub>,η</em>) that takes the gradient of a function <em>f </em>as input, the starting <em>x<sub>init </sub></em>and the learning rate <em>η</em>. The output of <em>gradient descent </em>is the value of <strong>x </strong>that minimizes ∇<em>f</em>. ∇<em>f </em>will be in the form of a function, so that you can calculate the gradient at a particular point. That is ∇<em>f </em>is a function with one input <strong>x </strong>and it outputs the value of the gradient at that point. If we are working with 1D variables, then <strong>x</strong>= (<em>x</em><sub>1</sub>). If <strong>x </strong>is 2D then <strong>x</strong>= (<em>x</em><sub>1</sub><em>,x</em><sub>2</sub>) and so on. <strong>x </strong>should be a 1D numpy array. <strong>Write-Up</strong>: describe your implementation concisely.

If you test your function using <em>f</em>(<em>x</em>) = <em>x</em><sup>2</sup>, <em>x<sub>init </sub></em>= 5, and <em>η </em>= 0<em>.</em>1. ∇<em>f </em>= 2<em>x</em>. You should get a final x of 4<em>.</em>56719262<em>e </em>− 05 or something very small like that. It should take 52 steps. Note, I am not checking for

1

gradient equal to 0. I am checking that the magnitude of the gradient is less than some very small value,

0<em>.</em>0001.

For testing purposes: I will test your program with various ∇<em>f</em>.

You should get the following output for the gradient descent when you run the test script.

<table width="576">

 <tbody>

  <tr>

   <td width="145">Gradient Descent :</td>

   <td width="431">[4.56719262e−05]</td>

  </tr>

  <tr>

   <td width="145">Gradient Descent :</td>

   <td width="431">[2.16433186e−55 5.77016976e−03]</td>

  </tr>

 </tbody>

</table>

1

2

2