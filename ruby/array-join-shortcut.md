# Shortcut for `Array#join`

To join array elements just multiply it by a string.

```ruby
[1, 2, 3, 4, 5] * ','         # => "1,2,3,4,5"
['one', 'two', 'three'] * '-' # => "one-two-three"
%w(a b c d e f g) * ', '      # => "a, b, c, d, e, f, g"
%i(hello world) * ' '         # => "hello world"
```
