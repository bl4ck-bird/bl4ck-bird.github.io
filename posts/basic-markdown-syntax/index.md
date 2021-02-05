# Basic Markdown Syntax


Sample of basic markdown syntax

<!--more-->

## Headings

```markdown
## h2 Heading
### h3 Heading
#### h4 Heading
##### h5 Heading
###### h6 Heading
### Heading Custom ID {#custom-id}
```

```html
<h2>h2 Heading</h2>
<h3>h3 Heading</h3>
<h4>h4 Heading</h4>
<h5>h5 Heading</h5>
<h6>h6 Heading</h6>
<h3 id="custom-id">Heading Custom ID</h3>
```

## Comments {#comment}

```markdown
<!--
This is a comment
-->
```

```html

```

## Horizontal Rules

```markdown
---
___
***
```

```html
<hr>
<hr>
<hr>
```

{{< admonition type=abstract title="Rendered" >}}
---
{{</ admonition >}}

## Paragraph

```markdown
Lorem ipsum dolor sit amet, graecis denique ei vel, at duo primis mandamus. Et legere ocurreret pri,
animal tacimates complectitur ad cum. Cu eum inermis inimicus efficiendi. Labore officiis his ex,
soluta officiis concludaturque ei qui, vide sensibus vim ad.

Lorem ipsum dolor sit amet, graecis denique ei vel, at duo primis mandamus. Et legere ocurreret pri,
animal tacimates complectitur ad cum. Cu eum inermis inimicus efficiendi. Labore officiis his ex,
soluta officiis concludaturque ei qui, vide sensibus vim ad.
```

```html
<p>Lorem ipsum dolor sit amet, graecis denique ei vel, at duo primis mandamus. Et legere ocurreret pri,
animal tacimates complectitur ad cum. Cu eum inermis inimicus efficiendi. Labore officiis his ex,
soluta officiis concludaturque ei qui, vide sensibus vim ad.</p>
<p>Lorem ipsum dolor sit amet, graecis denique ei vel, at duo primis mandamus. Et legere ocurreret pri,
animal tacimates complectitur ad cum. Cu eum inermis inimicus efficiendi. Labore officiis his ex,
soluta officiis concludaturque ei qui, vide sensibus vim ad.</p>
```

{{< admonition type=abstract title="Rendered" >}}
Lorem ipsum dolor sit amet, graecis denique ei vel, at duo primis mandamus. Et legere ocurreret pri,
animal tacimates complectitur ad cum. Cu eum inermis inimicus efficiendi. Labore officiis his ex,
soluta officiis concludaturque ei qui, vide sensibus vim ad.
{{</ admonition >}}

## Inline HTML

```markdown
Paragraph in Markdown.

<div class="class">
    This is <b>HTML</b>
</div>

Paragraph in Markdown.
```

```html
<p>Paragraph in Markdown.</p>
<div class="class">
    This is <b>HTML</b>
</div>
<p>Paragraph in Markdown.</p>
```

{{< admonition type=abstract title="Rendered" >}}
Paragraph in Markdown.

<div class="class">
    This is <b>HTML</b>
</div>

Paragraph in Markdown.
{{</ admonition >}}

## Emphasis

### Bold

```markdown
**rendered as bold text**
__rendered as bold text__
```

```html
<strong>rendered as bold text</strong>
```

{{< admonition type=abstract title="Rendered" >}}
**rendered as bold text**
{{</ admonition >}}

### Italics

```markdown
*rendered as italicized text*
_rendered as italicized text_
```

```html
<em>rendered as italicized text</em>
```

{{< admonition type=abstract title="Rendered" >}}
*rendered as italicized text*
{{</ admonition >}}

### Strikethrough

```markdown
~~Strike through this text.~~
```

```html
<del>Strike through this text.</del>
```

{{< admonition type=abstract title="Rendered" >}}
~~Strike through this text.~~
{{</ admonition >}}

### Combination

```markdown
***bold and italics***
~~**strikethrough and bold**~~
~~*strikethrough and italics*~~
~~***bold, italics and strikethrough***~~
```

```html
<em><strong>bold and italics</strong></em>
<del><strong>strikethrough and bold</strong></del>
<del><em>strikethrough and italics</em></del>
<del><em><strong>bold, italics and strikethrough</strong></em></del>
```

{{< admonition type=abstract title="Rendered" >}}
***bold and italics***

