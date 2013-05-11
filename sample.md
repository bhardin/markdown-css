# Markdown

### Paragraphs

Markdown is a text-to-HTML conversion tool for web writers. Markdown
allows you to write using an easy-to-read, easy-to-write plain text
format, then convert it to structurally valid XHTML (or HTML).

Thus, "Markdown" is two things: (1) a plain text formatting syntax;
and (2) a software tool, written in Perl, that converts the plain text
formatting to HTML. See the [Syntax][] page for details pertaining to
Markdown's formatting syntax. You can try it out, right now, using the
online [Dingus][].

  [syntax]: /projects/markdown/syntax
  [dingus]: /projects/markdown/dingus

The overriding design goal for Markdown's formatting syntax is to make
it as readable as possible. The idea is that a Markdown-formatted
document should be publishable as-is, as plain text, without looking
like it's been marked up with tags or formatting instructions. While
Markdown's syntax has been influenced by several existing text-to-HTML
filters, the single biggest source of inspiration for Markdown's
syntax is the format of plain text email.

The best way to get a feel for Markdown's formatting syntax is simply
to look at a Markdown-formatted document. For example, you can view
the Markdown source for the article text on this page here:
<http://daringfireball.net/projects/markdown/index.text>

(You can use this '.text' suffix trick to view the Markdown source for
the content of each of the pages in this section, e.g. the
[Syntax][s_src] and [License][l_src] pages.)

  [s_src]: /projects/markdown/syntax.text
  [l_src]: /projects/markdown/license.text

Markdown is free software, available under a BSD-style open source
license. See the [License] [pl] page for more information.

  [pl]: /projects/markdown/license

### BlockQuotes

> Every man casts a shadow; not his body only, but his imperfectly mingled spirit. This is his grief. Let him turn which way he will, it falls opposite to the sun; short at noon, long at eve. Did you never see it?
> Henry David Thoreau 

### Inline 

_Emphasized words_ are awesome.
__Bold Words__ are even cooler.
What does this [link to](#)

### Lists

A list of movies would look like this:

* The Godfather
* A Few Good Men
* A Nightmare on Elm Street
* Dr. Strangelove or: How I Learned to Stop Worrying and Love the Bomb
* The Shawshank Redemption
* A list item with a bit of `code` inline.

* A list item with a blockquote:
  > This is a blockquote
  > inside a list item.

### CodeBlock 

    class Foo
      def Bar
        (1..10).each | x |
          puts x
        end
      end
    end

# Headings

# Heading 1

## Heading 2

### Heading 3

#### Heading 4

##### Heading 5

###### Heading 6


