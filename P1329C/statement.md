## Description

<div><p>Drazil likes heap very much. So he created a problem with heap:</p><p>There is a max heap with a height $h$ implemented on the array. The details of this heap are the following:</p><p>This heap contains exactly $2^h - 1$ <span class="tex-font-style-bf">distinct</span> positive non-zero integers. All integers are distinct. These numbers are stored in the array $a$ indexed from $1$ to $2^h-1$. For any $1 &lt; i &lt; 2^h$, $a[i] &lt; a[\left \lfloor{\frac{i}{2}}\right \rfloor]$.</p><p>Now we want to reduce the height of this heap such that the height becomes $g$ with exactly $2^g-1$ numbers in heap. To reduce the height, we should perform the following action $2^h-2^g$ times:</p><p>Choose an index $i$, which contains an element and call the following function $f$ in index $i$:</p><p><img class="tex-graphics" src="file://EO40cLQ9.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>Note that we suppose that if $a[i]=0$, then index $i$ don't contain an element.</p><p>After all operations, the remaining $2^g-1$ element must be located in indices from $1$ to $2^g-1$. Now Drazil wonders what's the minimum possible sum of the remaining $2^g-1$ elements. Please find this sum and find a sequence of the function calls to achieve this value.</p></div><div class="input-specification"><p>The first line of the input contains an integer $t$ ($1 \leq t \leq 70\,000$): the number of test cases.</p><p>Each test case contain two lines. The first line contains two integers $h$ and $g$ ($1 \leq g &lt; h \leq 20$). The second line contains $n = 2^h-1$ <span class="tex-font-style-bf">distinct</span> positive integers $a[1], a[2], \ldots, a[n]$ ($1 \leq a[i] &lt; 2^{20}$). For all $i$ from $2$ to $2^h - 1$, $a[i] &lt; a[\left \lfloor{\frac{i}{2}}\right \rfloor]$.</p><p>The total sum of $n$ is less than $2^{20}$.</p></div><div class="output-specification"><p>For each test case, print two lines.</p><p>The first line should contain one integer denoting the minimum sum after reducing the height of heap to $g$. The second line should contain $2^h - 2^g$ integers $v_1, v_2, \ldots, v_{2^h-2^g}$. In $i$-th operation $f(v_i)$ should be called.</p></div>

## Input

<p>The first line of the input contains an integer $t$ ($1 \leq t \leq 70\,000$): the number of test cases.</p><p>Each test case contain two lines. The first line contains two integers $h$ and $g$ ($1 \leq g &lt; h \leq 20$). The second line contains $n = 2^h-1$ <span class="tex-font-style-bf">distinct</span> positive integers $a[1], a[2], \ldots, a[n]$ ($1 \leq a[i] &lt; 2^{20}$). For all $i$ from $2$ to $2^h - 1$, $a[i] &lt; a[\left \lfloor{\frac{i}{2}}\right \rfloor]$.</p><p>The total sum of $n$ is less than $2^{20}$.</p>

## Output

<p>For each test case, print two lines.</p><p>The first line should contain one integer denoting the minimum sum after reducing the height of heap to $g$. The second line should contain $2^h - 2^g$ integers $v_1, v_2, \ldots, v_{2^h-2^g}$. In $i$-th operation $f(v_i)$ should be called.</p>





```input1
2
3 2
7 6 3 5 4 2 1
3 2
7 6 5 4 3 2 1
```




```output1
10
3 2 3 1
8
2 1 3 1
```


