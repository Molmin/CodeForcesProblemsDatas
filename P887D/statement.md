## Description

<div><p>There are two main kinds of events in the life of top-model: fashion shows and photo shoots. Participating in any of these events affects the rating of appropriate top-model. After each photo shoot model's rating increases by <span class="tex-span"><i>a</i></span> and after each fashion show decreases by <span class="tex-span"><i>b</i></span> (designers do too many experiments nowadays). Moreover, sometimes top-models participates in talk shows. After participating in talk show model becomes more popular and increasing of her rating after photo shoots become <span class="tex-span"><i>c</i></span> and decreasing of her rating after fashion show becomes <span class="tex-span"><i>d</i></span>.</p><p>Izabella wants to participate in a talk show, but she wants to do it in such a way that her rating will never become negative. Help her to find a suitable moment for participating in the talk show. </p><p>Let's assume that model's career begins in moment 0. At that moment Izabella's rating was equal to <span class="tex-span"><i>start</i></span>. If talk show happens in moment <span class="tex-span"><i>t</i></span> if will affect all events in model's life in interval of time <span class="tex-span">[<i>t</i>..<i>t</i> + <i>len</i>)</span> (including <span class="tex-span"><i>t</i></span> and not including <span class="tex-span"><i>t</i> + <i>len</i></span>), where <span class="tex-span"><i>len</i></span> is duration of influence.</p><p>Izabella wants to participate in a talk show, but she wants to do it in such a way that her rating will not become become negative before talk show or during period of influence of talk show. Help her to find a suitable moment for participating in the talk show. </p></div><div class="input-specification"><p>In first line there are 7 positive integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span>, <span class="tex-span"><i>c</i></span>, <span class="tex-span"><i>d</i></span>, <span class="tex-span"><i>start</i></span>, <span class="tex-span"><i>len</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 3·10<sup class="upper-index">5</sup></span>, <span class="tex-span">0 ≤ <i>start</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>a</i>, <i>b</i>, <i>c</i>, <i>d</i>, <i>len</i> ≤ 10<sup class="upper-index">9</sup></span>), where <span class="tex-span"><i>n</i></span> is a number of fashion shows and photo shoots, <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span>, <span class="tex-span"><i>c</i></span> and <span class="tex-span"><i>d</i></span> are rating changes described above, <span class="tex-span"><i>start</i></span> is an initial rating of model and <span class="tex-span"><i>len</i></span> is a duration of influence of talk show.</p><p>In next <span class="tex-span"><i>n</i></span> lines descriptions of events are given. Each of those lines contains two integers <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>q</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">0 ≤ <i>q</i> ≤ 1</span>)&nbsp;— moment, in which event happens and type of this event. Type 0 corresponds to the fashion show and type 1&nbsp;— to photo shoot. </p><p>Events are given in order of increasing <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>, all <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> are different.</p></div><div class="output-specification"><p>Print one non-negative integer <span class="tex-span"><i>t</i></span>&nbsp;— the moment of time in which talk show should happen to make Izabella's rating non-negative before talk show and during period of influence of talk show. If there are multiple answers print smallest of them. If there are no such moments, print <span class="tex-span"> - 1</span>.</p></div>

## Input

<p>In first line there are 7 positive integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span>, <span class="tex-span"><i>c</i></span>, <span class="tex-span"><i>d</i></span>, <span class="tex-span"><i>start</i></span>, <span class="tex-span"><i>len</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 3·10<sup class="upper-index">5</sup></span>, <span class="tex-span">0 ≤ <i>start</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>a</i>, <i>b</i>, <i>c</i>, <i>d</i>, <i>len</i> ≤ 10<sup class="upper-index">9</sup></span>), where <span class="tex-span"><i>n</i></span> is a number of fashion shows and photo shoots, <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span>, <span class="tex-span"><i>c</i></span> and <span class="tex-span"><i>d</i></span> are rating changes described above, <span class="tex-span"><i>start</i></span> is an initial rating of model and <span class="tex-span"><i>len</i></span> is a duration of influence of talk show.</p><p>In next <span class="tex-span"><i>n</i></span> lines descriptions of events are given. Each of those lines contains two integers <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>q</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">0 ≤ <i>q</i> ≤ 1</span>)&nbsp;— moment, in which event happens and type of this event. Type 0 corresponds to the fashion show and type 1&nbsp;— to photo shoot. </p><p>Events are given in order of increasing <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>, all <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> are different.</p>

## Output

<p>Print one non-negative integer <span class="tex-span"><i>t</i></span>&nbsp;— the moment of time in which talk show should happen to make Izabella's rating non-negative before talk show and during period of influence of talk show. If there are multiple answers print smallest of them. If there are no such moments, print <span class="tex-span"> - 1</span>.</p>





```input1
5 1 1 1 4 0 5
1 1
2 1
3 1
4 0
5 0

```




```input2
1 1 2 1 2 1 2
1 0

```




```output1
6
```




```output2
-1
```