~~**strikethrough and bold**~~

~~*strikethrough and italics*~~

~~***bold, italics and strikethrough***~~
{{</ admonition >}}

## Blockquotes

```markdown
> **Fusion Drive** combines a hard drive with a flash storage (solid-state drive) and presents it as a single logical volume with the space of both drives combined.

> Donec massa lacus, ultricies a ullamcorper in, fermentum sed augue.
Nunc augue augue, aliquam non hendrerit ac, commodo vel nisi.
>> Sed adipiscing elit vitae augue consectetur a gravida nunc vehicula. Donec auctor
odio non est accumsan facilisis. Aliquam id turpis in dolor tincidunt mollis ac eu diam.
```

```html
<blockquote>
    <p><strong>Fusion Drive</strong> combines a hard drive with a flash storage (solid-state drive) and presents it as a single logical volume with the space of both drives combined.</p>
</blockquote>

<blockquote>
    <p>Donec massa lacus, ultricies a ullamcorper in, fermentum sed augue.
    Nunc augue augue, aliquam non hendrerit ac, commodo vel nisi.</p>
    <blockquote>
        <p>Sed adipiscing elit vitae augue consectetur a gravida nunc vehicula. Donec auctor
        odio non est accumsan facilisis. Aliquam id turpis in dolor tincidunt mollis ac eu diam.</p>
    </blockquote>
</blockquote>
```

{{< admonition type=abstract title="Rendered" >}}
> **Fusion Drive** combines a hard drive with a flash storage (solid-state drive) and presents it as a single logical volume with the space of both drives combined.

> Donec massa lacus, ultricies a ullamcorper in, fermentum sed augue.
Nunc augue augue, aliquam non hendrerit ac, commodo vel nisi.
>> Sed adipiscing elit vitae augue consectetur a gravida nunc vehicula. Donec auctor
odio non est accumsan facilisis. Aliquam id turpis in dolor tincidunt mollis ac eu diam.
{{</ admonition >}}

## Lists

### Unordered

```markdown
* Lorem ipsum dolor sit amet
* Consectetur adipiscing elit
* Integer molestie lorem at massa
* Facilisis in pretium nisl aliquet
* Nulla volutpat aliquam velit
    * Phasellus iaculis neque
    * Purus sodales ultricies
    * Vestibulum laoreet porttitor sem
    * Ac tristique libero volutpat at
* Faucibus porta lacus fringilla vel
* Aenean sit amet erat nunc
* Eget porttitor lorem
```

```html
<ul>
    <li>Lorem ipsum dolor sit amet</li>
    <li>Consectetur adipiscing elit</li>
    <li>Integer molestie lorem at massa</li>
    <li>Facilisis in pretium nisl aliquet</li>
    <li>Nulla volutpat aliquam velit
        <ul>
            <li>Phasellus iaculis neque</li>
            <li>Purus sodales ultricies</li>
            <li>Vestibulum laoreet porttitor sem</li>
            <li>Ac tristique libero volutpat at</li>
        </ul>
    </li>
    <li>Faucibus porta lacus fringilla vel</li>
    <li>Aenean sit amet erat nunc</li>
    <li>Eget porttitor lorem</li>
</ul>
```

{{< admonition type=abstract title="Rendered" >}}
* Lorem ipsum dolor sit amet
* Consectetur adipiscing elit
* Integer molestie lorem at massa
* Facilisis in pretium nisl aliquet
* Nulla volutpat aliquam velit
    * Phasellus iaculis neque
    * Purus sodales ultricies
    * Vestibulum laoreet porttitor sem
    * Ac tristique libero volutpat at
* Faucibus porta lacus fringilla vel
* Aenean sit amet erat nunc
* Eget porttitor lorem
{{</ admonition >}}

### Ordered

```markdown
1. Lorem ipsum dolor sit amet
2. Consectetur adipiscing elit
3. Integer molestie lorem at massa
    1. Facilisis in pretium nisl aliquet
    1. Nulla volutpat aliquam velit
    1. Faucibus porta lacus fringilla vel
7. Aenean sit amet erat nunc
1. Eget porttitor lorem
```

