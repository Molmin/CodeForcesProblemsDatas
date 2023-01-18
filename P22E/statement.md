## Description

<div><p>To learn as soon as possible the latest news about their favourite fundamentally new operating system, BolgenOS community from Nizhni Tagil decided to develop a scheme. According to this scheme a community member, who is the first to learn the news, calls some other member, the latter, in his turn, calls some third member, and so on; i.e. a person with index <span class="tex-span"><i>i</i></span> got a person with index <span class="tex-span"><i>f</i><sub class="lower-index"><i>i</i></sub></span>, to whom he has to call, if he learns the news. With time BolgenOS community members understood that their scheme doesn't work sometimes — there were cases when some members didn't learn the news at all. Now they want to supplement the scheme: they <span class="tex-font-style-underline">add</span> into the scheme some instructions of type <span class="tex-span">(<i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>)</span>, which mean that person <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> has to call person <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> as well. What is the minimum amount of instructions that they need to add so, that at the end everyone learns the news, no matter who is the first to learn it?</p></div><div class="input-specification"><p>The first input line contains number <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — amount of BolgenOS community members. The second line contains <span class="tex-span"><i>n</i></span> space-separated integer numbers <span class="tex-span"><i>f</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>f</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, <i>i</i> ≠ <i>f</i><sub class="lower-index"><i>i</i></sub></span>) — index of a person, to whom calls a person with index <span class="tex-span"><i>i</i></span>.</p></div><div class="output-specification"><p>In the first line output one number — the minimum amount of instructions to add. Then output one of the possible variants to add these instructions into the scheme, one instruction in each line. If the solution is not unique, output any.</p></div>

## Input

<p>The first input line contains number <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — amount of BolgenOS community members. The second line contains <span class="tex-span"><i>n</i></span> space-separated integer numbers <span class="tex-span"><i>f</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>f</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, <i>i</i> ≠ <i>f</i><sub class="lower-index"><i>i</i></sub></span>) — index of a person, to whom calls a person with index <span class="tex-span"><i>i</i></span>.</p>

## Output

<p>In the first line output one number — the minimum amount of instructions to add. Then output one of the possible variants to add these instructions into the scheme, one instruction in each line. If the solution is not unique, output any.</p>





```input1
3
3 3 2

```




```input2
7
2 3 1 3 4 4 1

```




```output1
1
3 1

```




```output2
3
2 5
2 6
3 7

```


