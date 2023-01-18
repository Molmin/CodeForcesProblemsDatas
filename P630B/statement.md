## Description

<div><p>The city administration of IT City decided to fix up a symbol of scientific and technical progress in the city's main square, namely an indicator board that shows the effect of Moore's law in real time.</p><p>Moore's law is the observation that the number of transistors in a dense integrated circuit doubles approximately every <span class="tex-span">24</span> months. The implication of Moore's law is that computer performance as function of time increases exponentially as well.</p><p>You are to prepare information that will change every second to display on the indicator board. Let's assume that every second the number of transistors increases exactly <span class="tex-span">1.000000011</span> times.</p></div><div class="input-specification"><p>The only line of the input contains a pair of integers <span class="tex-span"><i>n</i></span> (<span class="tex-span">1000 ≤ <i>n</i> ≤ 10&nbsp;000</span>) and <span class="tex-span"><i>t</i></span> (<span class="tex-span">0 ≤ <i>t</i> ≤ 2&nbsp;000&nbsp;000&nbsp;000</span>)&nbsp;— the number of transistors in the initial time and the number of seconds passed since the initial time.</p></div><div class="output-specification"><p>Output one number — the estimate of the number of transistors in a dence integrated circuit in <span class="tex-span"><i>t</i></span> seconds since the initial time. The relative error of your answer should not be greater than <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p></div>

## Input

<p>The only line of the input contains a pair of integers <span class="tex-span"><i>n</i></span> (<span class="tex-span">1000 ≤ <i>n</i> ≤ 10&nbsp;000</span>) and <span class="tex-span"><i>t</i></span> (<span class="tex-span">0 ≤ <i>t</i> ≤ 2&nbsp;000&nbsp;000&nbsp;000</span>)&nbsp;— the number of transistors in the initial time and the number of seconds passed since the initial time.</p>

## Output

<p>Output one number — the estimate of the number of transistors in a dence integrated circuit in <span class="tex-span"><i>t</i></span> seconds since the initial time. The relative error of your answer should not be greater than <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p>





```input1
1000 1000000

```




```output1
1011.060722383550382782399454922040

```


