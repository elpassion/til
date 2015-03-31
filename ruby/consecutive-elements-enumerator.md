# Array of Arrays of *n* consecutive elements

If you want to get an Array of Arrays of *n* consecutive elements (like `[[1, 2, 3], [2, 3, 4], [3, 4, 5]]`), you can use [`Enumerable#each_cons`][each_cons] on Range or Array:

```ruby
(1..6).each_cons(3) { |array| p array }

# Outputs:
[1, 2, 3]
[2, 3, 4]
[3, 4, 5]
[4, 5, 6]
```

Use [`Enumerable#to_a`][to_a] to get an Array and not an Enumerator.

```ruby
%w(a b c d).each_cons(2).to_a

# Outputs:
[["a", "b"], ["b", "c"], ["c", "d"]]
```

[each_cons]: http://ruby-doc.org/core/Enumerable.html#method-i-each_cons
[to_a]: http://ruby-doc.org/core/Enumerable.html#method-i-to_a