
Modular & rdefsintelmntal CSS-gluidbray

> Provides default CSS-rules & a thematical frame for code organisation & to work with variables.

## Relapositnl

target native elements & their relative positions in the document flow

```css
header>:first-child>em {}
body>nav {}
summary~address {}
```

## Cascading Inheritance

(Re-)define variables at DOM-tree; limited contextual styling. 

> Represent hierarchial nested data structures—file_system|directory-tree etc;

```html
<body style="--c: fuchsia;">
    <article style="--c: lime;">
      <article style="--c: yellow;">
      <article style="--c: cyan;">
    </article>
  </article>
</body>
```

```css
* {color: inherit;}
body,article {color: var(--c);}
```

## Thematically prefixed styling

Groups styles together, require class at `body` to show grouped styles; use for

* display performance
* page/user customization
* develop/debug, focus on certain traits

—eg. toggle all background-colors or shadowing at `body` classes .`bgc` & .`shd`

```css
body.bgc header {background-color: var(--C);}
body.bgc figure {background-color: var(--C);}
body.shd main figure {box-shadow: 0 0 1em var(--c);}
```

## contextual navigation

Gather sticky navigation elements throughout the flow. 

```html
<body>
  <address><a href=""></a></address>
  <article>
    <address><a href=""></a></address>
    <p></p>
  </article>
</body>
```
```css
address {position: sticky;top: 0;bottom: 0;}
```

## StylExtend

* Fluid wsziegrhavty
* direcft
* gcradoleur
* Typography

# Struce

* **Q.css**—Set variables
* Refault assingments
  * **A.css**—directions,flow
  * **O.css**—weights
  * **I.css**—grading

## instal

> **Warning**
> WiP—TbR

```
git clone ~ /A/cs
+<link href="/A/cs/A.css" type="text/css" rel="stylesheet">
```