```html
<ol>
    <li>Lorem ipsum dolor sit amet</li>
    <li>Consectetur adipiscing elit</li>
    <li>Integer molestie lorem at massa
        <ol>
            <li>Facilisis in pretium nisl aliquet</li>
            <li>Nulla volutpat aliquam velit</li>
            <li>Faucibus porta lacus fringilla vel</li>
        </ol>
    </li>
    <li>Aenean sit amet erat nunc</li>
    <li>Eget porttitor lorem</li>
</ol>
```

{{< admonition type=abstract title="Rendered" >}}
1. Lorem ipsum dolor sit amet
2. Consectetur adipiscing elit
3. Integer molestie lorem at massa
    1. Facilisis in pretium nisl aliquet
    1. Nulla volutpat aliquam velit
    1. Faucibus porta lacus fringilla vel
7. Aenean sit amet erat nunc
1. Eget porttitor lorem
{{</ admonition >}}

## Task Lists

```markdown
- [x] Write the press release
- [ ] Update the website
- [ ] Contact the media
```

```html
<ul>
    <li><input type="checkbox" disabled checked> Write the press release</li>
    <li><input type="checkbox" disabled> Update the website</li>
    <li><input type="checkbox" disabled> Contact the media</li>
</ul>
```

{{< admonition type=abstract title="Rendered" >}}
- [x] Write the press release
- [ ] Update the website
- [ ] Contact the media
{{</ admonition >}}

## Code

### Inline Code

```markdown
In this example, `<section></section>` should be wrapped as **code**.
```

```html
<p>In this example, <code>&lt;section&gt;&lt;/section&gt;</code> should be wrapped as <strong>code</strong>.</p>
```

{{< admonition type=abstract title="Rendered" >}}
In this example, `<section></section>` should be wrapped as **code**.
{{</ admonition >}}

### Indented Code

```markdown
    // Some comments
    line 1 of code
    line 2 of code
    line 3 of code
```

```html
<pre>
    <code>
        // Some comments
        line 1 of code
        line 2 of code
        line 3 of code
    </code>
</pre>
```

{{< admonition type=abstract title="Rendered" >}}
    // Some comments
    line 1 of code
    line 2 of code
    line 3 of code
{{</ admonition >}}

### Block Fenced Code

{{< highlight markdown >}}
```
Sample text here...
```
{{</ highlight >}}

```html
<pre>
  <code>Sample text here...</code>
</pre>
```

{{< admonition type=abstract title="Rendered" >}}
```
Sample text here...
```
{{</ admonition >}}

### Syntax Highlighting

{{< highlight markdown >}}
```js
grunt.initConfig({
    assemble: {
        options: {
            assets: 'docs/assets',
            data: 'src/data/*.{json,yml}',
            helpers: 'src/custom-helpers.js',
            partials: ['src/partials/**/*.{hbs,md}']
        },
        pages: {
            options: {
                layout: 'default.hbs'
            },
            files: {
                './': ['src/templates/pages/index.hbs']
            }
        }
    }
};
```
{{</ highlight >}}

{{< admonition type=abstract title="Rendered" >}}
```js
grunt.initConfig({
    assemble: {
        options: {
            assets: 'docs/assets',
            data: 'src/data/*.{json,yml}',
            helpers: 'src/custom-helpers.js',
            partials: ['src/partials/**/*.{hbs,md}']
        },
        pages: {
            options: {
                layout: 'default.hbs'
            },
            files: {
                './': ['src/templates/pages/index.hbs']
            }
        }
    }
};
```
{{</ admonition >}}

## Tables

```markdown
| Option | Description |
| ------ | ----------- |
| data   | path to data files to supply the data that will be passed into templates. |
| engine | engine to be used for processing templates. Handlebars is the default. |
| ext    | extension to be used for dest files. |

| Option | Description |
|:------:| -----------:|
| data   | path to data files to supply the data that will be passed into templates. |
| engine | engine to be used for processing templates. Handlebars is the default. |
| ext    | extension to be used for dest files. |
```

```html
<table>
    <thead>
        <tr>
            <th>Option</th>
            <th>Description</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>data</td>
            <td>path to data files to supply the data that will be passed into templates.</td>
        </tr>
        <tr>
            <td>engine</td>
            <td>engine to be used for processing templates. Handlebars is the default.</td>
        </tr>
        <tr>
            <td>ext</td>
            <td>extension to be used for dest files.</td>
        </tr>
    </tbody>
</table>

<table>
    <thead>
        <tr>
            <th style="text-align:center">Option</th>
            <th style="text-align:right">Description</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td style="text-align:center">data</td>
            <td style="text-align:right">path to data files to supply the data that will be passed into templates.</td>
        </tr>
        <tr>
            <td style="text-align:center">engine</td>
            <td style="text-align:right">engine to be used for processing templates. Handlebars is the default.</td>
        </tr>
        <tr>
            <td style="text-align:center">ext</td>
            <td style="text-align:right">extension to be used for dest files.</td>
        </tr>
    </tbody>
</table>
```

