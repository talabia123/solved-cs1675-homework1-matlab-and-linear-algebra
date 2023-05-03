Download Link: https://assignmentchef.com/product/solved-cs1675-homework1-matlab-and-linear-algebra
<br>
<u>Part I: Matlab and linear algebra</u>

Write your code in a script called <span style="font-family: courier new;">hw1.m</span>, except where noted. Each item is worth 3 points.

Since one optimization that Matlab uses is to vectorize code rather than use loops, pay close attention to whether you are allowed to use loops. If this is not specified, you can (but don’t have to) use loops. Remember to use the Matlab documentation whenever needed.

Basic operations:

<ol>

 <li>Generate a 1000000×1 (one million by one) vector of random numbers from a Gaussian (normal) distribution with mean of 0 and standard deviation of 5. Use Matlab’s <span style="font-family: Courier New;">randn</span> function.</li>

 <li>Add 1 to every value in the previous list, by using a loop. To determine how many times to loop, use Matlab’s <span style="font-family: Courier New;">size</span> function. Time this operation and print the number in the code. (Use Matlab’s documentation to find out how to time operations.)</li>

 <li>Now add 1 to every value in the original random vector, without using a loop. Time this operation, print the time and write it down. Use a different way to print the number than the method you used above. (See ways to print numbers at the beginning of the Matlab tutorial script.)</li>

 <li>Plot the exponential function <span style="font-family: courier new;">2.^x</span>, for non-negative <i>even</i> values of x smaller than 100, without using loops.</li>

 <li>[4 pts] Create two matrices <span style="font-family: courier new;">A</span> and <span style="font-family: courier new;">B</span> which, when added together, result in a 10×10 matrix <span style="font-family: courier new;">C</span> containing all numbers from 1 to 100. In other words, when I add <span style="font-family: courier new;">A</span> and <span style="font-family: courier new;">B</span> and convert the result to vector form, I should get a vector containing all numbers from 1 to 100. In code, <span style="font-family: courier new;">C = A + B; assert(all(C(:) == (1:100)’) == 1);</span> Each matrix should only be created with a single command (no loops).</li>

</ol>

Linear algebra:

<ol start="6">

 <li>Generate two random matrices <span style="font-family: Courier New;">A</span> and <span style="font-family: Courier New;">B</span>, and compute their product by hand, using loops. The size of the first matrix should be [5, 3] and of the second [3, 5]. Check your code by comparing the loop-computed product with the product that you get from Matlab’s <span style="font-family: Courier New;">A*B</span>. You can use loops.</li>

 <li>Show three ways to compute an inner product between two vectors.</li>

 <li>Compute and print the L1-norm and L2-norm for each of the following two vectors: x1 = [0.5 0 1.5] and x2 = [1 1 0]. Verify your answer against the Matlab function <span style="font-family: courier new;">norm</span>.</li>

 <li>Use Matlab to solve the system of linear equations: 2x + y + 3z = 1; 2x + 6y + 8z = 3; 6x + 8y + 18z = 5.</li>

</ol>

Functions:

<ol start="10">

 <li>Write a function <span style="font-family: courier new;">function [B] = normalize_rows(A)</span> which uses a single command (one line and no loops) to make the sum in each row of the matrix 1. You may need to use <span style="font-family: Courier New;">repmat</span>, depending on your Matlab version. Note that the sum of the entries in <i>each</i> row should be 1, in the matrix output by your function.</li>

 <li>Create a function <span style="font-family: courier new;">function [val] = fib(n)</span> that returns the n-th number (n &gt;= 1) in the Fibonacci sequence 1, 1, 2, 3, 5, 8, 13…</li>

</ol>

Machine learning setup:

<ol start="12">

 <li>We have the following training set: a red circle, a blue triangle, a blue circle, a green triangle, and a red square. Represent each of these samples as a feature vector, using the same representation scheme/strategy. Write a comment to explain the meaning of each dimension in your representation, i.e. what feature it corresponds to, and what the possible values of that feature are.</li>

</ol>

<u>Part II: Short answers</u> (4 pts)

In a file <span style="font-family: courier new;">answers.txt</span>, propose two new problems that can be solved with machine learning (ones that we have not discussed in class), and describe how you would go about solving each. For each problem, discuss:

<ul>

 <li>What features (x) would you use?</li>

 <li>What would the labels (y) be?</li>

 <li>How would you collect data?</li>

 <li>Why might the problem turn out to be challenging?</li>

</ul>