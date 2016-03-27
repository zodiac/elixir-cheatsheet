# elixir-cheatsheet

## String stuff

| Python 	| Elixir 	|
|-------- |--------	|
|`"a,b,c".split(',')` | `"a,b,c" |> String.split(",")`|
|`["a", "b"].join(",")` | `["a", "b"] |> Enum.join(",")`|


## Array slicing stuff

| Python 	| Elixir 	|
|-------- |--------	|
|`arr[0]` | `arr |> Enum.at(0)`|
|`arr[0:]` | `arr |> Enum.slice(1..-1)`|

## Functional stuff

| Python 	| Elixir 	|
|-------- |--------	|
|`[f(x) for x in xs]` | `xs |> Enum.map(fn x -> f x end)`|
|`[x for x in xs if p(x)` | `xs |> Enum.filter(fn x -> p x end)`|