{{< admonition type=abstract title="Rendered" >}}
| Option | Description |
| ------ | ----------- |
| data   | path to data files to supply the data that will be passed into templates. |
| engine | engine to be used for processing templates. Handlebars is the default. |
| ext    | extension to be used for dest files. |

| Option | Description |
|:------:| -----------:|
| data   | path to data files to supply the data that will be passed into templates. |
| engine | engine to be used for processing templates. Handlebars is the default. |
| ext    | extension to be used for dest files. |
{{</ admonition >}}

## Links

```markdown
<https://blog.bl4ckbird.com>
<bl4ckbird@bl4ckbird.com>
[bl4ckbird](https://blog.bl4ckbird.com)
[bl4ckbird](https://blog.bl4ckbird.com "BLOG!")
```

```html
<a href="https://blog.bl4ckbird.com">https://blog.bl4ckbird.com</a>
<a href="mailto:bl4ckbird@bl4ckbird.com">bl4ckbird@bl4ckbird.com</a>
<a href="https://blog.bl4ckbird.com">bl4ckbird</a>
<a href="https://blog.bl4ckbird.com" title="BLOG!">bl4ckbird</a>
```

{{< admonition type=abstract title="Rendered" >}}
<https://blog.bl4ckbird.com>

<bl4ckbird@bl4ckbird.com>

[bl4ckbird](https://blog.bl4ckbird.com)

[bl4ckbird](https://blog.bl4ckbird.com "BLOG!")
{{</ admonition >}}

## Named Anchors

```markdown
* [Chapter 1](#chapter-1)
* [Chapter 2](#chapter-2)
* [Chapter 3](#chapter-3)
```

```html
<ul>
    <li><a href="#chapter-1" rel="">Chapter 1</a></li>
    <li><a href="#chapter-2" rel="">Chapter 2</a></li>
    <li><a href="#chapter-3" rel="">Chapter 3</a></li>
</ul>
```

{{< admonition type=abstract title="Rendered" >}}
* [Chapter 1](#chapter-1)
* [Chapter 2](#chapter-2)
* [Chapter 3](#chapter-3)
{{</ admonition >}}

## Footnotes

```markdown
This is a digital footnote[^1].

This is a footnote with "label"[^label]

[^1]: This is a digital footnote
[^label]: This is a footnote with "label"
```

```html
<p>
    This is a digital footnote<sup id="fnref:1"><a href="#fn:1">1</a></sup>.
</p>
<p>
    This is a footnote with “label”<sup id="fnref:2"><a href="#fn:2">2</a></sup>
    </p>
```

{{< admonition type=abstract title="Rendered" >}}
This is a digital footnote[^1].

This is a footnote with "label"[^label]

[^1]: This is a digital footnote
[^label]: This is a footnote with "label"
{{</ admonition >}}

## Images

```markdown
![Minion](https://octodex.github.com/images/minion.png)
![Alt text](https://octodex.github.com/images/stormtroopocat.jpg "The Stormtroopocat")

![Alt text2][id]
Other contents

[id]: https://octodex.github.com/images/dojocat.jpg  "The Dojocat"
```

```html
<img src="https://octodex.github.com/images/minion.png" alt="Minion">
<img src="https://octodex.github.com/images/stormtroopocat.jpg" alt="Alt text" title="The Stormtroopocat">
<img src="https://octodex.github.com/images/dojocat.jpg" alt="Alt text2" title="The Dojocat">
<p>Other contents</p>
```

{{< admonition type=abstract title="Rendered" >}}
![Minion](https://octodex.github.com/images/minion.png)
![Alt text](https://octodex.github.com/images/stormtroopocat.jpg "The Stormtroopocat")

![Alt text2][id]
Other contents

[id]: https://octodex.github.com/images/dojocat.jpg  "The Dojocat"
{{</ admonition >}}

