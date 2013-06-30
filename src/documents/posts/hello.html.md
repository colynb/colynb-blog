```
title: This is a Hello Blog Post
layout: post
tags: ['intro','post']
type: quote
```

<pre><code class="lang-bash"><div class="highlight"><pre><span class="c"># Install a grunt plugin and save to devDependencies</span>
<span class="k">function </span>gi<span class="o">()</span> <span class="o">{</span>
  npm install --save-dev grunt-<span class="s2">"$@"</span>
<span class="o">}</span>

<span class="c"># Install a grunt-contrib plugin and save to devDependencies</span>
<span class="k">function </span>gci<span class="o">()</span> <span class="o">{</span>
  npm install --save-dev grunt-contrib-<span class="s2">"$@"</span>
<span class="o">}</span>
</pre></div>
</code></pre>