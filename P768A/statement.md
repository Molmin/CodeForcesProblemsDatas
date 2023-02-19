## Description

<div><p><span class="tex-font-style-it">"Night gathers, and now my watch begins. It shall not end until my death. I shall take no wife, hold no lands, father no children. I shall wear no crowns and win no glory. I shall live and die at my post. I am the sword in the darkness. I am the watcher on the walls. I am the shield that guards the realms of men. I pledge my life and honor to the Night's Watch, for this night and all the nights to come."</span> — The Night's Watch oath.</p><p>With that begins the watch of Jon Snow. He is assigned the task to support the stewards.</p><p>This time he has <span class="tex-span"><i>n</i></span> stewards with him whom he has to provide support. Each steward has his own strength. Jon Snow likes to support a steward only if there exists at least one steward who has strength strictly less than him and at least one steward who has strength strictly greater than him.</p><p>Can you find how many stewards will Jon support?</p></div><div class="input-specification"><p>First line consists of a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of stewards with Jon Snow.</p><p>Second line consists of <span class="tex-span"><i>n</i></span> space separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) representing the values assigned to the stewards.</p></div><div class="output-specification"><p>Output a single integer representing the number of stewards which Jon will feed.</p></div>

## Input

<p>First line consists of a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of stewards with Jon Snow.</p><p>Second line consists of <span class="tex-span"><i>n</i></span> space separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) representing the values assigned to the stewards.</p>

## Output

<p>Output a single integer representing the number of stewards which Jon will feed.</p>





```input1
2
1 5

```




```input2
3
1 2 5

```




```output1
0
```




```output2
1
```



## Note

<p>In the first sample, Jon Snow cannot support steward with strength <span class="tex-span">1</span> because there is no steward with strength less than <span class="tex-span">1</span> and he cannot support steward with strength <span class="tex-span">5</span> because there is no steward with strength greater than <span class="tex-span">5</span>.</p><p>In the second sample, Jon Snow can support steward with strength <span class="tex-span">2</span> because there are stewards with strength less than <span class="tex-span">2</span> and greater than <span class="tex-span">2</span>.</p>
