tuncs_cpp_style_guide
=====================

Name Conventions
----------------
~~~~~~cpp
// FileName.h
namespace name {

class CppClass
{
public:
  void compute_foo();
  auto compute_foo_variation() -> void;
  
  int id() {return _id;}
private:
  int _id;
  
  void _compute_internal();
};

}
~~~~

Editor Style
------------
* Tabs are converted to spaces: 1 tab = 4 space.

Include Order
-------------
* From external to internal with grouping:

~~~~~~cpp
#include <iostream>
#include <vector>
#include <map>

#include <boost/config/warning_disable.hpp>
#include <boost/spirit/include/qi.hpp>
#include <boost/spirit/include/phoenix_core.hpp>
#include <boost/spirit/include/phoenix_operator.hpp>
#include <boost/spirit/include/phoenix_stl.hpp>

#include <include/mylib/mylib1.h>
#include <include/mylib/mylib2.h>

#include "myheader1.h"
#include "myheader2.h"
~~~~

* use '/' as the directory seperator.
