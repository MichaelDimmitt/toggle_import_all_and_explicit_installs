# Research Spike: Toggle Import All and Explicit Installs
Javascript, Go, Java, other languages. looking for toggle on toggle off.

Javascript uses dereferencing, import {var1, var2} from 'module'; 
<br/>Javascript also supports bringing the whole object in import vars from 'module'

Go uses packages and will break if the same function is called.
<br/>Java uses packages. example: `import java.util.Scanner;` 

(Java example used because easy to grasp the need for this project) 
```java
import java.util.*;
```

Lets say you only use Scanner and Random from util,
<br/>The program should scan the code base and inside each file understand what classes and methods that package is using.

## Toggle on for this example:
```java
import java.util.Scanner;
import java.util.Random;
```

## Toggle off for this example:
```java
import java.util.*;
```

This is useful because with toggle off you can add usage of Timer and then when you toggle on it will automatically see it.
## Example Result:
```java
import java.util.Scanner;
import java.util.Random;
import java.util.Timer;
```

The main reason why this is needed is for package development in java outside an IDE.
<br/>Additionally in go development I was reading through source code that was hard to walk through 
<br/>because the paths that linked functions were not explicit.

## Toggle should always be off

## On addition of a new package <br/>Prompting occours turning toggle on and off again

## Causing package to be named automatically with functions dereferenced in Javascript like syntax.

IDEs already perform this action, I am looking for terminal add ons to cause toggle to always be off and full paths elucidated making code more readable and maintainable.
