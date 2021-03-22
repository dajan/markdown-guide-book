# Syntaxe de base {#basic-syntax}

La quasi-totalité des applications Markdown se conforment à la syntaxe de base décrite dans le document de conception original de John Gruber. Il y a des variations et des divergences mineures entre les processeurs Markdown - celles-ci sont notées en ligne chaque fois que cela est possible.

## Titres {#headings}

Pour créer un titre, ajoutez des dièses (`#`) devant un mot ou une phrase. Le nombre de dièses que vous utilisez doit correspondre au niveau du titre. Par exemple, pour créer un titre de niveau trois (`<h3>`), utilisez trois dièses (par exemple, `### Mon titre`).

| Markdown                       | HTML                       |
|--------------------------------|----------------------------|
| `# Titre niveau 1`            | `<h1>Titre niveau 1</h1>` |
| `## Titre niveau 2`           | `<h2>Titre niveau 2</h2>` |
| `### Titre niveau 3`          | `<h3>Titre niveau 3</h3>` |
| `#### Titre niveau 4`         | `<h4<Titre niveau 4</h4>` |
| `##### Titre niveau 5`        | `<h5>Titre niveau 5</h5>` |
| `###### Titre nvieau 6`       | `<h6>Titre niveau 6</h6>` |

### Autre syntaxe possible

Une autre manière de créer des titre consiste à placer sous la ligne du titre un nombre quelconque de `==` pour un titre de niveau 1 ou `--` pour un titre de niveau 2.

| Markdown                       | HTML                                   |
|--------------------------------|----------------------------------------|
| `Titre niveau 1`              | `<h1>Titre niveau 1</h1>`             |
| `===============`              |                                        |
|--------------------------------|----------------------------------------|
| `Titre niveau 2`              | `<h2>Titre niveau 2</h2>`             |
| `---------------`              |                                        |

### Bonnes pratiques avec les titres

Les applications Markdown ne traitent pas de la même manière les lignes vides entre les titres et les pragraphes qui suivent. Pour assurer une bonne compatibilité de votre texte avec les différentes applications Markdown, veillez à séparer les paragraphes et les titres avec une ou plusieurs lignes vides.

| Faites ceci                         | Ne faites pas cela                         |
|---------------------------------|---------------------------------------|
| `C'est un paragraphe.`          | `C'est un paragraphe.`                |
|                                 | `# Ceci est un titre 1`                |
| `# Ceci est un titre 1`          | `Et ceci est un nouveau paragraphe.`      |
|                                 |                                       |
| `Et ceci est un nouveau paragraphe.` |                                      |

## Paragraphes

Pour créer des paragraphes, utilisez une ligne blanche pour séparer une ou plusieurs lignes de texte.

{title="Markdown"}
~~~~~~~
J'aime beacuoup utiliser Markdown.

Je pense l'utiliser tout le temps dès aujourd'hui.
~~~~~~~

{title="HTML", lang=html}
~~~~~~~
<p>J'aime beacuoup utiliser Markdown.</p>

<p>Je pense l'utiliser tout le temps dès aujourd'hui.</p>
~~~~~~~

Le texte mis en forme resemble alors à ceci :

J'aime beacuoup utiliser Markdown.

Je pense l'utiliser tout le temps dès aujourd'hui.

### Bonnes pratiques avec les paragraphes

N'indentez pas les paragraphes avec des espaces ou des tabulations.

| Faites ceci                         | Ne faites pas cela                         |
|---------------------------------|---------------------------------------|
| `Ne mettez pas des tabulateurs ou des espaces au début des paragraphes.` | &nbsp;&nbsp;&nbsp;&nbsp;`Ceci peut provoquer des problèmes de mise en page.` |
|                                 |                                       |
| `Gardez toutes les lignes alignée à gauche, comme ceci.` | &nbsp;&nbsp;`N'ajoutez pas d'espaces ou des tabulateurs en début des paragraphes.` |

## Sauts de ligne

