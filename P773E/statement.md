## Description

<div><p>It's well-known that blog posts are an important part of Codeforces platform. Every blog post has a global characteristic changing over time&nbsp;— its <span class="tex-font-style-underline">community rating</span>. A newly created blog post's community rating is 0. Codeforces users may visit the blog post page and rate it, changing its community rating by +1 or -1.</p><p>Consider the following model of Codeforces users' behavior. The <span class="tex-span"><i>i</i></span>-th user has his own <span class="tex-font-style-underline">estimated blog post rating</span> denoted by an integer <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>. When a user visits a blog post page, he compares his estimated blog post rating to its community rating. If his estimated rating is higher, he rates the blog post with +1 (thus, the blog post's community rating increases by 1). If his estimated rating is lower, he rates the blog post with -1 (decreasing its community rating by 1). If the estimated rating and the community rating are equal, user doesn't rate the blog post at all (in this case we'll say that user rates the blog post for 0). In any case, after this procedure user closes the blog post page and never opens it again.</p><p>Consider a newly created blog post with the initial community rating of 0. For each of <span class="tex-span"><i>n</i></span> Codeforces users, numbered from 1 to <span class="tex-span"><i>n</i></span>, his estimated blog post rating <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is known.</p><p>For each <span class="tex-span"><i>k</i></span> from 1 to <span class="tex-span"><i>n</i></span>, inclusive, the following question is asked. Let users with indices from 1 to <span class="tex-span"><i>k</i></span>, <span class="tex-font-style-bf">in some order</span>, visit the blog post page, rate the blog post and close the page. Each user opens the blog post only after the previous user closes it. What could be the maximum possible community rating of the blog post after these <span class="tex-span"><i>k</i></span> visits?</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5·10<sup class="upper-index">5</sup></span>)&nbsp;— the number of Codeforces users.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"> - 5·10<sup class="upper-index">5</sup> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 5·10<sup class="upper-index">5</sup></span>)&nbsp;— estimated blog post ratings for users in order from 1 to <span class="tex-span"><i>n</i></span>.</p></div><div class="output-specification"><p>For each <span class="tex-span"><i>k</i></span> from 1 to <span class="tex-span"><i>n</i></span>, output a single integer equal to the maximum possible community rating of the blog post after users with indices from 1 to <span class="tex-span"><i>k</i></span>, in some order, visit the blog post page, rate the blog post, and close the page.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5·10<sup class="upper-index">5</sup></span>)&nbsp;— the number of Codeforces users.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"> - 5·10<sup class="upper-index">5</sup> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 5·10<sup class="upper-index">5</sup></span>)&nbsp;— estimated blog post ratings for users in order from 1 to <span class="tex-span"><i>n</i></span>.</p>

## Output

<p>For each <span class="tex-span"><i>k</i></span> from 1 to <span class="tex-span"><i>n</i></span>, output a single integer equal to the maximum possible community rating of the blog post after users with indices from 1 to <span class="tex-span"><i>k</i></span>, in some order, visit the blog post page, rate the blog post, and close the page.</p>





```input1
4
2 0 2 2

```




```input2
7
2 -3 -2 5 0 -3 1

```




```output1
1
1
2
2

```




```output2
1
0
-1
0
1
1
2

```


