# Wrap method around each Array element

You can wrap method around each Array element like this:

```ruby
[1, 2, 3].each &method(:puts)
```

This is equivalent to:

```ruby
[1, 2, 3].each { |number| puts number }
```

Actually, it's not only for *wrapping* Array elements. You can use any method (of any Class or Object) to pass it to any iterator like it were a block.

More fancy examples:

```ruby
%w(bar baz foo).any? &'foo'.method(:==)
%w(README.md CONTRIBUTING.md).map &File.method(:read)
```

PS. Note, that this might look similar to `array.map(&:to_s)`, but actually it's different.