Pour créer un saut de ligne dans un même paragraphe (`<br>`), terminez la ligne avec au moins deux espaces, puis tappez sur la touche *retour* pour créer un nouveau paragraphe.

{title="Markdown"}
~~~~~~~
Ceci est la première ligne.  
Et cela est la seconde.
~~~~~~~

{title="HTML", lang=html}
~~~~~~~
<p>Ceci est la première ligne.<br />
Et cela est la seconde.</p>
~~~~~~~

Le texte mis en forme resemble alors à ceci :

Ceci est la première ligne.  
Et cela est la seconde.

### Bonnes pratiques avec les sauts de ligne

Vous pouvez utiliser deux espaces, ou plus, (appelés "espaces blancs de fin de ligne") pour les sauts de ligne dans presque toutes les applications Markdown, mais cette pratique est controversée. Il est difficile de voir les espaces de fin de ligne dans un éditeur, et de nombreuses personnes mettent accidentellement ou intentionnellement deux espaces après chaque phrase (vieille habitude anglosaxone). C'est la raison pour laquelle vous voudrez peut-être utiliser autre chose que les espaces de queue pour les sauts de ligne. Heureusement, il existe une autre option prise en charge par presque toutes les applications Markdown : la balise HTML `<br>`.

Pour des raisons de compatibilité, utilisez l'espace blanc de fin de ligne ou la balise HTML `<br>` à la fin de la ligne.

Il existe deux autres options que je ne recommande pas d'utiliser. CommonMark et quelques autres langages de balisage légers vous permettent de taper une barre oblique inverse (*backslash*) (`\`) à la fin d'une ligne, mais toutes les applications Markdown ne le prennent pas en charge, ce qui n'est pas une bonne option du point de vue de la compatibilité. Et au moins deux langages de balisage légers ne nécessitent rien en fin de ligne - il suffit de taper return pour créer un saut de ligne.

