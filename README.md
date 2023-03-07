# Sequence

>
>Akala ko pindot-pindot lang.
>
> -me


---

## Table of Contents
- [main()](#main)
- [variables](variables)
- [printing "Hello World"](#print)
- [include](#include)
- [math operators](#math)
- [increment and decrement](#inc)



---

## <a id="main">main()</a>
Lahat ng C++ programs merong main function.

```cpp
void main(){}
//minimum, useless but runnable C++ program
```

Lahat lang nang nasa loob ng main() yung ma-eexecute. Pag nasa labas siya, either error or di gagana unless i-call sa loob ng main().

```cpp
cout<<"Hi";
void main(){

}
//Error
```

```cpp
void main(){
cout<<"Hi";
}
//Gumagana na
```

`Note: add 'using namespace std;' at the top if you are using a modern C++ compiler. The long and boring explanation can be found at `[namespaces]()`. For now, just add it.`



---

## <a id="variables">variables</a>
Para makastore tayo ng data sa computer, gagamit tayo ng variables.

`int` - for integers (negative to positive whole numbers only).

`float`/`double` - for fractional numbers (eg. 3.14).

`char` - for single character symbols (eg. 'A', '1', '$'). Should always be enclosed in single quotes (double quotes can be used on it using C string style, though it is not considered the best practice since there are better alternatives, which is...)

`string` - for long texts ("Hello World"). Should be enclosed in double quotes (but single quotes can still be used in certain circumstances. You can check out [arrays]() to learn more about it).




---

## <a id="print">printing "Hello World"</a>
Para makaprint, gagamit tayo ng `cout` with the operator `<<`.

```cpp
#include <iostream> //or <iostream.h> in turbo c++
using namespace std;

void main(){
cout<<"Hello World";
}

```

Paano ba gumagana yung `cout`? [Boring explanation]().

Ano yung `iostream`?



---

## <a id="include">include</a>
Para maka-connect ng separate na files sa C++, gagamit tayo ng include.

Kunwari merong kang program:

```cpp
#include <iostream> 
using namespace std;

string text = "Hello World";

void main(){
cout<<text;
}
//Output: Hello World
```





Pero gusto mo paghiwalayin. Magiging ganito:

`file1.cpp`
```cpp
string text = "Hello World";
```

`file2.cpp`
```cpp
#include <iostream> //arrows mean you're including a pre-installed library file
#include "file1.cpp" //double quotes mean you're including a local file
using namespace std;

void main(){
cout<<text;
}
//Output: Hello World
```




So basically, `iostream` is also just a C++ program to connect with your program so that you can print out stuffs in the console.



---

## <a id="math">math operators</a>
Para maka-compute tayo, gagamit tayo ng:

- `+` addition
- `-` subtraction
- `*` multiplication
- `/` division
- `%` remainder (modulo)

```cpp
#include <iostream>
using namespace std;

void main(){
int x=10;
int y=5;

cout << x+y; //10 + 5 = 15
cout << x-y; //10 - 5 = 5
cout << x*y; //10 x 5 = 50
cout << x/y; //10 ÷ 2 = 2
cout << x%y; //10 ÷ 2 = 0 remainder
}
```



---

## <a id="inc">increment and decrement</a>
The `++` operator basically just means `add 1`.

```cpp
int x=10;
cout << ++x; //11
```

But there is also a reversed one:
```cpp
int x=10;
cout << x++; //10  What? How?
```

Bakit 10?

Yung pinagkaiba ng `++x` at `x++` is that:

- `++x` is immediately added by 1.
- `x++` will only be added after the statement is finished (when it reaches the semicolon).

You can watch this short clip that helped me understand this.
[https://youtu.be/lJF0HBB_QvM](https://youtu.be/lJF0HBB_QvM).


---



## [Selection]()
