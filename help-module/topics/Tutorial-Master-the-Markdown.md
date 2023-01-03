# Tutorial: Master the Markdown

Markdown is a markup language designed to be simple enough to let anyone write structured documents without the need of a visual editor

I **strongly** encourage you to change the source of the various parts to see what happens (the output will change as y
Start typing here...

Basic styles
------------

With this markup you can obtain *simple emhpasis* (usually rendered in italic text), **strong emphasis** (usually rendered in bold text), `source code` text (usually rendered in monospaced text), or ~~strikethrough~~ text (usually rendered with a line through text).

You may use also _this_ or __this__ notation to emphatize text, and you can use all them _**`together`**_ (and you can mix `*` and `_` )

If you look at the source code you may note that
even
if
you
break
the
lines,
the text is kept together
in a single paragraph

Paragraphs are delimited by blank lines, leading and trailing spaces are removed

You may force a line break with two spaces or with a `\`\ at the end of the line.

Links
-----

- You can insert links in text like [this](Tutorial-How-to-ride-a-bike.topic)

- You may add a [title](https://agea.github.io/tutorial.md "Markdown Tutorial") to your link (can you see the tooltip?)

- If your link contains spaces you have to write the [link](<http://example.com/a space>) between `<>`

- You can use spaces and markup inside the [link **text**](https://agea.github.io/tutorial.md)

- Long links may decrease source readability, so it's posible to define all links somewhere in the document (the end is a good place) and just reference the [link](JVM-Spring-boot.md) you may also collapse the reference if it matches the link text (example:  [tutorial.md][])

- You may also write directly the link: <https://agea.github.io/tutorial.md>

- It will work also for email addresses: <email@example.com> (you may write vaild email links also using [mailto](mailto:email@example.com) as protocol.

Images
------

Syntax for images is like the syntax for links, but with a `!` before:

![alt text](1.png "image title")

![](2.png)

![ref]

[ref]: 3.png

Source code
-----------

If you have to insert code in your document you have three choices:

1. inline code like this: `*Hello* **world!**"`
2. fenced code blocks (you may use ` ``` ` or `~~~`
   as delimiters):
```Bash
*Hello* **world!**
```
3. indented code blocks


    *Hello* 
    
    **world!**

You need to leave a blank line after a paragraph and 2 blank lines after a list to start an indented code block (if you want the code to be out of the list), and you may insert the name of the language immediatly after the opening code fence (so some renderers may be able to highlight the syntax of the language)

| Specification                | Requirement                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |   |
|------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---|
| Platform                     | vSphere 7.0 (up to 7.0 U31) vSphere 6.x vSphere 5.5 VMware Cloud Foundation (VCF) This platform is supported as individual VMware software components. VMware components listed on this page can be part of VCF. For the information on the correspondence of VMware components to the VCF version, see this VMware KB article. VMware Cloud on AWS VMware Cloud on Dell EMC Azure VMware Solution For more information on Azure VMware Solution support, see this Veeam KB article. |   |
| Hypervisor                   | ESXi 7.0 (up to 7.0 U31) ESXi 6.x ESXi 5.5 Free ESXi is not supported. Veeam Backup & Replication leverages vSphere and vStorage APIs that are disabled by VMware in free ESXi.                                                                                                                                                                                                                                                                                                      |   |
| Management Server (optional) | vCenter Server 7.0 (optional) (up to 7.0 U31) vCenter Server 6.x (optional) vCenter Server 5.5 (optional)                                                                                                                                                                                                                                                                                                                                                                            |   |

