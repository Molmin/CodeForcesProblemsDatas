## Description

<div><p>Maxim wants to buy an apartment in a new house at Line Avenue of Metropolis. The house has <span class="tex-span"><i>n</i></span> apartments that are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> and are arranged in a row. Two apartments are adjacent if their indices differ by <span class="tex-span">1</span>. Some of the apartments can already be inhabited, others are available for sale.</p><p>Maxim often visits his neighbors, so apartment is <span class="tex-font-style-it">good</span> for him if it is available for sale and there is at least one already inhabited apartment adjacent to it. Maxim knows that there are exactly <span class="tex-span"><i>k</i></span> already inhabited apartments, but he doesn't know their indices yet.</p><p>Find out what could be the minimum possible and the maximum possible number of apartments that are good for Maxim.</p></div><div class="input-specification"><p>The only line of the input contains two integers: <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">0 ≤ <i>k</i> ≤ <i>n</i></span>).</p></div><div class="output-specification"><p>Print the minimum possible and the maximum possible number of apartments good for Maxim.</p></div>

## Input

<p>The only line of the input contains two integers: <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">0 ≤ <i>k</i> ≤ <i>n</i></span>).</p>

## Output

<p>Print the minimum possible and the maximum possible number of apartments good for Maxim.</p>





```input1
6 3

```




```output1
1 3

```



## Note

<p>In the sample test, the number of good apartments could be minimum possible if, for example, apartments with indices <span class="tex-span">1</span>, <span class="tex-span">2</span> and <span class="tex-span">3</span> were inhabited. In this case only apartment <span class="tex-span">4</span> is good. The maximum possible number could be, for example, if apartments with indices <span class="tex-span">1</span>, <span class="tex-span">3</span> and <span class="tex-span">5</span> were inhabited. In this case all other apartments: <span class="tex-span">2</span>, <span class="tex-span">4</span> and <span class="tex-span">6</span> are good.</p>
