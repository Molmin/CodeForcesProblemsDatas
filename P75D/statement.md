## Description

<div><p>Ahmed and Mostafa used to compete together in many programming contests for several years. Their coach Fegla asked them to solve one challenging problem, of course Ahmed was able to solve it but Mostafa couldn't.</p><p>This problem is similar to a standard problem but it has a different format and constraints.</p><p>In the standard problem you are given an array of integers, and you have to find one or more consecutive elements in this array where their sum is the maximum possible sum.</p><p>But in this problem you are given <span class="tex-span"><i>n</i></span> small arrays, and you will create one big array from the concatenation of one or more instances of the small arrays (each small array could occur more than once). The big array will be given as an array of indexes (1-based) of the small arrays, and the concatenation should be done in the same order as in this array. Then you should apply the standard problem mentioned above on the resulting big array.</p><p>For example let's suppose that the small arrays are {1, 6, -2}, {3, 3} and {-5, 1}. And the indexes in the big array are {2, 3, 1, 3}. So the actual values in the big array after formatting it as concatenation of the small arrays will be {3, 3, -5, 1, 1, 6, -2, -5, 1}. In this example the maximum sum is 9.</p><p>Can you help Mostafa solve this problem?</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>n</i></span> is the number of the small arrays (<span class="tex-span">1 ≤ <i>n</i> ≤ 50</span>), and <span class="tex-span"><i>m</i></span> is the number of indexes in the big array (<span class="tex-span">1 ≤ <i>m</i> ≤ 250000</span>). Then follow <span class="tex-span"><i>n</i></span> lines, the <span class="tex-span"><i>i</i></span>-th line starts with one integer <span class="tex-span"><i>l</i></span> which is the size of the <span class="tex-span"><i>i</i></span>-th array (<span class="tex-span">1 ≤ <i>l</i> ≤ 5000</span>), followed by <span class="tex-span"><i>l</i></span> integers each one will be greater than or equal -1000 and less than or equal 1000. The last line contains <span class="tex-span"><i>m</i></span> integers which are the indexes in the big array, and you should concatenate the small arrays in the same order, and each index will be greater than or equal to 1 and less than or equal to <span class="tex-span"><i>n</i></span>.</p><p>The small arrays are numbered from 1 to <span class="tex-span"><i>n</i></span> in the same order as given in the input. Some of the given small arrays may not be used in big array.</p><p>Note, that the array is very big. So if you try to build it straightforwardly, you will probably get time or/and memory limit exceeded.</p></div><div class="output-specification"><p>Print one line containing the maximum sum in the big array after formatting it as described above. You must choose at least one element for the sum, i. e. it cannot be empty.</p><p>Please, do not use <span class="tex-font-style-tt">%lld</span> specificator to write 64-bit integers in C++. It is preferred to use <span class="tex-font-style-tt">cout</span> (also you may use <span class="tex-font-style-tt">%I64d</span>).</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>n</i></span> is the number of the small arrays (<span class="tex-span">1 ≤ <i>n</i> ≤ 50</span>), and <span class="tex-span"><i>m</i></span> is the number of indexes in the big array (<span class="tex-span">1 ≤ <i>m</i> ≤ 250000</span>). Then follow <span class="tex-span"><i>n</i></span> lines, the <span class="tex-span"><i>i</i></span>-th line starts with one integer <span class="tex-span"><i>l</i></span> which is the size of the <span class="tex-span"><i>i</i></span>-th array (<span class="tex-span">1 ≤ <i>l</i> ≤ 5000</span>), followed by <span class="tex-span"><i>l</i></span> integers each one will be greater than or equal -1000 and less than or equal 1000. The last line contains <span class="tex-span"><i>m</i></span> integers which are the indexes in the big array, and you should concatenate the small arrays in the same order, and each index will be greater than or equal to 1 and less than or equal to <span class="tex-span"><i>n</i></span>.</p><p>The small arrays are numbered from 1 to <span class="tex-span"><i>n</i></span> in the same order as given in the input. Some of the given small arrays may not be used in big array.</p><p>Note, that the array is very big. So if you try to build it straightforwardly, you will probably get time or/and memory limit exceeded.</p>

## Output

<p>Print one line containing the maximum sum in the big array after formatting it as described above. You must choose at least one element for the sum, i. e. it cannot be empty.</p><p>Please, do not use <span class="tex-font-style-tt">%lld</span> specificator to write 64-bit integers in C++. It is preferred to use <span class="tex-font-style-tt">cout</span> (also you may use <span class="tex-font-style-tt">%I64d</span>).</p>





```input1
3 4
3 1 6 -2
2 3 3
2 -5 1
2 3 1 3

```




```input2
6 1
4 0 8 -3 -10
8 3 -2 -5 10 8 -9 -5 -4
1 0
1 -3
3 -8 5 6
2 9 6
1

```




```output1
9

```




```output2
8

```