| Faites ceci                         | Ne faites pas cela                         |
|---------------------------------|---------------------------------------|
| `Première ligne avec deux espaces après le point.` | `Première ligne avec une barre oblique inverse après le point.\` |
| `Puis la ligne suivante.`            | `Puis la ligne suivante.`                  |
|                                 |                                       |
| `Utiliser la balise HTML après le point.<br>`  | `Rien après le point.`                 |
| `Puis la ligne suivante.`            | `Puis la ligne suivante.`                  |

## Mise en évidence {#emphasis}

Vous pouvez mettre en évidence une partie du texte en y applicant du gras ou de l'italique.

### Gras {#bold}

Pour mettre un texte en gras, ajoutez deux astérisques ou deux traits de soulignement avant et après un mot ou une phrase. Pour mettre le milieu d'un mot en gras, ajoutez deux astérisques sans espace autour des lettres.

{title="Markdown"}
~~~~~~~
J'adore les **textes en gras**.

J'adore les __textes en gras__.

L'amour**est**grand
~~~~~~~

La sortie HTML des deux premiers exemples est la même.

{title="HTML", lang=html}
~~~~~~~
J'adore les<strong>texes en gras</strong>.

L'amour <strong>est</strong> grand
~~~~~~~

Le résultat ressemble à ceci :

J'adore les **textes en gras**.

L'amour**est**grand

#### Bonnes pratiques avec le gras

Les applications Markdown ne s'accordent pas sur la manière de gérer les caractères de soulignement au milieu d'un mot. Par souci de compatibilité, utilisez des astérisques pour mettre en gras le milieu d'un mot afin de le mettre en valeur.

| Faites ceci | Ne faites pas cela |
|------------|-------------------|
| `L'amour**est**grand` | `L'amour__est__grand` |

### Italique {#italic}

Pour mettre un texte en italique, ajoutez un astérisque ou un trait de soulignement avant et après un mot ou une phrase. Pour mettre en italique le milieu d'un mot, ajoutez un astérisque sans espace autour des lettres.

{title="Markdown"}
~~~~~~~
Le *miaou du chat*.

Le _miaou du chat_.

Un*chat*miaule
~~~~~~~

La sortie HTML des deux premiers exemples est la même.

{title="HTML", lang=html}
~~~~~~~
Le <em>miaulement du chat</em>.

Un<em>chat</em>miaule
~~~~~~~

Le résultat final ressemble à ceci :

Le *miaulement du chat*.

Un*chat*miaule

#### Bonnes pratiques avec l'italique

Les applications Markdown ne s'accordent pas sur la manière de traiter les traits de soulignement au milieu d'un mot. Pour des raisons de compatibilité, utilisez les astérisques pour mettre en italique le milieu d'un mot.

| Faites ceci | Ne faites pas cela |
|------------|-------------------|
| `Un*chat*miaule` | `Un_chat_miaule` |

### Gras et italique

Pour mettre du texte en gras et en italique en même temps, ajoutez trois astérisques ou caractères de soulignement avant et après un mot ou une phrase. Pour mettre en gras et en italique le milieu d'un mot, ajoutez trois astérisques sans espace autour des lettres.

{title="Markdown"}
~~~~~~~
Texte ***important***.

Texte ___important___.

Texte __*important*__.

**_important_** et à lire.

Très***très***important et à lire.
~~~~~~~

La sortie HTML des quatre premiers exemples est la même.

{title="HTML", lang=html}
~~~~~~~
Texte <strong><em>important</em></strong>.

Texte trés<strong><em>très</em></strong>important.
~~~~~~~

Le résultat ressemble à ceci :

Texte ***important***.

Texte très***très***important.

#### Bonnes pratiques avec le gras-italique

Les applications Markdown ne s'accordent pas sur la manière de gérer les caractères de soulignement au milieu d'un mot. Pour des raisons de compatibilité, utilisez les astérisques pour mettre en gras et en italique le milieu d'un mot afin de le mettre en valeur.

| Faites ceci | Ne faites pas cela |
|------------|-------------------|
| `Texte très***très***important text. ` | `Texte très___très___important.` |

## Citations {#blockquotes}

Pour créer une citation en bloc, ajoutez un `>` devant un paragraphe.

{title="Markdown"}
~~~~~~~
> Dorothy l'a suivie à travers de nombreuses pièces.
~~~~~~~

{title="HTML", lang=html}
~~~~~~~
<blockquote>
  <p>Dorothy l'a suivie à travers de nombreuses pièces.</p>
</blockquote>
~~~~~~~

Le résultat ressemble à cela :

> Dorothy l'a suivie à travers de nombreuses pièces.

### Citations avec plusieurs paragraphes

Les citations peuvent contenir plusieurs paragraphes. Ajoutez un `>` sur les lignes vides entre les paragraphes.

{title="Markdown"}
~~~~~~~
> Ceci est le premier paragraphe.
>
> Et cecla est le deuxième paragraphe.
~~~~~~~

{title="HTML", lang=html}
~~~~~~~
<blockquote>
  <p>Ceci est le premier paragraphe.</p>
  <p>Et cela est le deuxième paragraphe.</p>
</blockquote>
~~~~~~~

Le résulat ressemble à ceci :

> Ceci est le premier paragraphe.
>
> Cela est le deuxième paragraphe.

### Citations à plusieurs niveaux

Les citations peuvent se trouver à l'intérieur d'une autre citation. Dans ce cas, ajouter `>>` devant le paragraphe de deuxième niveau.Add a `>>` in front of the paragraph you want to nest.

{title="Markdown"}
~~~~~~~
> Ceci est le premier paragraphe.
>
>> Cela est le deuxième paragraphe.
~~~~~~~

{title="HTML", lang=html}
~~~~~~~
<blockquote>
  <p>Ceci est le premier paragraphe.</p>
  <blockquote>
    <p>Cela est le deuxième paragraphe.</p>
  </blockquote>
</blockquote>
~~~~~~~

Le résultat ressemble à ceci :

> Ceci est le premier paragraphe.
>
>> Cela est le deuxième paragraphe.

### Citations en bloc avec d'autres éléments

Les guillemets peuvent contenir d'autres éléments au format Markdown. Tous les éléments ne peuvent pas être utilisés - vous devrez expérimenter pour voir ceux qui fonctionnent.

{title="Markdown"}
~~~~~~~
> ##### Les résultats trimestriels sont excellents !
>
> - Les recettes ont atteint des sommets.
> - Les bénéfices sont plus élevés que jamais.
>
> *Tout* va **bien**.
~~~~~~~

{title="HTML", lang=html}
~~~~~~~
<blockquote>
  <h5>Les résultats trimestriels sont excellents !</h5>
  <ul>
    <li>Les recettes ont atteint des sommets.</li>
    <li>Les bénéfices sont plus élevés que jamais.</li>
  </ul>
  <p><em>Tout</em> va <strong>bien</strong>.</p>
</blockquote>
~~~~~~~

The rendered output looks like this:

> ##### Les résultats trimestriels sont excellents !
>
> - Les recettes ont atteint des sommets.
> - Les bénéfices sont plus élevés que jamais.
>
>  *Tout* va **bien**.

## Listes

Vous pouvez organiser les éléments en listes ordonnées et non ordonnées.

### Ordered Lists {#ordered-lists}

To create an ordered list, add line items with numbers followed by periods. The numbers don’t have to be in numerical order, but the list should start with the number one.

{title="Markdown"}
~~~~~~~
1. First item
2. Second item
3. Third item
4. Fourth item

1. First item
1. Second item
1. Third item
1. Fourth item

1. First item
8. Second item
3. Third item
5. Fourth item
~~~~~~~

The HTML output of all three example lists is the same.

{title="HTML", lang=html}
~~~~~~~
<ol>
  <li>First item</li>
  <li>Second item</li>
  <li>Third item</li>
  <li>Fourth item</li>
</ol>
~~~~~~~

The rendered output looks like this:

1. First item
2. Second item
3. Third item
4. Fourth item

#### Nesting List Items

To nest line items in an ordered list, indent the items four spaces or one tab.

{title="Markdown"}
~~~~~~~
1. First item
2. Second item
3. Third item
    1. Indented item
    2. Indented item
4. Fourth item
~~~~~~~

{title="HTML", lang=html}
~~~~~~~
<ol>
  <li>First item</li>
  <li>Second item</li>
  <li>Third item
    <ol>
      <li>Indented item</li>
      <li>Indented item</li>
    </ol>
  </li>
  <li>Fourth item</li>
</ol>
~~~~~~~

The rendered output looks like this:

1. First item
2. Second item
3. Third item
    1. Indented item
    2. Indented item
4. Fourth item

### Unordered Lists {#unordered-lists}

To create an unordered list, add dashes (`-`), asterisks (`*`), or plus signs (`+`) in front of line items.

{title="Markdown"}
~~~~~~~
- First item
- Second item
- Third item
- Fourth item

* First item
* Second item
* Third item
* Fourth item

+ First item
* Second item
- Third item
+ Fourth item
~~~~~~~

The HTML output of all three example lists is the same.

{title="HTML", lang=html}
~~~~~~~
<ul>
  <li>First item</li>
  <li>Second item</li>
  <li>Third item</li>
  <li>Fourth item </li>
</ul>
~~~~~~~

The rendered output looks like this:

- First item
- Second item
- Third item
- Fourth item

#### Nesting List Items

To nest line items in an unordered list, indent the items four spaces or one tab.

{title="Markdown"}
~~~~~~~
- First item
- Second item
- Third item
    - Indented item
    - Indented item
- Fourth item
~~~~~~~

{title="HTML", lang=html}
~~~~~~~
<ul>
  <li>First item</li>
  <li>Second item</li>
  <li>Third item
    <ul>
      <li>Indented item</li>
      <li>Indented item</li>
    </ul>
  </li>
  <li>Fourth item</li>
</ul>
~~~~~~~

The rendered output looks like this:

- First item
- Second item
- Third item
    - Indented item
    - Indented item
- Fourth item

### Adding Elements in Lists

To add another element in a list while preserving the continuity of the list, indent the element four spaces or one tab, as shown in the following examples.

#### Paragraphs

{title="Markdown"}
~~~~~~~
*   This is the first list item.
*   Here's the second list item.

    I need to add another paragraph below the second list item.

*   And here's the third list item.
~~~~~~~

{title="HTML", lang=html}
~~~~~~~
<ul>
  <li><p>This is the first list item.</p></li>
  <li><p>Here's the second list item.</p>
    <p>I need to add another paragraph below the second list item.</p>
  </li>
  <li><p>And here's the third list item.</p></li>
</ul>
~~~~~~~

The rendered output looks like this:

*   This is the first list item.
*   Here's the second list item.

    I need to add another paragraph below the second list item.

*   And here's the third list item.

#### Blockquotes

{title="Markdown"}
~~~~~~~
*   This is the first list item.
*   Here's the second list item.

    > A blockquote would look great here.

*   And here's the third list item.
~~~~~~~

{title="HTML", lang=html}
~~~~~~~
<ul>
  <li><p>This is the first list item.</p></li>
  <li><p>Here's the second list item.</p>
    <blockquote>
      <p>A blockquote would look great here.</p>
    </blockquote>
  </li>
  <li><p>And here's the third list item.</p>
  </li>
</ul>
~~~~~~~

The rendered output looks like this:

*   This is the first list item.
*   Here's the second list item.

    > A blockquote would look great here.

*   And here's the third list item.

#### Code Blocks

[Code blocks](#code-blocks) are normally indented four spaces or one tab. When they’re in a list, indent them eight spaces or two tabs.

{title="Markdown"}
~~~~~~~
1.  Open the file.
2.  Find the following code block on line 21:

        <html>
          <head>
            <title>Test</title>
          </head>

3.  Update the title to match the name of your website.
~~~~~~~

{title="HTML", lang=html}
~~~~~~~
<ol>
  <li><p>Open the file.</p></li>
  <li><p>Find the following code block on line 21:</p>
    <pre><code>&lt;html&gt;
      &lt;head&gt;
        &lt;title&gt;Test&lt;/title&gt;
      &lt;/head&gt;
    </code></pre>
  </li>
  <li><p>Update the title to match the name of your website.</p></li>
</ol>
~~~~~~~

The rendered output looks like this:

1.  Open the file.
2.  Find the following code block on line 21:

        <html>
          <head>
            <title>Test</title>
          </head>

3.  Update the title to match the name of your website.

#### Images

{title="Markdown"}
~~~~~~~
1.  Open the file containing Tux, the Linux mascot.
2.  Marvel at its beauty.

    ![Tux](images/tux.png)

3.  Close the file.
~~~~~~~

{title="HTML", lang=html}
~~~~~~~
<ol>
  <li><p>Open the file containing Tux, the Linux mascot.</p></li>
  <li>
    <p>Marvel at its beauty.</p>
    <p><img src="images/tux.png" alt="Tux" /></p>
  </li>
  <li><p>Close the file.</p></li>
</ol>
~~~~~~~

The rendered output looks like this:

1.  Open the file containing Tux, the Linux mascot.
2.  Marvel at its beauty.

    ![Tux](images/tux.png)

3.  Close the file.

## Code {#code}

To denote a word or phrase as code, enclose it in backticks (`` ` ``).

