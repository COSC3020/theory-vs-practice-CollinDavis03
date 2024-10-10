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

- The first reason that asymptotic analysis is misleading is that there are different machines in this world and they all run differently. Even if you do a test on one machine and you get the runtime from it, it will still factor out the other machines that are out there and we do not account for the analysis on those machines.
  
- The second reason is that it will look at the complexity with input size growing. This is very useful. It will also leave out information about the time and complexity that we might need to understand.

- The third reason is that it only looks at the impact that it makes on the input size of the complexity.  This could leave out factors that could contribute to the changes in the complexity of the code. While we are looking at the asymptotic complexity we tend to ignore the low order factors.

  Binary Search tree:
  
  Balanced: 
  k = constant
  5 seconds for the 1,000 elements
  k * log(1,000) = 5
  k * 3 = 5
  k = 5/3
  plug that into 10,000
  5/3 * log(10,000) = time 
  5/3 * 4 = time
  20/3 = time
  Takes 20/3 or 6 2/3 seconds to do the binary search tree if we follow the orignial method.
  
  Basic Math: 
  n = amount
  k = constant
  k * 1,000 = 5
  k = 5/1,000
  (5/1000) * 10,0000 = time
  50 seconds = time

  Reasoning why it was not the times we got above:

  - The first reason could be the machine we were using. The original time could have been from a machine that was stronger and faster than the second machine we tested it on. Which made the results worse than we thought they were going to be.
 
  - The second reason is that maybe the person testing this was watching a movie while the test was going. Which could have been using the resources on the computer making the test run slower than we anticipated it to.
 
  - If they were using an older machine the memory could have been old. This would lead the test to not having enough memory to run all the elements that were put into the test causing it to slow down and increase the time that it took to complete the test. 


Sources: 
After doing it the first time I spoke with Nolan and Lily about this to see what I was missing and what I could of over-thought with it. I forgot that I had to do the log stuff for the calculations. I did not explain the reasonings the best because I was thinking in a computer builder mindset and thought you would understand it. I also was on the right track with the complexity of misleading info but was not thinking deeper about the topics I wrote and did that. I also looked at egkallas repo to make sure I had the right calculations and was not messing up the times. 

Plagiarism Statement: 
“I certify that I have listed all sources used to complete this exercise, including the use of any Large Language Models. All of the work is my own, except where stated otherwise. I am aware that plagiarism carries severe penalties and that if plagiarism is suspected, charges may be filed against me without prior notice.”

