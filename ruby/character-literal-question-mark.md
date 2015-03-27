# `?A` Character literal

You can define single-character strings by `?x` character literal.

`?x` syntax is equal to writing `"x"`:

```ruby
letter =  ?A
letter == 'A' # => true

case letter
  when ?A then puts 'My favorite letter!'
  when ?1 then puts 'You have typed "one"'
  when ?? then puts 'What was the question?'
end
```