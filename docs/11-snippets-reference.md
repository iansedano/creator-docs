# Component Snippets

This is a quick reference to the HTML snippets used in our courses to build recurring elements. Most of them are based on Bootstrap. You can read more on the relevant Bootstrap classes by clicking the snippets title.

## [Section Tags](https://getbootstrap.com/docs/4.0/components/buttons/)

Blue:

```html
<div class="d-flex flex-row-reverse">
  <span class="badge badge-primary rounded">
      Section 1
  </span>
</div>
```

Yellow:

```html
<div class="d-flex flex-row-reverse">
  <span class="badge badge-warning rounded">
    Section 6
  </span>
</div>
```

## Section Dividers

Section Dividers (blue):

```html
<h5 class="section-divider">Section Mini-Heading</h5>
```

Assignment Dividers (yellow):

```html
<h5 class="section-assignment">Assignments</h5>
```

## Headings

Use Markdown for headings, and start your highest-level at `<h3>` (or `###` in Markdown). Avoid applying additional styling in the platform internal editor or through custom HTML classes and CSS.

## Color-Highlighted Boxes

Information Box (blue):

```html
<div class="alert alert-info" role="alert">
  <strong>Info:</strong> Highlights interesting (additional) information.
</div>
```

Note Box (yellow):

```html
<div class="alert alert-warning" role="alert">
  <strong>Note:</strong> Important infos about upcoming course sections, or potential gotchas.
</div>
```

## Resources

```html
<div class="jumbotron resources">
<h1>Resources</h1>
</div>
```

## Quotes

```html
<blockquote class="blockquote text-right">
  <p class="mb-0">insert quote text.</p>
  <footer class="blockquote-footer">who <a href=""><cite title="source title">source title</cite></a></footer>
</blockquote>
```

## Code Blocks

Use Markdown to create code blocks.

    ```python
    print("your code here")
    ```

## In-Line Code

Use Markdown to create in-line-code snippets:

  `my_funct()`

In the platform's **HTML editor** you can create them like this: `<code>your_code_here()</code>`
