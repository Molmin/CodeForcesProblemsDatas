## Description

<div><p>Phoenix is trying to take a photo of his $n$ friends with labels $1, 2, \dots, n$ who are lined up in a row in a special order. But before he can take the photo, his friends get distracted by a duck and mess up their order.</p><p>Now, Phoenix must restore the order but he doesn't remember completely! He only remembers that the $i$-th friend from the left had a label between $a_i$ and $b_i$ inclusive. Does there exist a unique way to order his friends based of his memory? </p></div><div class="input-specification"><p>The first line contains one integer $n$ ($1 \le n \le 2\cdot10^5$) &nbsp;— the number of friends.</p><p>The $i$-th of the next $n$ lines contain two integers $a_i$ and $b_i$ ($1 \le a_i \le b_i \le n$) &nbsp;— Phoenix's memory of the $i$-th position from the left.</p><p>It is guaranteed that Phoenix's memory is valid so there is at least one valid ordering.</p></div><div class="output-specification"><p>If Phoenix can reorder his friends in a unique order, print <span class="tex-font-style-tt">YES</span> followed by $n$ integers &nbsp;— the $i$-th integer should be the label of the $i$-th friend from the left.</p><p>Otherwise, print <span class="tex-font-style-tt">NO</span>. Then, <span class="tex-font-style-bf">print any two distinct valid orderings</span> on the following two lines. If are multiple solutions, print any.</p></div>

## Input

<p>The first line contains one integer $n$ ($1 \le n \le 2\cdot10^5$) &nbsp;— the number of friends.</p><p>The $i$-th of the next $n$ lines contain two integers $a_i$ and $b_i$ ($1 \le a_i \le b_i \le n$) &nbsp;— Phoenix's memory of the $i$-th position from the left.</p><p>It is guaranteed that Phoenix's memory is valid so there is at least one valid ordering.</p>

## Output

<p>If Phoenix can reorder his friends in a unique order, print <span class="tex-font-style-tt">YES</span> followed by $n$ integers &nbsp;— the $i$-th integer should be the label of the $i$-th friend from the left.</p><p>Otherwise, print <span class="tex-font-style-tt">NO</span>. Then, <span class="tex-font-style-bf">print any two distinct valid orderings</span> on the following two lines. If are multiple solutions, print any.</p>





```input1
4
4 4
1 3
2 4
3 4
```




```input2
4
1 3
2 4
3 4
2 3
```




```output1
YES
4 1 2 3
```




```output2
NO
1 3 4 2 
1 2 4 3
```


