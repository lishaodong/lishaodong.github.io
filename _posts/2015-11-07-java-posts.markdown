---
layout: post
title:  "Java Notes (1)"
date:   2015-11-07 21:54:10
categories: java
---

use


````
if(variable==null)
  throw new NullPointerException()
````

to prevent null variable. If you don't do this, and use variable.filed.subfield.method().field. you will never know  which is null.


do not let the reviewer guess what you are doing.
For example, a bVariable is boolean. write in this way.

````
if(bVariable==true)
  ...
else if(bVariable==false)
  ...
````

Yes, it's redundant, but make it easier to read.never use short names for variables, methods, use the long full name.

read lines without third-party library.

List<String> lines = Files.readAllLines(Paths.get(fileName), Charset.defaultCharset());
