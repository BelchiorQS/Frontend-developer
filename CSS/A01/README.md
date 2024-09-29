# CSS Selectors

A CSS selector selects the HTML element(s) you want to style.

## CSS Selectors

CSS selectors are used to "find" (or select) the HTML elements you want to style.

We can divide CSS selectors into five categories:

1. **Simple selectors** (select elements based on name, id, class)
2. **Combinator selectors** (select elements based on a specific relationship between them)
3. **Pseudo-class selectors** (select elements based on a certain state)
4. **Pseudo-elements selectors** (select and style a part of an element)
5. **Attribute selectors** (select elements based on an attribute or attribute value)

This page will explain the most basic CSS selectors.

### The CSS Element Selector

The element selector selects HTML elements based on the element name.

**Example:**

Here, all `<p>` elements on the page will be center-aligned, with a red text color:

```css
p {
  text-align: center;
  color: red;
}
```

### The CSS ID Selector

The ID selector uses the `id` attribute of an HTML element to select a specific element.

The ID of an element is unique within a page, so the ID selector is used to select one unique element!

To select an element with a specific ID, write a hash (`#`) character, followed by the ID of the element.

**Example:**

The CSS rule below will be applied to the HTML element with `id="para1"`:

```css
#para1 {
  text-align: center;
  color: red;
}
```

**Note:** An ID name cannot start with a number!

### The CSS Class Selector

The class selector selects HTML elements with a specific class attribute.

To select elements with a specific class, write a period (`.`) character, followed by the class name.

**Example:**

In this example, all HTML elements with `class="center"` will be red and center-aligned:

```css
.center {
  text-align: center;
  color: red;
}
```

You can also specify that only specific HTML elements should be affected by a class.

**Example:**

In this example, only `<p>` elements with `class="center"` will be red and center-aligned:

```css
p.center {
  text-align: center;
  color: red;
}
```


## All CSS Simple Selectors

| Selector           | Example      | Example Description                                      |
|--------------------|--------------|----------------------------------------------------------|
| `#id`              | `#firstname` | Selects the element with `id="firstname"`                |
| `.class`           | `.intro`     | Selects all elements with `class="intro"`                |
| `element.class`    | `p.intro`    | Selects only `<p>` elements with `class="intro"`         |
| `*`                | `*`          | Selects all elements                                     |
| `element`          | `p`          | Selects all `<p>` elements                               |
| `element,element,..` | `div, p`    | Selects all `<div>` elements and all `<p>` elements      |

