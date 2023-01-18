## Description

<div><p>Ford Prefect got a job as a web developer for a small company that makes towels. His current work task is to create a search engine for the website of the company. During the development process, he needs to write a subroutine for comparing strings <span class="tex-span"><i>S</i></span> and <span class="tex-span"><i>T</i></span> of equal length to be "similar". After a brief search on the Internet, he learned about the <span class="tex-font-style-it">Hamming distance</span> between two strings <span class="tex-span"><i>S</i></span> and <span class="tex-span"><i>T</i></span> of the same length, which is defined as the number of positions in which <span class="tex-span"><i>S</i></span> and <span class="tex-span"><i>T</i></span> have different characters. For example, the Hamming distance between words "<span class="tex-font-style-tt">permanent</span>" and "<span class="tex-font-style-tt">pergament</span>" is two, as these words differ in the fourth and sixth letters.</p><p>Moreover, as he was searching for information, he also noticed that modern search engines have powerful mechanisms to correct errors in the request to improve the quality of search. Ford doesn't know much about human beings, so he assumed that the most common mistake in a request is swapping two arbitrary letters of the string (not necessarily adjacent). Now he wants to write a function that determines which two letters should be swapped in string <span class="tex-span"><i>S</i></span>, so that the Hamming distance between a new string <span class="tex-span"><i>S</i></span> and string <span class="tex-span"><i>T</i></span> would be as small as possible, or otherwise, determine that such a replacement cannot reduce the distance between the strings.</p><p>Help him do this!</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200 000</span>) — the length of strings <span class="tex-span"><i>S</i></span> and <span class="tex-span"><i>T</i></span>.</p><p>The second line contains string <span class="tex-span"><i>S</i></span>.</p><p>The third line contains string <span class="tex-span"><i>T</i></span>.</p><p>Each of the lines only contains <span class="tex-font-style-bf">lowercase</span> Latin letters.</p></div><div class="output-specification"><p>In the first line, print number <span class="tex-span"><i>x</i></span> — the minimum possible Hamming distance between strings <span class="tex-span"><i>S</i></span> and <span class="tex-span"><i>T</i></span> if you swap at most one pair of letters in <span class="tex-span"><i>S</i></span>.</p><p>In the second line, either print the indexes <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> (<span class="tex-span">1 ≤ <i>i</i>, <i>j</i> ≤ <i>n</i></span>, <span class="tex-span"><i>i</i> ≠ <i>j</i></span>), if reaching the minimum possible distance is possible by swapping letters on positions <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span>, or print "<span class="tex-font-style-tt">-1 -1</span>", if it is not necessary to swap characters.</p><p>If there are multiple possible answers, print any of them.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200 000</span>) — the length of strings <span class="tex-span"><i>S</i></span> and <span class="tex-span"><i>T</i></span>.</p><p>The second line contains string <span class="tex-span"><i>S</i></span>.</p><p>The third line contains string <span class="tex-span"><i>T</i></span>.</p><p>Each of the lines only contains <span class="tex-font-style-bf">lowercase</span> Latin letters.</p>

## Output

<p>In the first line, print number <span class="tex-span"><i>x</i></span> — the minimum possible Hamming distance between strings <span class="tex-span"><i>S</i></span> and <span class="tex-span"><i>T</i></span> if you swap at most one pair of letters in <span class="tex-span"><i>S</i></span>.</p><p>In the second line, either print the indexes <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> (<span class="tex-span">1 ≤ <i>i</i>, <i>j</i> ≤ <i>n</i></span>, <span class="tex-span"><i>i</i> ≠ <i>j</i></span>), if reaching the minimum possible distance is possible by swapping letters on positions <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span>, or print "<span class="tex-font-style-tt">-1 -1</span>", if it is not necessary to swap characters.</p><p>If there are multiple possible answers, print any of them.</p>





```input1
9
pergament
permanent

```




```input2
6
wookie
cookie

```




```input3
4
petr
egor

```




```input4
6
double
bundle

```




```output1
1
4 6

```




```output2
1
-1 -1

```




```output3
2
1 2

```




```output4
2
4 1

```



## Note

<p>In the second test it is acceptable to print <span class="tex-span"><i>i</i> = 2</span>, <span class="tex-span"><i>j</i> = 3</span>.</p>
