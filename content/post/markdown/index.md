---
title: Markdown Reference Guide
tags: [markup]
categories: [Informatics]
katex: math
math: true
date: 2022-03-06 00:00:00+0000
image: cover.jpg
---

Markdown Reference Guide
===========

I am a paragraph in markdown with line
wrapping so fit in this width.
I am a continuation of the first paragraph
as there is no empty line before me.

I am in the second paragraph.


I am the third one. Even though there are
two line breaks before me, this does not
create any newline characters. After me there
are two spaces before the newline character.  
I have a line break before me. Even though
I am not a new paragraph, I do start on a
new line due to the manual line break via
spaces before the newline character.

Top Level H1
=============
H2
---

#Just a tag
\# Not a heading
Also a # tag.
# Alternate H1
## Alternate H2
### H3
###### H6

* This is a list element
+ This is also a list element
- This is also a list element
     - This is a sublist element
     + Also a sublist element
       + Sublist level 2
       1. Numbered sublist
       2. Next item
             1. Next indent level

1) Numbered list
2) Next item
     1. Next indent level
        * Sublist non numbered
3. Back

Horizontal Lines:

------------------------------------
.
***********************************
.
***
.

---

> Block Quote

    Preformatted text

## Inline formatting

*Italics*

_Italics_

__Bold__

__*Bold+Italics*__

**_Bold+Italics_**

this_is_not_emphasis

~~Strike-through~~

Content with a -- (dash) and a --- (long dash).

[link](http://link/path/to/target)

[link](http://link/path/to/target "TITLE ON LINK")

[Shared links with footnotes][target 1]

[Second shared link][target 1]

[target 1]

[target 1]: http://footnote.com

Sample inline code `a++` can be specified here.

![Alt Text](/path/to/image "Optional Tooltip")


## HTML escaped characters and inline HTML

Copyright: &copy;

Registered: &reg;

Trademark: &trade;

Less Than: &lt;

Greater Than: &gt;

Ampersand: &amp;

Smiley: &#x1F604;

Embedded HTML: x<sup>2</sup>

Floating image via HTML: <img src="/image/logo.png" style="float: right; padding: 0 0 0 10px"> Follow up text after the image. This honors the floats and wraps around the image, automatically going into the next line.

## Tables, code blocks and task lists

   Name | Job
--------|------
   Alex | Web Developer
    Bob | Sys Admin
   Gabby| Technical Writer


### Alternate table


|  Name | Mantra |
|  ---  | --- |
| Alex  | There must be a better way. |
| Bob   | Play it safe. |
| Gabby | Try everything, but do what you like. |

### Table alignment

| Index |  Product | Edges |
| --:   |  :--  | :-: |
| 1.  | Circle  | 0 |
| 2.  | Line   | 1 |
| 3.  | Square | 4 |

## Acme website task list

- [x] Get the home page up
- [x] Update Privacy Policy and Terms of Use
- [ ] Add the about page
- [ ] Start the blog
- [ ] Enable contact us

## Code block

```javascript
var x= 10;
x++;
console.log(x);
```

With highlighting:

```javascript {linenos=true,hl_lines=[2,"4-6"],linenostart=199}
while (!success) {
  tryAgain();
  attempt++;
  if (Dead) {
    break;
  }
}
```

## Direct Emojis
Smile please :smile:

I :heart: Hugo

Wink :wink:

A link to [Emojis](#direct-emojis)

## Smart conversion

This will convert to a dash --

This is followed by ellipses ...

## This is extra highlighted{style="background: yellow"}


## Definition Lists

Alex
: Hippy Web Developer
: Technophile

Bob
: Classic SysAdmin
: Conservative

Gabby
: Cool Content Master
: Cautious

## Shortcodes

*Youtube*
{{< youtube nLAVanlu5js >}}


*Highlight*
{{< highlight js "linenos=table,hl_lines=3-4,linenostart=1080" >}}
// Enjoy your work
if (!tired()) {
    keepCoding();
} else {
    drinkCoffee();
}
{{</ highlight >}}

{{< highlight html "linenos=table,hl_lines=2 ,linenostart=1080" >}}
<!-- Generated Youtube source code for video -->
{{</* youtube nLAVanlu5js */>}}
<!-- Output -->
{{< youtube nLAVanlu5js >}}
{{</ highlight >}}


## Inline shortcodes.

### Inline Shortcode declaration and first use
{{% reuse.inline %}}A programmer's wife sends him to the grocery with instructions: **Get a loaf of bread and if they have eggs, get a dozen**. He came back with a dozen loafs of bread: **They had eggs.**
{{% /reuse.inline %}}

### Shortcode usage as HTML
{{< reuse.inline />}}

### Shortcode usage as Markup
{{% reuse.inline /%}}


## Math

You start and end math using dollar signs. If you use on, you get inline
math, and if you use two, you get "display" math, which means you get the math
on a single line and centered.

This is inline math: $\int_a^b x\,\mathrm{d}x$.

This is display math: 
$$\sum_{j=1}^N \frac{1}{j^2}$$

Pandoc supports a large subset of math you can write in LaTeX.
For example, here is more complex equation.
$$
d(i,j) = \begin{cases}
\,i & j = 0 \\
\,j & i = 0 \\
\,\min\begin{cases}
    d(i-1,j-1) + \mathrm{1}(i\neq j) \\
    d(i,j-1) + 1 \\
    d(i-1,j) + 1
\end{cases} & i>0,j>0
\end{cases}
$$

Photo by [Super Snapper](https://unsplash.com/@supersnapper27?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText) on [Unsplash](https://unsplash.com/s/photos/writing?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText)