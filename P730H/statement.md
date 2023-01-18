## Description

<div><p>Polycarp is a beginner programmer. He is studying how to use a command line.</p><p>Polycarp faced the following problem. There are <span class="tex-span"><i>n</i></span> files in a directory and he needs to delete some of them. Polycarp wants to run a single delete command with filename pattern as an argument. All the files to be deleted should match the pattern and all other files shouldn't match the pattern.</p><p>Polycarp doesn't know about an asterisk '<span class="tex-font-style-tt">*</span>', the only special character he knows is a question mark '<span class="tex-font-style-tt">?</span>' which matches any single character. All other characters in the pattern match themselves only.</p><p>Formally, a pattern matches a filename if and only if they have equal lengths and all characters in the corresponding positions are equal except when the character in the pattern is '<span class="tex-font-style-tt">?</span>', in which case the corresponding filename character does not matter.</p><p>For example, the filename pattern "<span class="tex-font-style-tt">a?ba?</span>":</p><ul> <li> matches filenames "<span class="tex-font-style-tt">aabaa</span>", "<span class="tex-font-style-tt">abba.</span>", "<span class="tex-font-style-tt">a.ba9</span>" and "<span class="tex-font-style-tt">a.ba.</span>"; </li><li> does not match filenames "<span class="tex-font-style-tt">aaba</span>", "<span class="tex-font-style-tt">abaab</span>", "<span class="tex-font-style-tt">aabaaa</span>" and "<span class="tex-font-style-tt">aabaa.</span>". </li></ul><p>Help Polycarp find a pattern which matches files to be deleted and only them or report if there is no such pattern.</p></div><div class="input-specification"><p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ <i>n</i> ≤ 100</span>) — the total number of files and the number of files to be deleted.</p><p>The following <span class="tex-span"><i>n</i></span> lines contain filenames, single filename per line. All filenames are non-empty strings containing only lowercase English letters, digits and dots ('<span class="tex-font-style-tt">.</span>'). The length of each filename doesn't exceed 100. It is guaranteed that all filenames are distinct.</p><p>The last line of the input contains <span class="tex-span"><i>m</i></span> distinct integer numbers in ascending order <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>m</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) — indices of files to be deleted. All files are indexed from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> in order of their appearance in the input.</p></div><div class="output-specification"><p>If the required pattern exists, print "<span class="tex-font-style-tt">Yes</span>" in the first line of the output. The second line should contain the required pattern. If there are multiple solutions, print any of them.</p><p>If the required pattern doesn't exist, print the only line containing "<span class="tex-font-style-tt">No</span>".</p></div>

## Input

<p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ <i>n</i> ≤ 100</span>) — the total number of files and the number of files to be deleted.</p><p>The following <span class="tex-span"><i>n</i></span> lines contain filenames, single filename per line. All filenames are non-empty strings containing only lowercase English letters, digits and dots ('<span class="tex-font-style-tt">.</span>'). The length of each filename doesn't exceed 100. It is guaranteed that all filenames are distinct.</p><p>The last line of the input contains <span class="tex-span"><i>m</i></span> distinct integer numbers in ascending order <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>m</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) — indices of files to be deleted. All files are indexed from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> in order of their appearance in the input.</p>

## Output

<p>If the required pattern exists, print "<span class="tex-font-style-tt">Yes</span>" in the first line of the output. The second line should contain the required pattern. If there are multiple solutions, print any of them.</p><p>If the required pattern doesn't exist, print the only line containing "<span class="tex-font-style-tt">No</span>".</p>





```input1
3 2
ab
ac
cd
1 2

```




```input2
5 3
test
tezt
test.
.est
tes.
1 4 5

```




```input3
4 4
a
b
c
dd
1 2 3 4

```




```input4
6 3
.svn
.git
....
...
..
.
1 2 3

```




```output1
Yes
a?

```




```output2
Yes
?es?

```




```output3
No

```




```output4
Yes
.???

```


