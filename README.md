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

- The first reason is that you could have two algorithms that have the exact asymptotic analysis. You would think these two would run at the sametime. That is not necessarily true because a lot of the time one algorithm is going to be a lot more complex than the other algorithm and it will take up a lot more time to run have a longer output time and use up a lot more resources than the first one. In actuality, these two algorithms might have the same asymptotic analysis but might not have the same output time. 

- The second reason is the small input sizes. The asymptotic analysis ignores these small input sizes because these could dominate the times and mess up the constant factors too. 

- The third reason let's say we have an A and B algorithm. Algorithm A has a better worse-case time than algorithm B. You would think to choose algorithm A because the worst-case is better. That would not work because algorithm B has a better average case than A. Which means it performs better than A would. The better worse-case complexity is not always the faster algorithm. You have to look at everything that it has to over for time complexity. 

Answer to elements: 

- To answer the question above, you would treat it as a simple math problem and do 10,000 / 1,000 = 10, and 10 times 5 is 50. You would think that it takes 50 seconds to do a 10,000 element binary search tree with the original one you had. 

The three reasons that the complexity analysis is half of the actual time are the machine that was being used, the complexity of the algorithm, and the size of the algorithm. 

- The machine might not have been as quick and efficient as the complexity analysis that it would do. It would take longer to run and not have as high a performance as needed.

- The complexity of the algorithm could have been designed to deal with a smaller number of elements compared to larger sizes of elements. It could have been pulling more resources than it had and it slowed it down.

- The size of an array or elements can have a factor in it because RAM is usually in charge of uploading and trying to display data as fast and smoothly as possible. The RAM could not have been good enough to deal with that large amount of elements so it slowed down the process. 
