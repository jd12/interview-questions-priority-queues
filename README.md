# interview-questions-mergesort

Update this file with your answers. If you write outside files drop them in the repository

1. **Dynamic median.** Design a data type that supports insert in logarithmic time, find-the-median in constant time, and remove-the-median in logarithmic time. If the number of keys in the data type is even, find/remove the lower median.

*Hint: maintain two binary heaps, one that is max-oriented and one that is min-oriented.*

2. **Randomized priority queue.** Describe how to add the methods `sample()` and `delRandom()` to the books [binary heap implementation](https://algs4.cs.princeton.edu/24pq/). The two methods return a key that is chosen uniformly at random among the remaining keys, with the latter method also removing that key. The `sample()` method should take constant time; the `delRandom()` method should take logarithmic time. Do not worry about resizing the underlying array.

*Hint: use `sink()` and `swim()` from [MaxPQ.java](https://algs4.cs.princeton.edu/24pq/MaxPQ.java.html) and [MinPQ.java](https://algs4.cs.princeton.edu/24pq/MinPQ.java.html)*

3. **Taxicab numbers.** A taxicab number is an integer that can be expressed as the sum of two cubes of positive integers in two different ways: 
a<sup>3</sup> + b<sup>3</sup> = c<sup>3</sup> + d<sup>3</sup>. For example, 1729 is the smallest taxicab number: 9<sup>3</sup> + 10<sup>3</sup> = 1<sup>3</sup> + 12<sup>3</sup>. Design an algorithm to find all  taxicab numbers with a, b, c, and d less than n.

- Version 1: Use time proportional to n<sup>2</sup>log n and space proportional to n<sup>2</sup>
- Version 2: Use time proportional to n<sup>2</sup>log n and space proportional to n

*Hint: Version 1: Form the sums of a<sup>3</sup> + b<sup>3</sup> and sort. Version 2: Use a min oriented priority queue with n items*
