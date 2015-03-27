# Link references in document footnotes

You can use link references to keep the text clean.

So instead of defining links inside text like this:

```markdown
Read about it in [SO Thread][http://stackoverflow.com/questions/1217088/what-does-mapname-mean-in-ruby], go check it out!
```

you can use reference (defined at the bottom of the document, like footnotes):

```markdown
Read about it in [SO Thread], go check it out!

...more text...

[SO Thread]: http://stackoverflow.com/questions/1217088/what-does-mapname-mean-in-ruby
```

You can even format the link title, or use additional "identifiers" for references (eg. if link title is ambiguous):


```markdown
Just [*google*] it!
Or click [here][open_struct_class] to see the docs.

[*google*]: https://www.google.com/
[open_struct_class]: [http://ruby-doc.org/stdlib/libdoc/ostruct/rdoc/OpenStruct.html]
```
