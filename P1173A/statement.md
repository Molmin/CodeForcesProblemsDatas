## Description

<div><p>Nauuo is a girl who loves writing comments.</p><p>One day, she posted a comment on Codeforces, wondering whether she would get upvotes or downvotes.</p><p>It's known that there were $x$ persons who would upvote, $y$ persons who would downvote, and there were also another $z$ persons who would vote, but you don't know whether they would upvote or downvote. Note that each of the $x+y+z$ people would vote exactly one time.</p><p>There are three different results: if there are more people upvote than downvote, the result will be "+"; if there are more people downvote than upvote, the result will be "-"; otherwise the result will be "0".</p><p>Because of the $z$ unknown persons, the result may be uncertain (i.e. there are more than one possible results). More formally, the result is uncertain if and only if there exist two different situations of how the $z$ persons vote, that the results are different in the two situations.</p><p>Tell Nauuo the result or report that the result is uncertain.</p></div><div class="input-specification"><p>The only line contains three integers $x$, $y$, $z$ ($0\le x,y,z\le100$), corresponding to the number of persons who would upvote, downvote or unknown.</p></div><div class="output-specification"><p>If there is <span class="tex-font-style-bf">only one</span> possible result, print the result : "+", "-" or "0".</p><p>Otherwise, print "?" to report that the result is uncertain.</p></div>

## Input

<p>The only line contains three integers $x$, $y$, $z$ ($0\le x,y,z\le100$), corresponding to the number of persons who would upvote, downvote or unknown.</p>

## Output

<p>If there is <span class="tex-font-style-bf">only one</span> possible result, print the result : "+", "-" or "0".</p><p>Otherwise, print "?" to report that the result is uncertain.</p>





```input1
3 7 0
```




```input2
2 0 1
```




```input3
1 1 0
```




```input4
0 0 1
```




```output1
-
```




```output2
+
```




```output3
0
```




```output4
?
```



## Note

<p>In the first example, Nauuo would definitely get three upvotes and seven downvotes, so the only possible result is "-".</p><p>In the second example, no matter the person unknown downvotes or upvotes, Nauuo would get more upvotes than downvotes. So the only possible result is "+".</p><p>In the third example, Nauuo would definitely get one upvote and one downvote, so the only possible result is "0".</p><p>In the fourth example, if the only one person upvoted, the result would be "+", otherwise, the result would be "-". There are two possible results, so the result is uncertain.</p>
