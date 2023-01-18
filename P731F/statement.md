## Description

<div><p>Little Vlad is fond of popular computer game Bota-2. Recently, the developers announced the new add-on named Bota-3. Of course, Vlad immediately bought only to find out his computer is too old for the new game and needs to be updated.</p><p>There are <span class="tex-span"><i>n</i></span> video cards in the shop, the power of the <span class="tex-span"><i>i</i></span>-th video card is equal to integer value <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>. As Vlad wants to be sure the new game will work he wants to buy not one, but several video cards and unite their powers using the cutting-edge technology. To use this technology one of the cards is chosen as the leading one and other video cards are attached to it as secondary. For this new technology to work it's required that the power of each of the secondary video cards is divisible by the power of the leading video card. In order to achieve that the power of any secondary video card can be reduced to any integer value less or equal than the current power. However, the power of the leading video card should remain unchanged, i.e. it <span class="tex-font-style-bf">can't</span> be reduced.</p><p>Vlad has an infinite amount of money so he can buy any set of video cards. Help him determine which video cards he should buy such that after picking the leading video card and may be reducing some powers of others to make them work together he will get the maximum total value of video power.</p></div><div class="input-specification"><p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200 000</span>)&nbsp;— the number of video cards in the shop.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 200 000</span>)&nbsp;— powers of video cards.</p></div><div class="output-specification"><p>The only line of the output should contain one integer value&nbsp;— the maximum possible total power of video cards working together.</p></div>

## Input

<p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200 000</span>)&nbsp;— the number of video cards in the shop.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 200 000</span>)&nbsp;— powers of video cards.</p>

## Output

<p>The only line of the output should contain one integer value&nbsp;— the maximum possible total power of video cards working together.</p>





```input1
4
3 2 15 9

```




```input2
4
8 2 2 7

```




```output1
27

```




```output2
18

```



## Note

<p>In the first sample, it would be optimal to buy video cards with powers <span class="tex-span">3</span>, <span class="tex-span">15</span> and <span class="tex-span">9</span>. The video card with power <span class="tex-span">3</span> should be chosen as the leading one and all other video cards will be compatible with it. Thus, the total power would be <span class="tex-span">3 + 15 + 9 = 27</span>. If he buys all the video cards and pick the one with the power <span class="tex-span">2</span> as the leading, the powers of all other video cards should be reduced by <span class="tex-span">1</span>, thus the total power would be <span class="tex-span">2 + 2 + 14 + 8 = 26</span>, that is less than <span class="tex-span">27</span>. Please note, that it's not allowed to reduce the power of the leading video card, i.e. one can't get the total power <span class="tex-span">3 + 1 + 15 + 9 = 28</span>.</p><p>In the second sample, the optimal answer is to buy all video cards and pick the one with the power <span class="tex-span">2</span> as the leading. The video card with the power <span class="tex-span">7</span> needs it power to be reduced down to <span class="tex-span">6</span>. The total power would be <span class="tex-span">8 + 2 + 2 + 6 = 18</span>.</p>
