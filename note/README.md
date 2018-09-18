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
