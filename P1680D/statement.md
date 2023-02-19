## Description

<div><p>You are walking with your dog, and now you are at the promenade. The promenade can be represented as an infinite line. Initially, you are in the point $0$ with your dog. </p><p>You decided to give some freedom to your dog, so you untied her and let her run for a while. Also, you watched what your dog is doing, so you have some writings about how she ran. During the $i$-th minute, the dog position changed from her previous position by the value $a_i$ (it means, that the dog ran for $a_i$ meters during the $i$-th minute). If $a_i$ is positive, the dog ran $a_i$ meters to the right, otherwise (if $a_i$ is negative) she ran $a_i$ meters to the left.</p><p>During some minutes, you were chatting with your friend, so you don't have writings about your dog movement during these minutes. These values $a_i$ equal zero.</p><p>You want your dog to return to you after the end of the walk, so the destination point of the dog after $n$ minutes <span class="tex-font-style-bf">should be</span> $0$.</p><p>Now you are wondering: what is the maximum possible number of different <span class="tex-font-style-bf">integer points</span> of the line your dog could visit on her way, if you replace every $0$ with some integer from $-k$ to $k$ (and your dog <span class="tex-font-style-bf">should</span> return to $0$ after the walk)? The dog visits an integer point if she runs through that point or reaches in it at the end of any minute. Point $0$ is always visited by the dog, since she is initially there.</p><p>If the dog cannot return to the point $0$ after $n$ minutes regardless of the integers you place, print <span class="tex-font-style-tt">-1</span>.</p></div><div class="input-specification"><p>The first line of the input contains two integers $n$ and $k$ ($1 \le n \le 3000; 1 \le k \le 10^9$) — the number of minutes and the maximum possible speed of your dog during the minutes without records.</p><p>The second line of the input contains $n$ integers $a_1, a_2, \ldots, a_n$ ($-10^9 \le a_i \le 10^9$), where $a_i$ is the number of meters your dog ran during the $i$-th minutes (to the left if $a_i$ is negative, to the right otherwise). If $a_i = 0$ then this value is <span class="tex-font-style-bf">unknown</span> and can be replaced with any integer from the range $[-k; k]$.</p></div><div class="output-specification"><p>If the dog cannot return to the point $0$ after $n$ minutes regardless of the set of integers you place, print <span class="tex-font-style-tt">-1</span>. Otherwise, print one integer — the maximum number of <span class="tex-font-style-bf">different</span> integer points your dog could visit if you fill all the unknown values optimally and the dog will return to the point $0$ at the end of the walk.</p></div>

## Input

<p>The first line of the input contains two integers $n$ and $k$ ($1 \le n \le 3000; 1 \le k \le 10^9$) — the number of minutes and the maximum possible speed of your dog during the minutes without records.</p><p>The second line of the input contains $n$ integers $a_1, a_2, \ldots, a_n$ ($-10^9 \le a_i \le 10^9$), where $a_i$ is the number of meters your dog ran during the $i$-th minutes (to the left if $a_i$ is negative, to the right otherwise). If $a_i = 0$ then this value is <span class="tex-font-style-bf">unknown</span> and can be replaced with any integer from the range $[-k; k]$.</p>

## Output

<p>If the dog cannot return to the point $0$ after $n$ minutes regardless of the set of integers you place, print <span class="tex-font-style-tt">-1</span>. Otherwise, print one integer — the maximum number of <span class="tex-font-style-bf">different</span> integer points your dog could visit if you fill all the unknown values optimally and the dog will return to the point $0$ at the end of the walk.</p>





```input1
3 2
5 0 -4
```




```input2
6 4
1 -2 0 3 -4 5
```




```input3
3 1000000000
0 0 0
```




```input4
5 9
-7 -3 8 12 0
```




```input5
5 3
-1 0 3 3 0
```




```input6
5 4
0 2 0 3 0
```




```output1
6
```




```output2
7
```




```output3
1000000001
```




```output4
-1
```




```output5
7
```




```output6
9
```


