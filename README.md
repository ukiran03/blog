
# Table of Contents

1.  [Headlines](#org2e61735)
    1.  [Second level](#orgfd961d6)
        1.  [Third level](#orga1142b5)
2.  [Task Lists <code>[1/3]</code>](#orgac1f2ce)
3.  [List Bullets](#orgc39018e)
4.  [Timestamps](#orgf51c887):example:
5.  [Blocks](#orgb6fd33e)
6.  [Todo Labels and Tags](#orgcd2d6b6)
    1.  [Write `org-modern`](#org558dada):emacs:foss:coding:
    2.  [Publish `org-modern`](#org9b6ef13)
    3.  [Fix all the bugs](#orgbbb9ded)
7.  [Priorities](#orge832671)
    1.  [Most important](#org570c7a3)
    2.  [Less important](#orgc0242da)
    3.  [Not that important](#orgfa6984b)
    4.  [<code>[100%]</code> [#A] Everything combined](#orgcf66de9):tag:test:
8.  [Tables](#org5293a23)
9.  [Special Links](#org2521e6d)
10. [Progress bars](#org7987862)
11. [2.7 Drawers](#orge90cb4c)
    1.  [sdfdf](#org0df55e8)
        1.  [sdfsdf](#orgb1a0e5a)
12. [4 HyperLinks](#orge1afc28)
13. [5 TODO Items](#orgbba3f8a)
    1.  [An Important task](#org1113510)
    2.  [parent](#org302ca6a)
        1.  [a](#orgf9fd5a9)
        2.  [b](#org9cc20c0)
        3.  [c](#orgfc51876)

This example Org file demonstrates the Org elements,
which are styled by `org-modern`.

---


<a id="org2e61735"></a>

# Headlines


<a id="orgfd961d6"></a>

## Second level


<a id="orga1142b5"></a>

### Third level

1.  Fourth level

    1.  Fifth level


<a id="orgac1f2ce"></a>

# Task Lists <code>[1/3]</code>

-   [X] Write `org-modern`
-   [-] Publish `org-modern`
-   [ ] Fix all the bugs


<a id="orgc39018e"></a>

# List Bullets

-   Dash
    -   Plus
        -   Asterisk
-   **description:** list one
-   **sfsdf:** list two


<a id="orgf51c887"></a>

# Timestamps     :example:

SCHEDULED: <span class="timestamp-wrapper"><span class="timestamp">&lt;2022-02-25 Fri 10:00&gt;</span></span>
DRANGE:    <span class="timestamp-wrapper"><span class="timestamp">[2022-03-01 Tue]&#x2013;[2022-04-01 Fri]</span></span>
DRANGE:    <span class="timestamp-wrapper"><span class="timestamp">&lt;2022-03-01 Tue&gt;&#x2013;&lt;2022-04-01 Fri&gt;</span></span>
TRANGE:    <span class="timestamp-wrapper"><span class="timestamp">[2022-03-01 Tue 10:42]&#x2013;[2022-03-01 Tue 11:00]</span></span>
TIMESTAMP: <span class="timestamp-wrapper"><span class="timestamp">[2022-02-21 Mon 13:00]</span></span>
DREPEATED: <span class="timestamp-wrapper"><span class="timestamp">&lt;2022-02-26 Sat .+1d&gt;</span></span>
TREPEATED: <span class="timestamp-wrapper"><span class="timestamp">&lt;2022-02-26 Sat 10:00 .+1d&gt;</span></span>


<a id="orgb6fd33e"></a>

# Blocks

    ;; Taken from the well-structured Emacs config by @oantolin.
    ;; Take a look at https://github.com/oantolin/emacs-config!
    (defun command-of-the-day ()
      "Show the documentation for a random command."
      (interactive)
      (let ((commands))
        (mapatoms (lambda (s)
                    (when (commandp s) (push s commands))))
        (describe-function
         (nth (random (length commands)) commands))))

    taylor(sin(x),x=0,3)

    printf("a|b\nc|d\n");

    (define three
      (+ 1 2))


<a id="orgcd2d6b6"></a>

# Todo Labels and Tags


<a id="org558dada"></a>

## DONE Write `org-modern`     :emacs:foss:coding:


<a id="org9b6ef13"></a>

## TODO Publish `org-modern`


<a id="orgbbb9ded"></a>

## WAIT Fix all the bugs


<a id="orge832671"></a>

# Priorities


<a id="org570c7a3"></a>

## DONE Most important


<a id="orgc0242da"></a>

## TODO Less important


<a id="orgfa6984b"></a>

## CANCEL Not that important


<a id="orgcf66de9"></a>

## DONE <code>[100%]</code> [#A] Everything combined     :tag:test:

-   [X] First
-   [X] Second
-   [X] Third


<a id="org5293a23"></a>

# Tables

<table border="2" cellspacing="0" cellpadding="6" rules="groups" frame="hsides">


<colgroup>
<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />
</colgroup>
<thead>
<tr>
<th scope="col" class="org-right">N</th>
<th scope="col" class="org-right">N<sup>2</sup></th>
<th scope="col" class="org-right">N<sup>3</sup></th>
<th scope="col" class="org-right">N<sup>4</sup></th>
<th scope="col" class="org-right">sqrt(n)</th>
<th scope="col" class="org-right">sqrt[4](N)</th>
</tr>
</thead>

<tbody>
<tr>
<td class="org-right">2</td>
<td class="org-right">4</td>
<td class="org-right">8</td>
<td class="org-right">16</td>
<td class="org-right">1.4142</td>
<td class="org-right">1.1892</td>
</tr>


<tr>
<td class="org-right">3</td>
<td class="org-right">9</td>
<td class="org-right">27</td>
<td class="org-right">81</td>
<td class="org-right">1.7321</td>
<td class="org-right">1.3161</td>
</tr>
</tbody>
</table>

<table border="2" cellspacing="0" cellpadding="6" rules="groups" frame="hsides">


<colgroup>
<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />
</colgroup>
<thead>
<tr>
<th scope="col" class="org-right">N</th>
<th scope="col" class="org-right">N<sup>2</sup></th>
<th scope="col" class="org-right">N<sup>3</sup></th>
<th scope="col" class="org-right">N<sup>4</sup></th>
<th scope="col" class="org-right">sqrt(n)</th>
<th scope="col" class="org-right">sqrt[4](N)</th>
</tr>
</thead>

<tbody>
<tr>
<td class="org-right">2</td>
<td class="org-right">4</td>
<td class="org-right">8</td>
<td class="org-right">16</td>
<td class="org-right">1.4142</td>
<td class="org-right">1.1892</td>
</tr>


<tr>
<td class="org-right">3</td>
<td class="org-right">9</td>
<td class="org-right">27</td>
<td class="org-right">81</td>
<td class="org-right">1.7321</td>
<td class="org-right">1.3161</td>
</tr>
</tbody>
</table>

    | a | b | c |
    | a | b | c |
    | a | b | c |


<a id="org2521e6d"></a>

# Special Links

Test numeric footnotes<sup><a id="fnr.1" class="footref" href="#fn.1" role="doc-backlink">1</a></sup> and named footnotes<sup><a id="fnr.2" class="footref" href="#fn.2" role="doc-backlink">2</a></sup>.

<a id="org58ec4e3"></a>

<a id="org8cf4dd8">radio link</a>

[9](#org58ec4e3)

<a href="#org8cf4dd8">radio link</a>


<a id="org7987862"></a>

# Progress bars

-   quotient <code>[1/13]</code>
-   quotient <code>[12/13]</code>
-   quotient <code>[13/13]</code>

-   percent <code>[10%]</code>
-   percent <code>[90%]</code>
-   percent <code>[100%]</code>

-   overflow <code>[110%]</code>
-   overflow <code>[20/10]</code>


<a id="orge90cb4c"></a>

# 2.7 Drawers


<a id="org0df55e8"></a>

## sdfdf


<a id="orgb1a0e5a"></a>

### sdfsdf

`C-c C-x d` `> org-insert-drawer
=C-u C-c C-x d` => org-insert-property-drawer


<a id="orge1afc28"></a>

# 4 HyperLinks

[A link with C-c C-l](#orge1afc28)
<org-man-test.md>
<file:///home/ukiran/org-man-test.md>

    (setq org-return-follows-link t) ;; <RET> will follows the link


<a id="orgbba3f8a"></a>

# 5 TODO Items


<a id="org1113510"></a>

## TODO An Important task


<a id="org302ca6a"></a>

## parent


<a id="orgf9fd5a9"></a>

### TODO a


<a id="org9cc20c0"></a>

### TODO b


<a id="orgfc51876"></a>

### TODO c


# Footnotes

<sup><a id="fn.1" href="#fnr.1">1</a></sup> This is footnote 1

<sup><a id="fn.2" href="#fnr.2">2</a></sup> This is the foonote
