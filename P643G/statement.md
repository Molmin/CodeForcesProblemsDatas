## Description

<div><p>One social network developer recently suggested a new algorithm of choosing ads for users.</p><p>There are <span class="tex-span"><i>n</i></span> slots which advertisers can buy. It is possible to buy a segment of consecutive slots at once. The more slots you own, the bigger are the chances your ad will be shown to users.</p><p>Every time it is needed to choose ads to show, some segment of slots is picked by a secret algorithm. Then some advertisers are chosen. The only restriction is that it should be guaranteed for advertisers which own at least <span class="tex-span"><i>p</i></span>% of slots composing this segment that their ad will be shown.</p><p>From the other side, users don't like ads. So it was decided to show no more than <img align="middle" class="tex-formula" src="file://Xx0Fy9mC.png" style="max-width: 100.0%;max-height: 100.0%;"> ads at once. You are asked to develop a system to sell segments of slots and choose ads in accordance with the rules described above.</p></div><div class="input-specification"><p>The first line of the input contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>p</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 150 000, 20 ≤ <i>p</i> ≤ 100</span>)&nbsp;— the number of slots, the number of queries to your system and threshold for which display of the ad is guaranteed.</p><p>Next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 150 000)</span>, where the <span class="tex-span"><i>i</i></span>-th number means id of advertiser who currently owns the <span class="tex-span"><i>i</i></span>-th slot.</p><p>Next <span class="tex-span"><i>m</i></span> lines contain queries descriptions. Each description is of one of the following forms: </p><ul> <li> <span class="tex-font-style-tt">1 l r id</span> (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i>, 1 ≤ <i>id</i> ≤ 150 000</span>)&nbsp;— advertiser <span class="tex-span"><i>id</i></span> bought all slots in a range from <span class="tex-span"><i>l</i></span> to <span class="tex-span"><i>r</i></span> inclusive; </li><li> <span class="tex-font-style-tt">2 l r</span> (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i></span>)&nbsp;— you need to choose advertisers for segment <span class="tex-span">[<i>l</i>, <i>r</i>]</span>. </li></ul></div><div class="output-specification"><p>For each query of the second type answer should be printed in a separate line. First integer of the answer should be the number of advertisements that will be shown <img align="middle" class="tex-formula" src="file://SayTVQxp.png" style="max-width: 100.0%;max-height: 100.0%;">. Next <span class="tex-span"><i>cnt</i></span> integers should be advertisers' ids. </p><p>It is allowed to print one advertiser more than once, but each advertiser that owns at least <img align="middle" class="tex-formula" src="file://7G2K7TZD.png" style="max-width: 100.0%;max-height: 100.0%;"> slots of the segment from <span class="tex-span"><i>l</i></span> to <span class="tex-span"><i>r</i></span> should be in your answer.</p></div>

## Input

<p>The first line of the input contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>p</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 150 000, 20 ≤ <i>p</i> ≤ 100</span>)&nbsp;— the number of slots, the number of queries to your system and threshold for which display of the ad is guaranteed.</p><p>Next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 150 000)</span>, where the <span class="tex-span"><i>i</i></span>-th number means id of advertiser who currently owns the <span class="tex-span"><i>i</i></span>-th slot.</p><p>Next <span class="tex-span"><i>m</i></span> lines contain queries descriptions. Each description is of one of the following forms: </p><ul> <li> <span class="tex-font-style-tt">1 l r id</span> (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i>, 1 ≤ <i>id</i> ≤ 150 000</span>)&nbsp;— advertiser <span class="tex-span"><i>id</i></span> bought all slots in a range from <span class="tex-span"><i>l</i></span> to <span class="tex-span"><i>r</i></span> inclusive; </li><li> <span class="tex-font-style-tt">2 l r</span> (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i></span>)&nbsp;— you need to choose advertisers for segment <span class="tex-span">[<i>l</i>, <i>r</i>]</span>. </li></ul>

## Output

<p>For each query of the second type answer should be printed in a separate line. First integer of the answer should be the number of advertisements that will be shown <img align="middle" class="tex-formula" src="file://SayTVQxp.png" style="max-width: 100.0%;max-height: 100.0%;">. Next <span class="tex-span"><i>cnt</i></span> integers should be advertisers' ids. </p><p>It is allowed to print one advertiser more than once, but each advertiser that owns at least <img align="middle" class="tex-formula" src="file://7G2K7TZD.png" style="max-width: 100.0%;max-height: 100.0%;"> slots of the segment from <span class="tex-span"><i>l</i></span> to <span class="tex-span"><i>r</i></span> should be in your answer.</p>





```input1
5 9 33
1 2 1 3 3
2 1 5
2 1 5
2 1 3
2 3 3
1 2 4 5
2 1 5
2 3 5
1 4 5 1
2 1 5

```




```output1
3 1 2 3
2 1 3
2 2 1
3 1 1000 1000
1 5
2 5 3
2 1 5
```



## Note

<p>Samples demonstrate that you actually have quite a lot of freedom in choosing advertisers.</p>
