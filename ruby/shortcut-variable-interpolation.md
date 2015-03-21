# Shortcut variable interpolation

Curly braces are optional when interpolating the `@`, `@@` or `$` variables:

```ruby
@instance = 'instance'
@@class   = 'class'
$global   = 'global'

puts "#@instance, #@@class and #$global variables do not need curly braces"
```

Remember that `#` is still required :smile: See this [SO question] for an explanation.

[SO question]: http://stackoverflow.com/questions/10091156/why-does-string-interpolation-work-in-ruby-when-there-are-no-curly-braces
