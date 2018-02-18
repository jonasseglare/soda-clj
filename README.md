# Soda&mdash;Stack Oriented Data API

These are the Clojure Soda bindings. Soda is a simple data-oriented API
that C++ programs can expose to make it easy for other languages to call
them. See the related CMake project [soda-cpp](https://github.com/jonasseglare/soda-cpp) that can be used by C++ code to expose a Soda API and be callable
from Clojure.


## Usage

1. Install [soda-cpp](https://github.com/jonasseglare/soda-cpp) (See the readme of that project). Note in particular where ```libsoda.so``` gets installed.

2. Write your C++ code so that it exposes a Soda API, see for instance [the example code](cpp_example/) where there is a ```Makefile```.

3. Compile the C++ code to a shared library and put it somewhere the JNA can find it (e.g. under [resources/](resources/).


## License

Copyright © 2018 Jonas Östlund

Distributed under the Eclipse Public License either version 1.0 or (at
your option) any later version.