{title="Markdown"}
~~~~~~~
At the command prompt, type `nano`.
~~~~~~~

{title="HTML", lang=html}
~~~~~~~
At the command prompt, type <code>nano</code>.
~~~~~~~

The rendered output looks like this:

At the command prompt, type `nano`.

### Escaping Backticks {#escaping-backticks}

If the word or phrase you want to denote as code includes one or more backticks, you can escape it by enclosing the word or phrase in double backticks (`` `` ``).

{title="Markdown"}
~~~~~~~
``Use `code` in your Markdown file.``
~~~~~~~

{title="HTML", lang=html}
~~~~~~~
<code>Use `code` in your Markdown file.</code>
~~~~~~~

The rendered output looks like this:

``Use `code` in your Markdown file.``

### Code Blocks {#code-blocks}

To create code blocks, indent every line of the block by at least four spaces or one tab.

{title="Markdown"}
~~~~~~~
    <html>
      <head>
      </head>
    </html>
~~~~~~~

{title="HTML", lang=html}
~~~~~~~
<pre>
  <code>
    &lt;html&gt;
      &lt;head&gt;
      &lt;/head&gt;
    &lt;/html&gt;
  </code>
</pre>
~~~~~~~

The rendered output looks like this:

    <html>
      <head>
      </head>
    </html>

