# Markdown Syntax Images

See [Daring Fireball: Markdown Syntax Images Documents](https://daringfireball.net/projects/markdown/syntax#img) .

Admittedly, it’s fairly difficult to devise a “natural” syntax for placing images into a plain text document format.

Markdown uses an image syntax that is intended to resemble the syntax for links, allowing for two styles: *inline* and *reference*.

Inline image syntax looks like this:

```markdown
![Alt text](/path/to/img.jpg)

![Alt text](/path/to/img.jpg "Optional title")
```

That is:

- An exclamation mark: `!`;
- followed by a set of square brackets, containing the `alt` attribute text for the image;
- followed by a set of parentheses, containing the URL or path to the image, and an optional `title` attribute enclosed in double or single quotes.

Reference-style image syntax looks like this:

```markdown
![Alt text][id]
```

Where “id” is the name of a defined image reference. Image references are defined using syntax identical to link references:

```markdown
[id]: url/to/image  "Optional title attribute"
```

As of this writing, Markdown has no syntax for specifying the dimensions of an image; if this is important to you, you can simply use regular HTML `<img>` tags.

