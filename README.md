# The Running Time Of Sorting Algorithms On Different Distributions Data Set

Sorting-Algorithm Repository implements most of common used comparison sorts and linear sorts. The repostiory also provides few sample test cases to show the actual running time of the sorting algorithm on different distributions data set.

Sample test includes uniform distribution, normal distribution, gamma distribution, exponential distribution, Poisson distribution, binomial distribution, Bernoulli distribution, 10,000 random float numbers between 0 and 1, ascending integers from 0 to 10,0000, and descending integers from 0 to 10,000. The test sorts 10,000 in each case.

The result suggest that the running time of quicksort is largely depended on the distribution of that data. For those who distribute symmetrically and not or less repeated are much better than those who perform extremely unbalance and contain repeated data. In the case of sorting 10,000 same numbers, the running time of quicksort is close to that of bubble sort. 

In general, the running time of merge sort and insertion sort do better than that of the quick sort. Quicksort appears a large variation. Merge sort with insertion sort in it has the best average running time. RadixSort is very suitable for sorting a small range of floating numbers. 

**Requirements**

C++11

Any version above Python3

Python Packages
1) pandas
2) scipy

**To run the sample test:**
```
$ cd tools/
$ python3 dataGeneator.py arg1(the size of dataset you want to generate)
$ cd -
$ make all
$ ./sorting.exe
```
**Sorting Algorithms:**
* bubble sort
* recursive bubble sort
* bubble sort(inline assembly code)(NOT DONE YET)
* selection sort
* insertion sort
* recursive insertion sort
* merge sort
* merge sort with insertion sort in merge proceduce*
* merge sort with selection sort in merge proceduce*
* heap sort
* quick sort
* randomized quick sort (three median method)*
* counting sort
* radix sort 
* bucket sort  

\* The implementations are based closely on the Introduction To Algorithms implementations described by Thomas H. Cormen, Charles E. Leiserson, Ronald L. Rivest, and Clifford Stein.

\* A modification to merge sort in which n=k sublists of length k are sorted using selection/insertion sort and then merged
using the standard merging mechanism, where k is a value to be determined. Here, I choose k.

\* The median-of-3 method: choose the pivot as the median (middle element) of a set of 3 elements randomly selected
from the subarray.

\* Detailed information and the math behind are in description.pdf

**Future Work:**
* datasetGeneator.py:
* make the size of data changeable.

* interactive.py:
* Prompt the user to selete sorting algorithms
* Make some tables and graphs:
1) Matplotlib, numpy, and other python packages (on A-N)
2) Gnuplot (on Terminal)
* Generate a running report in Excel

**Acknowledgement**

This work was supported in part by [Liting Huang](https://github.com/llliting).

Modified Sorting Algorithms are based on Cormen, T. (2009). Introduction to algorithms (3rd ed.) [3rd ed.]. Cambridge, Mass.: MIT Press. (2009). Retrieved October 12, 2019, from Franklin and Marshall College Online Library.
