## Description

<div><p>Surely you have seen insane videos by South Korean rapper PSY, such as "Gangnam Style", "Gentleman" and "Daddy". You might also hear that PSY has been recording video "Oppa Funcan Style" two years ago (unfortunately we couldn't find it on the internet). We will remind you what this hit looked like (you can find original description <a href="http://acm.timus.ru/problem.aspx?space=1&amp;num=2107&amp;locale=en">here</a>):</p><p>On the ground there are $n$ platforms, which are numbered with integers from $1$ to $n$, on $i$-th platform there is a dancer with number $i$. Further, every second all the dancers standing on the platform with number $i$ jump to the platform with the number $f(i)$. The moving rule $f$ is selected in advance and is not changed throughout the clip.</p><p>The duration of the clip was $k$ seconds and the rule $f$ was chosen in such a way that after $k$ seconds all dancers were in their initial positions (i.e. the $i$-th dancer stood on the platform with the number $i$). That allowed to loop the clip and collect even more likes.</p><p>PSY knows that enhanced versions of old artworks become more and more popular every day. So he decided to release a remastered-version of his video.</p><p>In his case "enhanced version" means even more insanity, so the number of platforms can be up to $10^{18}$! But the video director said that if some dancer stays on the same platform all the time, then the viewer will get bored and will turn off the video immediately. Therefore, for all $x$ from $1$ to $n$ $f(x) \neq x$ must hold.</p><p>Big part of classic video's success was in that looping, so in the remastered version all dancers should return to their initial positions in the end of the clip as well.</p><p>PSY hasn't decided on the exact number of platforms and video duration yet, so he asks you to check if there is a good rule $f$ for different options.</p></div><div class="input-specification"><p>In the first line of input there is one integer $t$ ($1 \le t \le 10^{4}$)&nbsp;— the number of options for $n$ and $k$ to check.</p><p>In the next $t$ lines the options are given: each option is described with two integers $n$ and $k$ ($1 \le n \le 10^{18}$, $1 \le k \le 10^{15}$)&nbsp;— the number of dancers and the duration in seconds.</p><p><span class="tex-font-style-bf">It is guaranteed that the number of different values of $k$ in one test is not greater than $50$.</span></p></div><div class="output-specification"><p>Print $t$ lines. If the $i$-th option of the video is feasible, print "<span class="tex-font-style-tt">YES</span>" (without quotes) in $i$-th line, otherwise print "<span class="tex-font-style-tt">NO</span>" (without quotes).</p></div>

## Input

<p>In the first line of input there is one integer $t$ ($1 \le t \le 10^{4}$)&nbsp;— the number of options for $n$ and $k$ to check.</p><p>In the next $t$ lines the options are given: each option is described with two integers $n$ and $k$ ($1 \le n \le 10^{18}$, $1 \le k \le 10^{15}$)&nbsp;— the number of dancers and the duration in seconds.</p><p><span class="tex-font-style-bf">It is guaranteed that the number of different values of $k$ in one test is not greater than $50$.</span></p>

## Output

<p>Print $t$ lines. If the $i$-th option of the video is feasible, print "<span class="tex-font-style-tt">YES</span>" (without quotes) in $i$-th line, otherwise print "<span class="tex-font-style-tt">NO</span>" (without quotes).</p>





```input1
3
7 7
3 8
5 6

```




```output1
YES
NO
YES

```


