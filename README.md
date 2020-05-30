# blog-Binary-search
Binary search

search space: the domain in which our answer  is surely located.
				The search space is initially the entire sequence. At each step, the algorithm compares the median value in the search space to the target value. Based on the comparison and because the sequence is sorted, it can then eliminate half of the search space. By doing this repeatedly, it will eventually be left with a search space consisting of a single element, the target value and that will lead to our answer.
Finding a value in a sorted sequence:
Let the sequence be:			
values	0	5	13	19	22	41	55	68	72	81	98	
index	0	1	2	3	4	5	6	7	8	9	10	

Let we are seraching for 55
it is sure that it is somewhere between index 0 and 10 , so it is our search space.
Let var l=0 anr r=10 (our search space)
median=(0+10)/2=5,
now check if the median value is 55 greater than 55 or smaller than 55.
if median value is our key(55)
	 than we found our key. We will exit by printing be found the value.
If the median value is smaller than key.
as in our example median is 5 and value at index 5 is 41 than is smaller than our key(55). So we are sure that 55 will not be in range of indeces 0 to 5. is it?.
So now our search space is from index 6 to 10 i.e.
values	55	68	72	81	98
index	6	7	8	9	10
Now, again claculate the median and check the median value.
Median=(6+10)/2=8.
If the median value is greater than key.
as in our example median is 8 and value at index 8 is 72 than is greater than our key(55). So we are sure that 55 will not be in range of indeces 8 to 510 is it?.
So sgain we will reduce our search space
values	55	68
index	6	7

In next step our median value will become (6+7)/2=6.
and value at index 6 is 55 so we found our answer.




Binary search in c++ standard template library:
•	lower_bound,
•	upper_bound,
•	binary_search and equal_range,
	
	it is best to use library function whwnever possible. Implementing binary search on own is can be tricky, we will see it now.

Variants of binary search:

























	






























