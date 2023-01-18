## Description

<div><p>Heidi is a statistician to the core, and she likes to study the evolution of marmot populations in each of <span class="tex-span"><i>V</i></span> (<span class="tex-span">1 ≤ <i>V</i> ≤ 100</span>) villages! So it comes that every spring, when Heidi sees the first snowdrops sprout in the meadows around her barn, she impatiently dons her snowshoes and sets out to the Alps, to welcome her friends the marmots to a new season of thrilling adventures.</p><p>Arriving in a village, Heidi asks each and every marmot she comes across for the number of inhabitants of that village. This year, the marmots decide to play an April Fools' joke on Heidi. Instead of consistently providing the exact number of inhabitants <span class="tex-span"><i>P</i></span> (<span class="tex-span">10 ≤ <i>P</i> ≤ 1000</span>) of the village, they respond with a random non-negative integer <span class="tex-span"><i>k</i></span>, drawn from one of two types of probability distributions:</p><ul> <li> Poisson (d'avril) distribution: the probability of getting an answer <span class="tex-span"><i>k</i></span> is <img align="middle" class="tex-formula" src="file://29M5vgsj.png" style="max-width: 100.0%;max-height: 100.0%;"> for <span class="tex-span"><i>k</i> = 0, 1, 2, 3, ...</span>, </li><li> Uniform distribution: the probability of getting an answer <span class="tex-span"><i>k</i></span> is <img align="middle" class="tex-formula" src="file://bKxRdl6c.png" style="max-width: 100.0%;max-height: 100.0%;"> for <span class="tex-span"><i>k</i> = 0, 1, 2, ..., 2<i>P</i></span>. </li></ul><p>Heidi collects exactly 250 answers per village. Every village follows either the Poisson or the uniform distribution. Heidi cannot tell marmots apart, so she may query some marmots several times, and each time the marmot will answer with a new number drawn from the village's distribution.</p><p>Can you help Heidi to find out whether a village follows a Poisson or a uniform distribution?</p></div><div class="input-specification"><p>The first line of input will contain the number of villages <span class="tex-span"><i>V</i></span> (<span class="tex-span">1 ≤ <i>V</i> ≤ 100</span>). The following <span class="tex-span"><i>V</i></span> lines each describe one village. The description of each village consists of 250 space-separated integers <span class="tex-span"><i>k</i></span>, drawn from one of the above distributions.</p></div><div class="output-specification"><p>Output one line per village, in the same order as provided in the input. The village's line shall state <span class="tex-font-style-it">poisson</span> if the village's distribution is of the Poisson type, and <span class="tex-font-style-it">uniform</span> if the answer came from a uniform distribution.</p></div>

## Input

<p>The first line of input will contain the number of villages <span class="tex-span"><i>V</i></span> (<span class="tex-span">1 ≤ <i>V</i> ≤ 100</span>). The following <span class="tex-span"><i>V</i></span> lines each describe one village. The description of each village consists of 250 space-separated integers <span class="tex-span"><i>k</i></span>, drawn from one of the above distributions.</p>

## Output

<p>Output one line per village, in the same order as provided in the input. The village's line shall state <span class="tex-font-style-it">poisson</span> if the village's distribution is of the Poisson type, and <span class="tex-font-style-it">uniform</span> if the answer came from a uniform distribution.</p>





```input1
2
92 100 99 109 93 105 103 106 101 99 ... (input is truncated)
28 180 147 53 84 80 180 85 8 16 ... (input is truncated)
```




```output1
poisson
uniform

```



## Note

<p>The full example input is visually represented below, along with the probability distribution function it was drawn from (the <span class="tex-span"><i>y</i></span>-axis is labeled by its values multiplied by 250).</p><p><img class="tex-graphics" src="file://5rm2hShX.png" style="max-width: 100.0%;max-height: 100.0%;"></p>
