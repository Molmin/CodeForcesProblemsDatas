## Description

<div><p>In the army, it isn't easy to form a group of soldiers that will be effective on the battlefield. The communication is crucial and thus no two soldiers should share a name (what would happen if they got an order that Bob is a scouter, if there are two Bobs?).</p><p>A group of soldiers is effective if and only if their names are different. For example, a group (John, Bob, Limak) would be effective, while groups (Gary, Bob, Gary) and (Alice, Alice) wouldn't.</p><p>You are a spy in the enemy's camp. You noticed <span class="tex-span"><i>n</i></span> soldiers standing in a row, numbered <span class="tex-span">1</span> through <span class="tex-span"><i>n</i></span>. The general wants to choose a group of <span class="tex-span"><i>k</i></span> consecutive soldiers. For every <span class="tex-span"><i>k</i></span> consecutive soldiers, the general wrote down whether they would be an effective group or not.</p><p>You managed to steal the general's notes, with <span class="tex-span"><i>n</i> - <i>k</i> + 1</span> strings <span class="tex-span"><i>s</i><sub class="lower-index">1</sub>, <i>s</i><sub class="lower-index">2</sub>, ..., <i>s</i><sub class="lower-index"><i>n</i> - <i>k</i> + 1</sub></span>, each either "<span class="tex-font-style-tt">YES</span>" or "<span class="tex-font-style-tt">NO</span>". </p><ul> <li> The string <span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span> describes a group of soldiers <span class="tex-span">1</span> through <span class="tex-span"><i>k</i></span> ("<span class="tex-font-style-tt">YES</span>" if the group is effective, and "<span class="tex-font-style-tt">NO</span>" otherwise). </li><li> The string <span class="tex-span"><i>s</i><sub class="lower-index">2</sub></span> describes a group of soldiers <span class="tex-span">2</span> through <span class="tex-span"><i>k</i> + 1</span>. </li><li> And so on, till the string <span class="tex-span"><i>s</i><sub class="lower-index"><i>n</i> - <i>k</i> + 1</sub></span> that describes a group of soldiers <span class="tex-span"><i>n</i> - <i>k</i> + 1</span> through <span class="tex-span"><i>n</i></span>. </li></ul><p>Your task is to find possible names of <span class="tex-span"><i>n</i></span> soldiers. Names should match the stolen notes. Each name should be a string that consists of between <span class="tex-span">1</span> and <span class="tex-span">10</span> English letters, inclusive. The first letter should be uppercase, and all other letters should be lowercase. Names don't have to be existing names&nbsp;— it's allowed to print "<span class="tex-font-style-tt">Xyzzzdj</span>" or "<span class="tex-font-style-tt">T</span>" for example.</p><p>Find and print any solution. It can be proved that there always exists at least one solution.</p></div><div class="input-specification"><p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">2 ≤ <i>k</i> ≤ <i>n</i> ≤ 50</span>)&nbsp;— the number of soldiers and the size of a group respectively.</p><p>The second line contains <span class="tex-span"><i>n</i> - <i>k</i> + 1</span> strings <span class="tex-span"><i>s</i><sub class="lower-index">1</sub>, <i>s</i><sub class="lower-index">2</sub>, ..., <i>s</i><sub class="lower-index"><i>n</i> - <i>k</i> + 1</sub></span>. The string <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> is "<span class="tex-font-style-tt">YES</span>" if the group of soldiers <span class="tex-span"><i>i</i></span> through <span class="tex-span"><i>i</i> + <i>k</i> - 1</span> is effective, and "<span class="tex-font-style-tt">NO</span>" otherwise.</p></div><div class="output-specification"><p>Find any solution satisfying all given conditions. In one line print <span class="tex-span"><i>n</i></span> space-separated strings, denoting possible names of soldiers in the order. The first letter of each name should be uppercase, while the other letters should be lowercase. Each name should contain English letters only and has length from <span class="tex-span">1</span> to <span class="tex-span">10</span>.</p><p>If there are multiple valid solutions, print any of them.</p></div>

## Input

<p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">2 ≤ <i>k</i> ≤ <i>n</i> ≤ 50</span>)&nbsp;— the number of soldiers and the size of a group respectively.</p><p>The second line contains <span class="tex-span"><i>n</i> - <i>k</i> + 1</span> strings <span class="tex-span"><i>s</i><sub class="lower-index">1</sub>, <i>s</i><sub class="lower-index">2</sub>, ..., <i>s</i><sub class="lower-index"><i>n</i> - <i>k</i> + 1</sub></span>. The string <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> is "<span class="tex-font-style-tt">YES</span>" if the group of soldiers <span class="tex-span"><i>i</i></span> through <span class="tex-span"><i>i</i> + <i>k</i> - 1</span> is effective, and "<span class="tex-font-style-tt">NO</span>" otherwise.</p>

## Output

<p>Find any solution satisfying all given conditions. In one line print <span class="tex-span"><i>n</i></span> space-separated strings, denoting possible names of soldiers in the order. The first letter of each name should be uppercase, while the other letters should be lowercase. Each name should contain English letters only and has length from <span class="tex-span">1</span> to <span class="tex-span">10</span>.</p><p>If there are multiple valid solutions, print any of them.</p>





```input1
8 3
NO NO YES YES YES NO

```




```input2
9 8
YES NO

```




```input3
3 2
NO NO

```




```output1
Adam Bob Bob Cpqepqwer Limak Adam Bob Adam
```




```output2
R Q Ccccccccc Ccocc Ccc So Strong Samples Ccc
```




```output3
Na Na Na
```



## Note

<p>In the first sample, there are <span class="tex-span">8</span> soldiers. For every <span class="tex-span">3</span> consecutive ones we know whether they would be an effective group. Let's analyze the provided sample output:</p><ul> <li> First three soldiers (i.e. Adam, Bob, Bob) wouldn't be an effective group because there are two Bobs. Indeed, the string <span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span> is "<span class="tex-font-style-tt">NO</span>". </li><li> Soldiers <span class="tex-span">2</span> through <span class="tex-span">4</span> (Bob, Bob, Cpqepqwer) wouldn't be effective either, and the string <span class="tex-span"><i>s</i><sub class="lower-index">2</sub></span> is "<span class="tex-font-style-tt">NO</span>". </li><li> Soldiers <span class="tex-span">3</span> through <span class="tex-span">5</span> (Bob, Cpqepqwer, Limak) would be effective, and the string <span class="tex-span"><i>s</i><sub class="lower-index">3</sub></span> is "<span class="tex-font-style-tt">YES</span>". </li><li> ..., </li><li> Soldiers <span class="tex-span">6</span> through <span class="tex-span">8</span> (Adam, Bob, Adam) wouldn't be effective, and the string <span class="tex-span"><i>s</i><sub class="lower-index">6</sub></span> is "<span class="tex-font-style-tt">NO</span>". </li></ul>
