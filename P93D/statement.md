## Description

<div><p>When Igor K. was a freshman, his professor strictly urged him, as well as all other freshmen, to solve programming Olympiads. One day a problem called "Flags" from a website called Timmy's Online Judge caught his attention. In the problem one had to find the number of three-colored flags that would satisfy the condition... actually, it doesn't matter. Igor K. quickly found the formula and got the so passionately desired Accepted.</p><p>However, the professor wasn't very much impressed. He decided that the problem represented on Timmy's Online Judge was very dull and simple: it only had three possible colors of flag stripes and only two limitations. He suggested a complicated task to Igor K. and the fellow failed to solve it. Of course, we won't tell anybody that the professor couldn't solve it as well.</p><p>And how about you? Can you solve the problem?</p><p>The flags consist of one or several parallel stripes of similar width. The stripes can be one of the following colors: white, black, red or yellow. You should find the number of different flags with the number of stripes from <span class="tex-span"><i>L</i></span> to <span class="tex-span"><i>R</i></span>, if:</p><ul> <li> a flag cannot have adjacent stripes of one color; </li><li> a flag cannot have adjacent white and yellow stripes; </li><li> a flag cannot have adjacent red and black stripes; </li><li> a flag cannot have the combination of black, white and red stripes following one after another in this or reverse order; </li><li> symmetrical flags (as, for example, a WB and a BW flag, where W and B stand for the white and black colors) are considered the same. </li></ul></div><div class="input-specification"><p>The only line contains two integers <span class="tex-span"><i>L</i></span> and <span class="tex-span"><i>R</i></span> (<span class="tex-span">1 ≤ <i>L</i> ≤ <i>R</i> ≤ 10<sup class="upper-index">9</sup></span>). They are the lower and upper borders of the number of stripes on the flag.</p></div><div class="output-specification"><p>Print a single number — the number of different flags that would satisfy the condition of the problem and would have from <span class="tex-span"><i>L</i></span> to <span class="tex-span"><i>R</i></span> stripes, modulo <span class="tex-span">1000000007</span>.</p></div>

## Input

<p>The only line contains two integers <span class="tex-span"><i>L</i></span> and <span class="tex-span"><i>R</i></span> (<span class="tex-span">1 ≤ <i>L</i> ≤ <i>R</i> ≤ 10<sup class="upper-index">9</sup></span>). They are the lower and upper borders of the number of stripes on the flag.</p>

## Output

<p>Print a single number — the number of different flags that would satisfy the condition of the problem and would have from <span class="tex-span"><i>L</i></span> to <span class="tex-span"><i>R</i></span> stripes, modulo <span class="tex-span">1000000007</span>.</p>





```input1
3 4

```




```input2
5 6

```




```output1
23
```




```output2
64
```



## Note

<p>In the first test the following flags exist (they are listed in the lexicographical order, the letters B, R, W, Y stand for Black, Red, White and Yellow correspondingly):</p><p>3 stripes: BWB, BYB, BYR, RWR, RYR, WBW, WBY, WRW, WRY, YBY, YRY (overall 11 flags).</p><p>4 stripes: BWBW, BWBY, BYBW, BYBY, BYRW, BYRY, RWRW, RWRY, RYBW, RYBY, RYRW, RYRY (12 flags).</p><p>That's why the answer to test 1 is equal to <span class="tex-span">11 + 12 = 23</span>.</p>
