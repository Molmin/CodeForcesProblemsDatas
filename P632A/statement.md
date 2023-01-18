## Description

<div><p>Grandma Laura came to the market to sell some apples. During the day she sold all the apples she had. But grandma is old, so she forgot how many apples she had brought to the market.</p><p>She precisely remembers she had <span class="tex-span"><i>n</i></span> buyers and each of them bought exactly half of the apples she had at the moment of the purchase and also she gave a half of an apple to some of them as a gift (if the number of apples at the moment of purchase was odd), until she sold all the apples she had.</p><p>So each buyer took some integral positive number of apples, but maybe he didn't pay for a half of an apple (if the number of apples at the moment of the purchase was odd).</p><p>For each buyer grandma remembers if she gave a half of an apple as a gift or not. The cost of an apple is <span class="tex-span"><i>p</i></span> (the number <span class="tex-span"><i>p</i></span> is even).</p><p>Print the total money grandma should have at the end of the day to check if some buyers cheated her.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>p</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 40, 2 ≤ <i>p</i> ≤ 1000</span>) — the number of the buyers and the cost of one apple. It is guaranteed that the number <span class="tex-span"><i>p</i></span> is even.</p><p>The next <span class="tex-span"><i>n</i></span> lines contains the description of buyers. Each buyer is described with the string <span class="tex-font-style-tt">half</span> if he simply bought half of the apples and with the string <span class="tex-font-style-tt">halfplus</span> if grandma also gave him a half of an apple as a gift.</p><p>It is guaranteed that grandma has at least one apple at the start of the day and she has no apples at the end of the day.</p></div><div class="output-specification"><p>Print the only integer <span class="tex-span"><i>a</i></span> — the total money grandma should have at the end of the day.</p><p>Note that the answer can be too large, so you should use <span class="tex-span">64</span>-bit integer type to store it. In <span class="tex-font-style-tt">C++</span> you can use the <span class="tex-font-style-tt">long long</span> integer type and in <span class="tex-font-style-tt">Java</span> you can use <span class="tex-font-style-tt">long</span> integer type.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>p</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 40, 2 ≤ <i>p</i> ≤ 1000</span>) — the number of the buyers and the cost of one apple. It is guaranteed that the number <span class="tex-span"><i>p</i></span> is even.</p><p>The next <span class="tex-span"><i>n</i></span> lines contains the description of buyers. Each buyer is described with the string <span class="tex-font-style-tt">half</span> if he simply bought half of the apples and with the string <span class="tex-font-style-tt">halfplus</span> if grandma also gave him a half of an apple as a gift.</p><p>It is guaranteed that grandma has at least one apple at the start of the day and she has no apples at the end of the day.</p>

## Output

<p>Print the only integer <span class="tex-span"><i>a</i></span> — the total money grandma should have at the end of the day.</p><p>Note that the answer can be too large, so you should use <span class="tex-span">64</span>-bit integer type to store it. In <span class="tex-font-style-tt">C++</span> you can use the <span class="tex-font-style-tt">long long</span> integer type and in <span class="tex-font-style-tt">Java</span> you can use <span class="tex-font-style-tt">long</span> integer type.</p>





```input1
2 10
half
halfplus

```




```input2
3 10
halfplus
halfplus
halfplus

```




```output1
15

```




```output2
55

```



## Note

<p>In the first sample at the start of the day the grandma had two apples. First she sold one apple and then she sold a half of the second apple and gave a half of the second apple as a present to the second buyer.</p>
