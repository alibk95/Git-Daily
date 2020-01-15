---


---

<h1 id="git---help">Git --help!</h1>
<p><strong>Hi! I’m gonna share my Git experience at work</strong><br>
<em>Target audience: You have a very basic experience with Git</em><br>
<em>Structure: The issues that I had from the very first day and the appropriate solutions</em></p>
<blockquote>
<p><strong>Note:</strong> The solutions here might not be the best way of course.</p>
</blockquote>
<h2 id="how-do-i-create-a-branch">How do I create a branch:</h2>
<p>Whenever I want to start working on a new task of course I need to create a new fresh branch from the master usually. The point is if I’m gonna work on some task on my own then I would create a branch from my personal fork. But if I know that some other colleagues might work on the same issue then it is logical to make branch from the master repo.<br>
Normally I create a branch from the webUI but also the CL commands is possible.<br>
then I would go as follow in the CL:</p>
<blockquote>
<p>git pull<br>
git checkout ''the name of the branch I created"</p>
</blockquote>
<h2 id="what-i-must-do-after-finishing-my-task">What I must do after finishing my task:</h2>
<p>Whenever I finish part of my task I do commit with an appropriate message, short and meaningful.<br>
and I go:</p>
<blockquote>
<p>git commit “appropriate text to this commit”</p>
</blockquote>
<p>after finishing all the task and committing all the related commits(<em>funny sentence!</em>) now I have to push them.<br>
and I go:</p>
<blockquote>
<p>git push</p>
</blockquote>
<p>after pushing all the commits, now from the WebUI (of course could be done from CL) I create a pull request to a person who is in charge of reviewing my code and only after he approves my pull request, I can merge it to the master branch.<br>
The last part which I have to send a pull request is usually happens when you are working in a company and important project and not everybody are permitted to merge something to the master. And another idea behind it which is also decided in our company is that you are not permitted to approve your own pull request. so the process would be as follows:</p>
<blockquote>
<p>I send a pull request ----&gt; my colleague in charge approves —&gt; then I’m allowed to merge</p>
</blockquote>
<p><strong>So the concept and main idea is that, it needs to be always at least two people to merge something to the master branch.</strong></p>
<h2 id="what-if-i-accidentally-worked-wrong-branch">What if I accidentally worked wrong branch:</h2>
<p>let’s make the scenario this way, so that lately I worked on a branch and I forgot to checkout in my new task and I continued working on it for my new task.<br>
In order to save my works, first need to save them in a stack and I go:</p>
<blockquote>
<p>git stash</p>
</blockquote>
<p>then I create a new branch same as I did previously.<br>
then I go:</p>
<blockquote>
<p>git pull<br>
git checkout “the name of the new branch created”<br>
git stash pop</p>
</blockquote>
<p>now I can check my changes with:</p>
<blockquote>
<p>git diff</p>
</blockquote>
<p>so now I have my changes in my new branch without damaging the other branch.<br>
<strong>Note: The ideal way is that after merging a branch to the master then delete it and start working on a new fresh branch</strong></p>
<p>.<br>
.<br>
.<br>
<em>updating daily</em></p>

