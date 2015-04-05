# `curry` Closure currying

When you have given closure, instead of calling it with two parameters,
```groovy
def stringMultiplier = { String string, int count ->
    return string * count
}
assert stringMultiplier.call('foo', 2) == 'foofoo'
```
you can pass one argument and save this closure for later using `curry`.
```groovy
def fooMultiplier = stringMultiplier.curry('foo')
assert fooMultiplier.call(2) == 'foofoo'
```
You can also pass specyfic parameter using `ncurry`.
```groovy
def stringDuplicator = stringMultiplier.ncurry(1, 2)
assert stringDuplicator.call('foo') == 'foofoo'
```

More examples: [`Closure (Groovy 2.4.3)`]
[`Closure (Groovy 2.4.3)`]: http://docs.groovy-lang.org/latest/html/api/groovy/lang/Closure.html#curry(java.lang.Object...)