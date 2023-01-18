## Description

<div><p>The police department of your city has just started its journey. Initially, they don’t have any manpower. So, they started hiring new recruits in groups.</p><p>Meanwhile, crimes keeps occurring within the city. One member of the police force can investigate only one crime during his/her lifetime.</p><p>If there is no police officer free (isn't busy with crime) during the occurrence of a crime, it will go untreated.</p><p>Given the chronological order of crime occurrences and recruit hirings, find the number of crimes which will go untreated.</p></div><div class="input-specification"><p>The first line of input will contain an integer <span class="tex-span"><i>n</i>&nbsp;(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span>, the number of events. The next line will contain <span class="tex-span"><i>n</i></span> space-separated integers.</p><p>If the integer is -1 then it means a crime has occurred. Otherwise, the integer will be positive, the number of officers recruited together at that time. No more than 10 officers will be recruited at a time.</p></div><div class="output-specification"><p>Print a single integer, the number of crimes which will go untreated.</p></div>

## Input

<p>The first line of input will contain an integer <span class="tex-span"><i>n</i>&nbsp;(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span>, the number of events. The next line will contain <span class="tex-span"><i>n</i></span> space-separated integers.</p><p>If the integer is -1 then it means a crime has occurred. Otherwise, the integer will be positive, the number of officers recruited together at that time. No more than 10 officers will be recruited at a time.</p>

## Output

<p>Print a single integer, the number of crimes which will go untreated.</p>





```input1
3
-1 -1 1

```




```input2
8
1 -1 1 -1 -1 1 1 1

```




```input3
11
-1 -1 2 -1 -1 -1 -1 -1 -1 -1 -1

```




```output1
2

```




```output2
1

```




```output3
8

```



## Note

<p>Lets consider the second example:</p><ol> <li> Firstly one person is hired. </li><li> Then crime appears, the last hired person will investigate this crime. </li><li> One more person is hired. </li><li> One more crime appears, the last hired person will investigate this crime. </li><li> Crime appears. There is no free policeman at the time, so this crime will go untreated. </li><li> One more person is hired. </li><li> One more person is hired. </li><li> One more person is hired. </li></ol><p>The answer is one, as one crime (on step 5) will go untreated.</p>
