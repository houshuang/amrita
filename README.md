#Amrita (Work in Progress)

[![Build Status](https://travis-ci.org/josephwilk/amrita.png?branch=master)](https://travis-ci.org/josephwilk/amrita)

A polite, well mannered and throughly upstanding testing framework for Elixir.

![Elixir of life](http://s9.postimg.org/uv0ubzjm7/elixir.jpg)


#Usage

```elixir
defmodule MathFacts do
  use Amrita.Sweet

  fact "arithmetic" do
    assert 1 + 1 == 2
  end

  facts "about substraction" do
    fact "positive numbers" do
      assert 1 - 1 == 0
    end

    fact "negative numbers" do
      assert -1 - -1 == 0
    end
  end
end
```

##License
(The MIT License)

Copyright (c) 2013 Joseph Wilk

Permission is hereby granted, free of charge, to any person obtaining
a copy of this software and associated documentation files (the
'Software'), to deal in the Software without restriction, including
without limitation the rights to use, copy, modify, merge, publish,
distribute, sublicense, and/or sell copies of the Software, and to
permit persons to whom the Software is furnished to do so, subject to
the following conditions:

The above copyright notice and this permission notice shall be
included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.