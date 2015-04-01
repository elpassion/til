#### Problem: Filtering array of hashes by given values

#### Sample input
```ruby
hashes = [
    { "id" => 1 },
    { "id" => 2 },
    { "id" => 3 },
    { "id" => 4 },
    { "id" => 5 },
]

ids = [1, 3, 4]

filter(hashes, ids) #=> [{"id"=>1}, {"id"=>3}, {"id"=>4}]
```

- With O(nk)
```ruby
def naive_filter(hashes, ids)
    hashes.select do |hash|
        ids.include? hash["id"]
    end
end
```

- With O(n+k)
```ruby
def filter(hashes, ids)
    ids_map = Hash[ids.map { |id| [id, true] }]
    
    hashes.select do |hash|
        ids_map[hash["id"]]
    end
end
```
