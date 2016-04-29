# pprint

A pretty printing library for C++ containers.
This library was forked from [cxx-prettyprint](https://github.com/louisdx/cxx-prettyprint) which was written by Louis Delacroix.

## Synopsis

Simply by including this header-only library in your source file,
you can say `std::cout << x` for any container object `x`. Sensible
defaults are provided, but the behaviour (i.e. the delimiters) are
compile-time customizable to a great extent via partial specializiation.

## Usage

Just copy `include/pprint` and add `#include <pprint/pprint.h>` to your source file and make sure
that `pprint.h` is findable.

## Example

Some usage examples are provided by `example/ppdemo.cpp`.

Using GCC, compile with

```bash
$ g++ -W -Wall -pedantic -O2 -s ppdemo.cpp -o ppdemo -std=c++0x
$ g++ -W -Wall -pedantic -O2 -s ppdemo98.cpp -o ppdemo98
```

For the C++98/03-version, define `NO_TR1` to prevent any inclusion of
TR1 headers and to disable `std::tr1::tuple` support.

For details, please see the website https://github.com/rinatz/pprint.

## License

Boost Software License, Version 1.0.
