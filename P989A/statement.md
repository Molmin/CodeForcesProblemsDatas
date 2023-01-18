## Description

<div><div class="epigraph"><div class="epigraph-text"><span class="tex-font-style-it"> When the curtains are opened, a canvas unfolds outside. Kanno marvels at all the blonde colours along the riverside&nbsp;— not tangerines, but blossoms instead.<p>"What a pity it's already late spring," sighs Mino with regret, "one more drizzling night and they'd be gone."</p><p>"But these blends are at their best, aren't they?" Absorbed in the landscape, Kanno remains optimistic. </p></span></div></div><p>The landscape can be expressed as a row of consecutive cells, each of which either contains a flower of colour amber or buff or canary yellow, or is empty.</p><p>When a flower withers, it disappears from the cell that it originally belonged to, and it spreads petals of its colour in its two neighbouring cells (or outside the field if the cell is on the side of the landscape). In case petals fall outside the given cells, they simply become invisible.</p><p>You are to help Kanno determine whether it's possible that after some (possibly none or all) flowers shed their petals, at least one of the cells contains all three colours, considering both petals and flowers. Note that flowers can wither in arbitrary order.</p></div><div class="input-specification"><p>The first and only line of input contains a non-empty string $s$ consisting of uppercase English letters '<span class="tex-font-style-tt">A</span>', '<span class="tex-font-style-tt">B</span>', '<span class="tex-font-style-tt">C</span>' and characters '<span class="tex-font-style-tt">.</span>' (dots) only ($\lvert s \rvert \leq 100$)&nbsp;— denoting cells containing an amber flower, a buff one, a canary yellow one, and no flowers, respectively.</p></div><div class="output-specification"><p>Output "<span class="tex-font-style-tt">Yes</span>" if it's possible that all three colours appear in some cell, and "<span class="tex-font-style-tt">No</span>" otherwise.</p><p>You can print each letter in any case (upper or lower).</p></div>

## Input

<p>The first and only line of input contains a non-empty string $s$ consisting of uppercase English letters '<span class="tex-font-style-tt">A</span>', '<span class="tex-font-style-tt">B</span>', '<span class="tex-font-style-tt">C</span>' and characters '<span class="tex-font-style-tt">.</span>' (dots) only ($\lvert s \rvert \leq 100$)&nbsp;— denoting cells containing an amber flower, a buff one, a canary yellow one, and no flowers, respectively.</p>

## Output

<p>Output "<span class="tex-font-style-tt">Yes</span>" if it's possible that all three colours appear in some cell, and "<span class="tex-font-style-tt">No</span>" otherwise.</p><p>You can print each letter in any case (upper or lower).</p>





```input1
.BAC.

```




```input2
AA..CB

```




```output1
Yes

```




```output2
No

```



## Note

<p>In the first example, the buff and canary yellow flowers can leave their petals in the central cell, blending all three colours in it.</p><p>In the second example, it's impossible to satisfy the requirement because there is no way that amber and buff meet in any cell.</p>
