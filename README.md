Makes printing stuff to console in C++ is just fun! be it anything, set, map, ... 


# printUtil
print all kinds of stl containers to console, debug recrsion by printing recursion call stack, plug and play C++ utlity
with 3 globally vailable void functions _w(), _e(), _b()

#### cout<< anything...(stl*)
![cout<< anything...(stl*)](https://github.com/Shubhambawner/printUtil/blob/main/Screenshot%20(305).png)

#### _w() Fnction
![recursion](https://github.com/Shubhambawner/printUtil/static/blob/main/Screenshot%20(307).png)

`output`
![_w() Fnction](https://github.com/Shubhambawner/printUtil/blob/main/Screenshot%20(306).png)

#### recursion tree
![_e() and _b() Fnction](https://github.com/Shubhambawner/printUtil/blob/main/Screenshot%20(310).png)
![_e() and _b() Fnction](https://github.com/Shubhambawner/printUtil/blob/main/Screenshot%20(308).png)


# _w print_stl_operator_overloaded
#### function _w() : overloads << os stream operator for printing all kinds of stl containers, if nested identifies the nesting and prints inner containers recursively
or in simple words, _w() prints anything and everything that is passed inn, space separated, after **spacing**
* feature: includes string **spacing**, that is also modified by recursive function

todo: cant print those containers initialised with custom compare functions, 
so, containers like : set<int, decltype(somefunction)*> cant be printed yet


# recursion_utilities: _e() and _b()
functions:
#### recurse() or _r(): increments spacing, passes all args passed to _w()
#### returnrecurse() or _b(): decrements spacing, passes all args passed to _w()
these fns use verdiac macros to get the name of calling function to be printed to console.

----------------------------------------------------------------
