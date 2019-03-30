## Markdown for Chez-scheme 
It provides `markdown->sxml` procedure, Completely based on chez-scheme and is written on pure scheme (r6rs). It doesn't rely on other scheme library.

## How to use
import it and `markdown->sxml` accept a texture port, returning sxml.

you may need a `sxml->html` library to transform sxml to html.

## Features
- syntax based on [GitHub Flavored Markdown](https://github.github.com/gfm)
- support `#` header
- suport `***` and `---` hr element
- support `*`, and `-` list also with ordered list with `1~9.`
- support `**`, `** **`, `_ _`, `__ __` inline strong and em element
- support `` ` `` inline code
- support `>` block quote
- support `- [ ] ` task list
- support `![]()` img element
- support `[]()` inner link
- support `$$` latex extension (you need to use katex to support this feature)
- support `~~` strike through element

- not support ~~space indent~~ and ~~nested element~~
  > that means four spaces will just be four spaces in a paragraph instead of a code block.
  and
```
> this is a block quote, the one
> this is another block quote, the two
  this just follows 'the two' block quote, including two spaces.
```
- not support ~~direct html code~~
- not support ~~link breaks~~
- not support ~~autolinks~~

~~there are more details in it, just in the docs(not available now).~~
