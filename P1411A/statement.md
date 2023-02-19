## Description

<div><p>You have been assigned to develop a filter for bad messages in the in-game chat. A message is a string $S$ of length $n$, consisting of lowercase English letters and characters '<span class="tex-font-style-tt">)</span>'. The message is <span class="tex-font-style-it">bad</span> if the number of characters '<span class="tex-font-style-tt">)</span>' at the end of the string strictly greater than the number of remaining characters. For example, the string "<span class="tex-font-style-tt">)bc)))</span>" has three parentheses at the end, three remaining characters, and is not considered bad.</p></div><div class="input-specification"><p>The first line contains the number of test cases $t$ ($1 \leq t \leq 100$). Description of the $t$ test cases follows.</p><p>The first line of each test case contains an integer $n$ ($1 \leq n \leq 100$). The second line of each test case contains a string $S$ of length $n$, consisting of lowercase English letters and characters '<span class="tex-font-style-tt">)</span>'.</p></div><div class="output-specification"><p>For each of $t$ test cases, print "<span class="tex-font-style-tt">Yes</span>" if the string is bad. Otherwise, print "<span class="tex-font-style-tt">No</span>".</p><p>You can print each letter in any case (upper or lower).</p></div>

## Input

<p>The first line contains the number of test cases $t$ ($1 \leq t \leq 100$). Description of the $t$ test cases follows.</p><p>The first line of each test case contains an integer $n$ ($1 \leq n \leq 100$). The second line of each test case contains a string $S$ of length $n$, consisting of lowercase English letters and characters '<span class="tex-font-style-tt">)</span>'.</p>

## Output

<p>For each of $t$ test cases, print "<span class="tex-font-style-tt">Yes</span>" if the string is bad. Otherwise, print "<span class="tex-font-style-tt">No</span>".</p><p>You can print each letter in any case (upper or lower).</p>





```input1
5
2
))
12
gl))hf))))))
9
gege)))))
14
)aa))b))))))))
1
)
```




```output1
Yes
No
Yes
Yes
Yes
```