I> To create code blocks without indenting lines, use [fenced code blocks](#fenced-code-blocks).

## Horizontal Rules {#horizontal-rules}

To create a horizontal rule, use three or more asterisks (`***`), dashes (`---`), or underscores (`___`) on a line by themselves.

{title="Markdown"}
~~~~~~~
***

---

_________________
~~~~~~~

{title="HTML", lang=html}
~~~~~~~
<hr />

<hr />

<hr />
~~~~~~~

The rendered output of all three looks identical:

***

### Horizontal Rule Best Practices

For compatibility, put blank lines before and after horizontal rules.

Do this:

{title="Markdown"}
~~~~~~~
Try to put a blank line before...

---

...and after a horizontal rule.
~~~~~~~

Don't do this:

{title="Markdown"}
~~~~~~~
Without blank lines, this would be a heading.
---
Don't do this!
~~~~~~~

## Links {#links}

To create a link, enclose the link text in brackets (e.g., `[Duck Duck Go]`) and then follow it immediately with the URL in parentheses (e.g., `(https://duckduckgo.com)`).

{title="Markdown"}
~~~~~~~
Use [Duck Duck Go](https://duckduckgo.com).
~~~~~~~

{title="HTML", lang=html}
~~~~~~~
Use <a href="https://duckduckgo.com">Duck Duck Go</a>.
~~~~~~~

The rendered output looks like this:

Use [Duck Duck Go](https://duckduckgo.com).

### Adding Titles

You can optionally add a title for a link. This will appear as a tooltip when the user hovers over the link. To add a title, enclose it in parentheses after the URL.

{title="Markdown"}
~~~~~~~
Use [Duck Duck Go](https://duckduckgo.com "My search engine!").
~~~~~~~

{title="HTML", lang=html}
~~~~~~~
Use <a href="https://duckduckgo.com" title="My search engine!">Duck Duck Go</a>.
~~~~~~~

The rendered output looks like this:

Use [Duck Duck Go](https://duckduckgo.com "My search engine!").

### URLs and Email Addresses

To quickly turn a URL or email address into a link, enclose it in angle brackets.

{title="Markdown"}
~~~~~~~
<https://eff.org>
<fake@example.com>
~~~~~~~

{title="HTML", lang=html}
~~~~~~~
<a href="https://eff.org">https://eff.org</a>
<a href="mailto:fake@example.com">fake@example.com</a>
~~~~~~~

The rendered output looks like this:

<https://eff.org>  
<fake@example.com>

### Formatting Links

To [emphasize](#emphasis) links, add asterisks before and after the brackets and parentheses. To denote links as [code](#code), add backticks in the brackets.

{title="Markdown"}
~~~~~~~
I love supporting **[EFF](https://eff.org)**.
This is the *[EFF](https://eff.org)*.
See the section on [`code`](#code).
~~~~~~~

{title="HTML", lang=html}
~~~~~~~
I love supporting <strong><a href="https://eff.org">EFF</a></strong>.
This is the <em><a href="https://eff.org">EFF</a></em>.
See the section on <a href="#code"><code>code</code></a>.
~~~~~~~

The rendered output looks like this:

I love supporting **[EFF](https://eff.org)**.  
This is the *[EFF](https://eff.org)*.
See the section on [`code`](#code).

### Reference-style Links

Reference-style links are a special kind of link that make URLs easier to display and read in Markdown. Reference-style links are constructed in two parts: the part you keep inline with your text and the part you store somewhere else in the file to keep the text easy to read.

#### Formatting the First Part of the Link

The first part of a reference-style link is formatted with two sets of brackets. The first set of brackets surrounds the text that should appear linked. The second set of brackets displays a label used to point to the link you’re storing elsewhere in your document.

Although not required, you can include a space between the first and second set of brackets. Also, the label in the second set of brackets is not case sensitive and can include letters, numbers, spaces, or punctuation.

This means the following example formats are all roughly equivalent for the first part of the link:

- `[hobbit-hole][1]`
- `[hobbit-hole] [1]`
- `[hobbit-hole][a]`
- `[hobbit-hole][A]`

#### Formatting the Second Part of the Link

The second part of a reference-style link is formatted with the following attributes:

1. The label, in brackets, followed immediately by a colon and at least one space (e.g., `[label]:` ).
2. The URL for the link, which you can optionally enclose in angle brackets.
3. The optional title for the link, which you can enclose in double quotes, single quotes, or parentheses.

This means the following example formats are all roughly equivalent for the second part of the link:

- `[hobbit-hole]: https://en.wikipedia.org/wiki/Hobbit#Lifestyle`
- `[hobbit-hole]: https://en.wikipedia.org/wiki/Hobbit#Lifestyle "Hobbit lifestyles"`
- `[hobbit-hole]: https://en.wikipedia.org/wiki/Hobbit#Lifestyle 'Hobbit lifestyles'`
- `[hobbit-hole]: https://en.wikipedia.org/wiki/Hobbit#Lifestyle (Hobbit lifestyles)`
- `[hobbit-hole]: <https://en.wikipedia.org/wiki/Hobbit#Lifestyle> "Hobbit lifestyles"`
- `[hobbit-hole]: <https://en.wikipedia.org/wiki/Hobbit#Lifestyle> 'Hobbit lifestyles'`
- `[hobbit-hole]: <https://en.wikipedia.org/wiki/Hobbit#Lifestyle> (Hobbit lifestyles)`

You can place this second part of the link anywhere in your Markdown document. Some people place them immediately after the paragraph in which they appear while other people place them at the end of the document (like endnotes or footnotes).

#### An Example Putting the Parts Together

Say you add a URL as a [standard URL link](#links) to a paragraph and it looks like this in Markdown:

{title="Markdown"}
~~~~~~~
In a hole in the ground there lived a hobbit. Not a nasty, dirty, wet hole, filled with the ends of worms and an oozy smell, nor yet a dry, bare, sandy hole with nothing in it to sit down on or to eat: it was a [hobbit-hole](https://en.wikipedia.org/wiki/Hobbit#Lifestyle "Hobbit lifestyles"), and that means comfort.
~~~~~~~

{title="Markdown"}
~~~~~~~
In a hole in the ground there lived a hobbit. Not a nasty, dirty, wet hole, filled with the ends of worms and an oozy smell, nor yet a dry, bare, sandy hole with nothing in it to sit down on or to eat: it was a [hobbit-hole][1], and that means comfort.

[1]: <https://en.wikipedia.org/wiki/Hobbit#Lifestyle> "Hobbit lifestyles"
~~~~~~~

In both instances above, the HTML for the link would be identical:

{title="HTML", lang=html}
~~~~~~~
<a href="https://en.wikipedia.org/wiki/Hobbit#Lifestyle" title="Hobbit lifestyles">hobbit-hole</a>
~~~~~~~

The output is also identical:

In a hole in the ground there lived a hobbit. Not a nasty, dirty, wet hole, filled with the ends of worms and an oozy smell, nor yet a dry, bare, sandy hole with nothing in it to sit down on or to eat: it was a [hobbit-hole](https://en.wikipedia.org/wiki/Hobbit#Lifestyle), and that means comfort.

### Link Best Practices

Markdown applications don’t agree on how to handle spaces in the middle of a URL. For compatibility, try to URL encode any spaces with `%20`.

Do this:

{title="Markdown"}
~~~~~~~
[link](https://www.example.com/my%20great%20page)
~~~~~~~

Don't do this:

{title="Markdown"}
~~~~~~~
[link](https://www.example.com/my great page)
~~~~~~~

## Images {#images}

To add an image, add an exclamation mark (`!`), followed by alt text in brackets, and the path or URL to the image asset in parentheses. You can optionally add a title after the URL in the parentheses.

{title="Markdown"}
~~~~~~~
![Philadelphia's Magic Gardens. This place was so cool!](images/philly-magic-garden.png "Philadelphia's Magic Gardens")
~~~~~~~

{title="HTML", lang=html}
~~~~~~~
<img src="images/philly-magic-garden.png" alt="Philadelphia's Magic Gardens. This place was so cool!" title="Philadelphia's Magic Gardens" />
~~~~~~~

The rendered output looks like this:

![Philadelphia's Magic Gardens. This place was so cool!](images/philly-magic-garden.png "Philadelphia's Magic Gardens")

## Escaping Characters

To display a literal character that would otherwise be used to format text in a Markdown document, add a backslash (`\`) in front of the character.

{title="Markdown"}
~~~~~~~
\* Without the backslash, this would be a bullet in an unordered list.
~~~~~~~

{title="HTML", lang=html}
~~~~~~~
* Without the backslash, this would be a bullet in an unordered list.
~~~~~~~

The rendered output looks like this:

\* Without the backslash, this would be a bullet in an unordered list.

### Characters You Can Escape

You can use a backslash to escape the following characters.

| Character         | Name                  |
|-------------------|-----------------------|
| `\`               | backslash             |
| `` ` ``           | backtick (see also [escaping backticks in code](#escaping-backticks)) |
| `*`               | asterisk              |
| `_`               | underscore            |
| `{}`              | curly braces          |
| `[]`              | brackets              |
| `()`              | parentheses           |
| `#`               | pound sign            |
| `+`               | plus sign             |
| `-`               | minus sign (hyphen)   |
| `.`               | dot                   |
| `!`               | exclamation mark      |
| `|`               | pipe (see also [escaping pipe in tables](#escaping-pipe-characters-in-tables)) |

## HTML

Many Markdown applications allow you to use HTML tags in Markdown-formatted text. This is helpful if you prefer certain HTML tags to Markdown syntax. For example, some people find it easier to use HTML tags for images. Using HTML is also helpful when you need to change the attributes of an element, like specifying the color of text or changing the width of an image.

To use HTML, place the tags in the text of your Markdown-formatted file.

{title="Markdown"}
~~~~~~~
This **word** is bold. This <em>word</em> is italic.
~~~~~~~

{title="HTML", lang=html}
~~~~~~~
This <strong>word</strong> is bold. This <em>word</em> is italic.
~~~~~~~

The rendered output looks like this:

This **word** is bold. This *word* is italic.

### HTML Best Practices

For security reasons, not all Markdown applications support HTML in Markdown documents. When in doubt, check your Markdown application's documentation. Some applications support only a subset of HTML tags.

Use blank lines to separate block-level HTML elements like `<div>`, `<table>`, `<pre>`, and `<p>` from the surrounding content. Try not to indent the tags with tabs or spaces — that can interfere with the formatting.

You can't use Markdown syntax inside block-level HTML tags. For example, `<p>italic and **bold**</p>` won't work.
