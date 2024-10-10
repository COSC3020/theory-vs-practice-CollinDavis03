# Theory vs. Practice

- List 3 reasons why asymptotic analysis may be misleading with respect to
  actual performance in practice.

- Suppose finding a particular element in a binary search tree with 1,000
  elements take 5 seconds. Given what you know about the asymptotic complexity
  of search in a binary search tree, how long would you guess finding the same
  element in a search tree with 10,000 elements takes? Explain your reasoning.

- You measure the time with 10,000 elements and it takes 100 seconds! List 3
  reasons why this could be the case, given that reasoning with the asymptotic
  complexity suggests a different time.

Add your answers to this markdown file.

Reasoning for asymptotic analysis is misleading: 

- The first reason that asymptotic analysis is misleading is that there are different machines in this world, and they all run differently. Even if you do a test on one machine and you get the runtime from it, it will still factor out the runtime on other machines, and we do not account for the analysis on those machines. 
  
- The second reason is that alot of these focus on the growth rate of the algorithm and ignore the constant factors that you might run into. The reason I say that is cause _O_(log n) might have a larger constant value than compared to _O_(n) might have a faster runtime for smaller input sizes. 

- The third reason is that a lot of these complexities do not account for the memory that is being used. The reason being said is that there could be a lot of memory cache misses and not having enough memory within the system. Which will most likely slow down the time than they predicted it to be. 

  Binary Search Tree Time:
  
  -Balanced: 
  -k = constant
  -5 seconds for the 1,000 elements
  -k * log(1,000) = 5
  -k * 3 = 5
  -k = 5/3
  -plug that into 10,000
  -5/3 * log(10,000) = time 
  -5/3 * 4 = time
  -20/3 = time
  -Takes 20/3 or 6 2/3 seconds to do the binary search tree if we follow the orignial method.
  
  -Complexity: 
  -n = amount
  -k = constant
  -k * 1,000 = 5
  -k = 5/1,000
  -(5/1000) * 10,0000 = time
  -50 seconds = time

  Using _O_(log n) (Time complexity) we got 6.666 seconds for the runtime. With the complexity of math, it should have been 50 seconds. 

  Reasoning why it was not the times we got above:

  - The first reason could be the machine used during the test. They could have used a different machine for the second test that was completely different than the first one. If it does not have the same specs as the first one it could possibly run at different times. 
 
  - The second reason is that there is a possibility that the test computer memory or RAM is old and does not have the memory capacity to withstand the amount of numbers that are being put out. This will cause the computer to slow down and have a lower runtime because it is limited on the memory it can use and has to complete it before it can move on to the next bit of info. 
 
  - The third reason is using the same machine for testing (1,000 elements) there is a chance that the tester had some extra source running while the test was running. This would cause the computer to put all of its resources into the program that it is being used because it is important and the test just run on the reserved resources that it has because it is not the priority application being used. 

Sources: 
After doing it the first time I spoke with Nolan and Lily about this to see what I was missing and what I could of over-thought with it. I forgot that I had to do the log stuff for the calculations. I did not explain the reasonings the best because I was thinking in a computer builder mindset and thought you would understand it. I also was on the right track with the complexity of misleading info but was not thinking deeper about the topics I wrote and did that. I also looked at egkallas repo to make sure I had the right calculations and was not messing up the times. 

Plagiarism Statement: 
“I certify that I have listed all sources used to complete this exercise, including the use of any Large Language Models. All of the work is my own, except where stated otherwise. I am aware that plagiarism carries severe penalties and that if plagiarism is suspected, charges may be filed against me without prior notice.”

