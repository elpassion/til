# Link references in document footnotes

You can use link references to keep the text clean.

So instead of defining links inside text like this:

```markdown
You can read about it more in this [SO Thread][http://stackoverflow.com/questions/1217088/what-does-mapname-mean-in-ruby],
go check it out! Or just [*google*][https://www.google.com/] it.
Also, we can just use [`OpenStruct`][http://ruby-doc.org/stdlib/libdoc/ostruct/rdoc/OpenStruct.html].
```

you can use reference (defined at the bottom of the document, like footnotes). You can even format the link title, or use additional "identifiers" for references.


```markdown
You can read about it more in this [SO Thread], go check it out! Or just [*google*] it.
Also, we can just use [`OpenStruct`][open_struct_class].

[SO Thread]: http://stackoverflow.com/questions/1217088/what-does-mapname-mean-in-ruby
[*google*]: https://www.google.com/
[open_struct_class]: [http://ruby-doc.org/stdlib/libdoc/ostruct/rdoc/OpenStruct.html]
```