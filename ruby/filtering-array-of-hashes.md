```ruby
hashes = [
    { "id" => 1 },
    { "id" => 2 },
    { "id" => 3 },
    { "id" => 4 },
    { "id" => 5 },
]

ids = [1, 3, 4]

# PROBLEM: Filter hashes by given ids

def naive_filter(hashes, ids)   # O(n*k)
    hashes.select do |hash|
        ids.include? hash["id"]
    end
end

def filter(hashes, ids)         # O(n+k)
    ids_map = Hash[ids.map { |id| [id, true] }]
    
    hashes.select do |hash|
        ids_map[hash["id"]]
    end
end
```
