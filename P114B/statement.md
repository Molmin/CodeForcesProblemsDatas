## Description

<div><p>When little Petya grew up and entered the university, he started to take part in АСМ contests. Later he realized that he doesn't like how the АСМ contests are organised: the team could only have three members (and he couldn't take all his friends to the competitions and distribute the tasks between the team members efficiently), so he decided to organize his own contests PFAST Inc. — Petr and Friends Are Solving Tasks Corporation. PFAST Inc. rules allow a team to have unlimited number of members.</p><p>To make this format of contests popular he organised his own tournament. To create the team he will prepare for the contest organised by the PFAST Inc. rules, he chose several volunteers (up to 16 people) and decided to compile a team from them. Petya understands perfectly that if a team has two people that don't get on well, then the team will perform poorly. Put together a team with as many players as possible given that all players should get on well with each other.</p></div><div class="input-specification"><p>The first line contains two integer numbers <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 16</span>) — the number of volunteers, and <span class="tex-span"><i>m</i></span> (<img align="middle" class="tex-formula" src="file://U27SVAa4.png" style="max-width: 100.0%;max-height: 100.0%;">) — the number of pairs that do not get on. Next <span class="tex-span"><i>n</i></span> lines contain the volunteers' names (each name is a non-empty string consisting of no more than 10 uppercase and/or lowercase Latin letters). Next <span class="tex-span"><i>m</i></span> lines contain two names — the names of the volunteers who do not get on. The names in pair are separated with a single space. Each pair of volunteers who do not get on occurs exactly once. The strings are case-sensitive. All <span class="tex-span"><i>n</i></span> names are distinct.</p></div><div class="output-specification"><p>The first output line should contain the single number <span class="tex-span"><i>k</i></span> — the number of people in the sought team. Next <span class="tex-span"><i>k</i></span> lines should contain the names of the sought team's participants in the lexicographical order. If there are several variants to solve the problem, print any of them. Petya might not be a member of the sought team. </p></div>

## Input

<p>The first line contains two integer numbers <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 16</span>) — the number of volunteers, and <span class="tex-span"><i>m</i></span> (<img align="middle" class="tex-formula" src="file://U27SVAa4.png" style="max-width: 100.0%;max-height: 100.0%;">) — the number of pairs that do not get on. Next <span class="tex-span"><i>n</i></span> lines contain the volunteers' names (each name is a non-empty string consisting of no more than 10 uppercase and/or lowercase Latin letters). Next <span class="tex-span"><i>m</i></span> lines contain two names — the names of the volunteers who do not get on. The names in pair are separated with a single space. Each pair of volunteers who do not get on occurs exactly once. The strings are case-sensitive. All <span class="tex-span"><i>n</i></span> names are distinct.</p>

## Output

<p>The first output line should contain the single number <span class="tex-span"><i>k</i></span> — the number of people in the sought team. Next <span class="tex-span"><i>k</i></span> lines should contain the names of the sought team's participants in the lexicographical order. If there are several variants to solve the problem, print any of them. Petya might not be a member of the sought team. </p>





```input1
3 1
Petya
Vasya
Masha
Petya Vasya

```




```input2
3 0
Pasha
Lesha
Vanya

```




```output1
2
Masha
Petya

```




```output2
3
Lesha
Pasha
Vanya

```


