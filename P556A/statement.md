## Description

<div><p>Andrewid the Android is a galaxy-famous detective. In his free time he likes to think about strings containing zeros and ones.</p><p>Once he thought about a string of length <span class="tex-span"><i>n</i></span> consisting of zeroes and ones. Consider the following operation: we choose any two <span class="tex-font-style-it">adjacent</span> positions in the string, and if one them contains 0, and the other contains 1, then we are allowed to remove these two digits from the string, obtaining a string of length <span class="tex-span"><i>n</i> - 2</span> as a result.</p><p>Now Andreid thinks about what is the minimum length of the string that can remain after applying the described operation several times (possibly, zero)? Help him to calculate this number.</p></div><div class="input-specification"><p>First line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>), the length of the string that Andreid has.</p><p>The second line contains the string of length <span class="tex-span"><i>n</i></span> consisting only from zeros and ones.</p></div><div class="output-specification"><p>Output the minimum length of the string that may remain after applying the described operations several times.</p></div>

## Input

<p>First line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>), the length of the string that Andreid has.</p><p>The second line contains the string of length <span class="tex-span"><i>n</i></span> consisting only from zeros and ones.</p>

## Output

<p>Output the minimum length of the string that may remain after applying the described operations several times.</p>





```input1
4
1100

```




```input2
5
01010

```




```input3
8
11101111

```




```output1
0

```




```output2
1

```




```output3
6

```



## Note

<p>In the first sample test it is possible to change the string like the following: <img align="middle" class="tex-formula" src="file://kSqA5pnJ.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>In the second sample test it is possible to change the string like the following: <img align="middle" class="tex-formula" src="file://ExkPOhFn.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>In the third sample test it is possible to change the string like the following: <img align="middle" class="tex-formula" src="file://8sNrv4YN.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>
