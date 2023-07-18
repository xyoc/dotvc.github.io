---
title: "This is a Test post"
date: 2023-07-18T10:00:00-00:00
categories:
  - blog
tags:
  - test
  - update
toc: true
---
标题{#ID3}

##### Header1 {#ID1}

#### Header2 #### {#ID2}

Header3 {#ID3}
-----

脚注{#ID3}
[GoH1](#ID1), [GoH2](#ID2), [GoH3](#ID3)

This is some text.[^1]. 
Other text.[^footnote]. 
Not exist: [^noexist]

[^1]: Some *crazy* footnote definition.

[^footnote]:
    > Blockquotes can be in a footnote.

        as well as code blocks

    or, naturally, simple paragraphs

[^another]: Another test.

链接{#ID3}
[link](http://kramdown.gettalong.org "hp")

Information can be found on the <http://example.com> homepage.
You can also mail me: <me.example@example.com>

A [link][kramdown hp]
to the homepage.

A link to the [kramdown hp].

[kramdown hp]: http://kramdown.gettalong.org "hp"

Table表格{#ID3}

|-----------------+------------+-----------------+----------------|
| Default aligned |Left aligned| Center aligned  | Right aligned  |
|-----------------|:-----------|:---------------:|---------------:|
| First body part |Second cell | Third cell      | fourth cell    |
| Second line     |foo         | **strong**      | baz            |
| Third line      |quux        | baz             | bar            |
|-----------------+------------+-----------------+----------------|
| Second body     |            |                 |                |
| 2 line          |            |                 |                |
|=================+============+=================+================|
| Footer row      |            |                 |                |
|-----------------+------------+-----------------+----------------|

Math{#ID3}

$$
\begin{align*}
  & \phi(x,y) = \phi \left(\sum_{i=1}^n x_ie_i, \sum_{j=1}^n y_je_j \right)
  = \sum_{i=1}^n \sum_{j=1}^n x_i y_j \phi(e_i, e_j) = \\
  & (x_1, \ldots, x_n) \left( \begin{array}{ccc}
      \phi(e_1, e_1) & \cdots & \phi(e_1, e_n) \\
      \vdots & \ddots & \vdots \\
      \phi(e_n, e_1) & \cdots & \phi(e_n, e_n)
    \end{array} \right)
  \left( \begin{array}{c}
      y_1 \\
      \vdots \\
      y_n
    \end{array} \right)
\end{align*}
$$

This is inline $$\sum_{i=1}^n x_ie_i$$

The following is a math block:

$$\sum_{i=1}^n x_ie_i$$

But next comes a paragraph with an inline math statement:

\$$\sum_{i=1}^n x_ie_i$$

List{#ID3}

连续list项

* list item one
* list item two

被分割list项

* list item one

* list item two

EOB的list项

* list item one
^
* list item two

CodeBlock{ID#3}

~~~c#
#kramdown code fenced code block
using System;

namespace Program
{
    class static void Program (args String[])
    {
        Console.WriteLine("hello world");
    }
}
~~~

引用{#ID3}
>此中有真意，欲辩已忘言