## Description

<div><p>Today on a lecture about strings Gerald learned a new definition of string equivalency. Two strings <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> of equal length are called <span class="tex-font-style-it">equivalent</span> in one of the two cases: </p><ol> <li> They are equal. </li><li> If we split string <span class="tex-span"><i>a</i></span> into two halves of the same size <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, and string <span class="tex-span"><i>b</i></span> into two halves of the same size <span class="tex-span"><i>b</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index">2</sub></span>, then one of the following is correct: <ol> <li> <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span> is equivalent to <span class="tex-span"><i>b</i><sub class="lower-index">1</sub></span>, and <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span> is equivalent to <span class="tex-span"><i>b</i><sub class="lower-index">2</sub></span> </li><li> <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span> is equivalent to <span class="tex-span"><i>b</i><sub class="lower-index">2</sub></span>, and <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span> is equivalent to <span class="tex-span"><i>b</i><sub class="lower-index">1</sub></span> </li></ol> </li></ol><p>As a home task, the teacher gave two strings to his students and asked to determine if they are equivalent.</p><p>Gerald has already completed this home task. Now it's your turn!</p></div><div class="input-specification"><p>The first two lines of the input contain two strings given by the teacher. Each of them has the length from <span class="tex-span">1</span> to <span class="tex-span">200 000</span> and consists of lowercase English letters. The strings have the same length.</p></div><div class="output-specification"><p>Print "<span class="tex-font-style-tt">YES</span>" (without the quotes), if these two strings are equivalent, and "<span class="tex-font-style-tt">NO</span>" (without the quotes) otherwise.</p></div>

## Input

<p>The first two lines of the input contain two strings given by the teacher. Each of them has the length from <span class="tex-span">1</span> to <span class="tex-span">200 000</span> and consists of lowercase English letters. The strings have the same length.</p>

## Output

<p>Print "<span class="tex-font-style-tt">YES</span>" (without the quotes), if these two strings are equivalent, and "<span class="tex-font-style-tt">NO</span>" (without the quotes) otherwise.</p>





```input1
aaba
abaa

```




```input2
aabb
abab

```




```output1
YES

```




```output2
NO

```



## Note

<p>In the first sample you should split the first string into strings "<span class="tex-font-style-tt">aa</span>" and "<span class="tex-font-style-tt">ba</span>", the second one — into strings "<span class="tex-font-style-tt">ab</span>" and "<span class="tex-font-style-tt">aa</span>". "<span class="tex-font-style-tt">aa</span>" is equivalent to "<span class="tex-font-style-tt">aa</span>"; "<span class="tex-font-style-tt">ab</span>" is equivalent to "<span class="tex-font-style-tt">ba</span>" as "<span class="tex-font-style-tt">ab</span>" = "<span class="tex-font-style-tt">a</span>" + "<span class="tex-font-style-tt">b</span>", "<span class="tex-font-style-tt">ba</span>" = "<span class="tex-font-style-tt">b</span>" + "<span class="tex-font-style-tt">a</span>".</p><p>In the second sample the first string can be splitted into strings "<span class="tex-font-style-tt">aa</span>" and "<span class="tex-font-style-tt">bb</span>", that are equivalent only to themselves. That's why string "<span class="tex-font-style-tt">aabb</span>" is equivalent only to itself and to string "<span class="tex-font-style-tt">bbaa</span>".</p>
