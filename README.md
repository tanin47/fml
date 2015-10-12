Fongmun Markup Language
=========================

Fongmun Markup Language (FML) is a simpler variant of [Markdown](https://daringfireball.net/projects/markdown/).

It's safer and more suitable for a discussion board.


Building blocks
----------------

Blocks are separated by 2 new lines (\n). Below are all the possible blocks:

``````
test

1. test
2. test

- test
- test

(three-backticks ```)java
test
(three-backticks ```)

> test
> test
``````

is converted to the HTML below:

```html
<p>test</p>
<ol>
  <li>test</li>
  <li>test</li>
</ol>
<ul>
  <li>test</li>
  <li>test</li>
</ul>
<pre><code class="java">test</code></pre>
<blockquote>test</blockquote>
```

Inlines
---------

Within each block, text can be styled as below:

```
test
____bold____ ___bold___ __bold__ _bold_
****italic**** ***italic*** **italic** **italic**
----strikethrough---- --strikethrough-- --strikethrough-- -strikethrough-
||||underlined|||| |||strikethrough||| ||strikethrough|| |strikethrough|
____***--|combined|--***____
````code```` ```code``` ``code`` `code`
https://twitter.com/tanin/status/576520585708093440
```

is converted to the HTML below:

```html
normal
<strong>bold</strong> <strong>bold</strong> <strong>bold</strong> <strong>bold</strong>
<i>italic</i> <i>italic</i> <i>italic</i> <i>italic</i>
<s>strikethrough</s> <s>strikethrough</s> <s>strikethrough</s> <s>strikethrough</s>
<u>underlined</u> <u>underlined</u> <u>underlined</u> <u>underlined</u>
<strong><i><s><u>combined</u></s></i></strong>
<code class="inline">code</code> <code class="inline">code</code> <code class="inline">code</code> <code class="inline">code</code>
<a href="https://twitter.com/tanin/status/576520585708093440">twitter.com/tanin...</a>
```

Authors
----------

Tanin Na Nakorn [@tanin](http://twitter.com/tanin)

