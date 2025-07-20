# map-nelua

Macro function to inline hashmap instantiation

## Requirements
- [nelua](https://nelua.io/)

## How to install
Copy `map.nelua` into your project and require normally or add to your [nlpm](https://github.com/kmafeni04/nlpm) package dependencies
```lua
{
  name = "map-nelua",
  repo = "https://github.com/kmafeni04/map-nelua",
  version = "COMMIT-HASH-OR-TAG",
},
```

## Quick start

```lua
require "map"
local map = map!(string, string, {
  first_name = "John",
  last_name = "Doe"
})

print(map["first_name"]) --> John
```

## Reference

### map macro

See the nelua [hashmap-doc](https://nelua.io/libraries/#hashmap-1) for more information
`vals` must be a lua table of type `{K:V}`

```lua
## function map(K, V, vals, HashFunc, KeyEqualFunc, Allocator)
```

