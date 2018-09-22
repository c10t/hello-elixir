# Note

## iex

- `$ iex` start interactive elixir
- `iex(1)> String.reverse "stressed"` 
- `iex(2)> h` helper list
- `iex> h IO` or `iex> h(IO)` help for I/O module
  + `iex> h IO.puts`
  + `iex> h IEx.configure`
- `iex> i 123` information about the value

## compile and run

- `$ elixir hello.exs`
  + **.exs**: run without compile
  + **.ex** : compile to binary

- `$ iex`
  + `iex> c "hello.exs"`

## pattern matching

- example 1
  + `iex> list = [1, 2, [3, 4, 5]]`
  + `iex> [a, b, c] = list`
  + `iex> a`
    * `1`
  + `iex> c`
    * `[3, 4, 5]`

- example 2
  + `iex> list = [1, 2, 3]`
  + `iex> [a, 2, b] = list`
  + `iex> b`
    * `3`
  + `iex> [a, 1, b] = list`
    * `** (MatchError) no match of right hand side value: [1, 2, 3]`

- example 3
  + `iex> [1, _, _] = [1, 2, 3]`
  + `iex> [1, _, _] = [1, "cat", "dog"]`
