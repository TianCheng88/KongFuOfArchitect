## c++ 编程

C++是一种静态类型化、编译化、通用性、大小写敏感、自由格式编程语言，支持过程性、面向对象和泛型编程。
C++被视为一种中级语言，因为它包括高级语言和低级语言功能的组合。
C++由 `Bjarne Stroustrup` 于1979年在新泽西州默里山的贝尔实验室开发，作为C语言的加强版，最初命名为C类，但后来于1983年更名为C++。
> 在编译期间执行类型检查时，称为编程语言使用静态类型，而不是运行时。

### 面向对象编程

`C++` 支持面向对象的编程，包括面向对象的开发四大支柱 |

- 封装
- 数据隐藏
- 继承
- 多态

### 标准库

标准C++由三个重要部分组成：

- 提供所有构建基块的核心语言，包括变量、数据类型和字面量等
- `C++`库，提供一组丰富的函数，用于操作文件、字符串等。
- 标准模板库 （`STL`） 提供一组丰富的方法来操作数据结构等。

### `ANSI` 标准

`ANSI` 标准是为了确保其 `C++` ;您为 `Microsoft` 编译器编写的代码将编译时没有错误，
使用 `Mac`、`UNIX`、`Windows box` 或 `Alpha` 上的编译器。 `ANSI` 标准已经稳定了一段时间，所有主要的C++制造商都支持 `ANSI` 标准。

### 学习 C++ 

学习时最重要的是`C++`概念。 学习编程语言的目的是成为一个更好的程序员;也就是说，在设计和实施新系统以及维护旧系统方面更加有效。

c++ 支持多种编程风格，你可以使用 `Fortran` 风格，`C`, `Smalltalk` 等风格。每种样式都可以有效地实现其目标，同时保持运行时和空间效率。

### 使用 C++

C++被几十万程序员用于本质上的每个应用程序领域。
C++被高度用于编写设备驱动程序和其他软件，这些软件依赖于在实时约束下直接操作硬件。
C++广泛用于教学和研究，因为它足够干净，足以成功教授基本概念。
任何使用过` Apple Macintosh` 或运行 `Windows` 的 `PC` 的人都间接接触过 `C++` ，因为这些系统的主要用户界面是用C++。

### 环境

#### 文本编辑器

#### 编译器

这是一个C++编译器，将用于将源代码编译为最终的可执行程序。
大多数C++编译器都不关心您向源代码提供什么拓展名，但如果您没有指定其他方式，默认的形式是`.cpp`。
最常用的和免费可用的编译器是 `GNU C/C++` 编译器，否则，如果您有相应的操作系统，则可以使用来自 `HP` 或 `Solaris` 的编译器。 
 
##### 安装编译器

###### UNIX/LINUX 

如果您使用的是 `Linux` 或 `UNIX`，则通过从命令行输入以下命令来检查系统上是否安装了 `GCC` | 

```bash 
$ g++ -v
```

如果您已经安装了 `GCC`，则它应该打印如下类似的消息 |

```text
Using built-in specs.
Target: i386-redhat-linux
Configured with: ../configure --prefix=/usr .......
Thread model: posix
gcc version 4.1.2 20080704 (Red Hat 4.1.2-46)
```

如果未安装 `GCC`，则您必须使用此处提供的详细说明 https://gcc.gnu.org/install/

###### macosX 

如果您使用 Mac OS X，获取 `GCC` 的最简单方法是从 `Apple` 网站下载 `Xcode` 开发环境，并按照简单的安装说明进行操作。
 `Xcode` 当前在 `developer.apple.com/technologies/tools/`。
 
###### windows

若要在 `Windows` 上安装 `GCC`，您需要安装 `MinGW`。
要安装 `MinGW`，请转到 `MinGW` 主页，`www.mingw.org`，然后按照 `MinGW` 下载页面的链接进行。
下载最新版本的 `MinGW` 安装程序，该程序应命名为 MinGW-&lt;版本&gt;.exe。 

安装 `MinGW` 时，至少必须安装 `gcc` 核心、`gcc-g+`、`binutils` 和 `MinGW` 运行时（`runtime`），但您可能希望安装更多。
将 `MinGW` 安装的 `bin` 子目录添加到 `PATH` 环境变量中，以便可以通过命令行中的简单名称指定这些工具。
安装完成后，您将能够从 `Windows` 命令行运行 `gcc`、`g+`、`ar`、`ranlib`、`dlltool` 和其他几个 `GNU` 工具。
  
  
### 基础语法

当我们想到C++程序时，它可以定义为通过调用彼此的方法进行通信的对象的集合。
现在，让我们简要地了解一个类、对象、方法和即时变量意味着什么。


- 对象

对象具有状态和行为。示例：狗有状态 - 颜色，名称，品种以及行为 - 摇尾巴，吠，饮食。对象是类的实例。

- 类

类可以定义为模板/蓝图，用于描述其类型支持的对象的行为/状态。

- 方法

方法基本上是一种行为。类可以包含许多方法。它存在于编写逻辑、操作数据和执行所有操作的方法中。

- 即时变量

每个对象都有其唯一的实例变量集。对象的状态由分配给这些实例变量的值创建。



一个简单的c++ 代码文件示例：


[hello](./c++_basic/hello.cpp)

请看该代码的几个部分的内容：

- C ++语言定义了几个标头，其中包含对程序必要或有用的信息。`<iostream>` 是必要的头部。
- 该行`using namespace std`;告诉编译器使用std命名空间。命名空间是C ++中相对较新的功能。
- 下一行'// main（）是程序开始执行的地方。 是C ++中可用的单行注释。 单行注释以//开头，并在该行的结尾处停止。
- `int main()`行是程序执行开始的主要函数。
- 下一行`cout <<“ Hello World”;`使消息“ Hello World”显示在屏幕上。
- 下一行`return 0`；终止 `main()` 函数并使它返回值 0 到调用进程。


确保 `g++` 在您的环境变量中，并且正在包含文件 `hello.cpp` 的目录中运行它。
您可以使用 [`makefile`](https://www.tutorialspoint.com/makefile/index.htm) 编译 `C/C++` 程序。 

### C ++中的分号和作用域

在C ++中，分号是语句终止符。
也就是说，每个单独的语句必须以分号结尾。
它表示一个逻辑实体的结尾。
例如，以下是三个不同的语句-

```c++
x = y;
y = y + 1;
add(x, y);
```

作用域是一组逻辑连接的语句，由开括号和闭括号包围。
例如:

```c++
{
   cout << "Hello World"; // prints Hello World
   return 0;
}
```

`C++` 无法将行尾识别为终止符。
因此，将语句放在一行中都没有关系。
例如-你也可以这么些：

```c++
x = y; y = y + 1; add(x, y);
```
### `C++` 标识符

C ++标识符是用于标识变量，函数，类，模块或任何其他用户定义项的名称。
标识符以字母`A`到`Z`或`a`到`z`或下划线（`_`）开头，后跟零个或多个字母，下划线和数字（0到9）。
`C++` 不允许在标识符内使用标点符号，例如`@`，`$`和`％`。
`C++` 是区分大小写的编程语言。
因此，`Manpower` 和 `manpower`  是 `C++` 中的两个不同的标识符。

这是可接受的标识符的一些示例-

```text
mohd       zara    abc   move_name  a_123
myname50   _temp   j     a23b9      retVal
```
### `C++` 关键字

以下列表显示了 `C++` 中的保留字。
这些保留字不得用作常量或变量或任何其他标识符名称。
```text
asm  	else	new     	this
auto	enum	operator	throw
bool	explicit	private	true
break	export	protected	try
case	extern	public	typedef
catch	false	register	typeid
char	float	reinterpret_cast	typename
class	for	    return	union
const	friend	short	unsigned
const_cast	goto	signed	using
continue if	sizeof	virtual
default	inline	static	void
delete	int 	static_cast	volatile
do	    long	    struct	wchar_t
double	mutable	switch	while
dynamic_cast	namespace	template	
```
### 三字符组

一些字符具有另一种表示形式，称为三字符组序列。
三字符组是一个由三个字符组成的序列，代表一个字符，该序列始终以两个问号开头。
三字符组会延展到它们出现的任何位置，包括在字符串文字和字符文字中，在注释中以及在预处理程序指令中。



|  三字符组 | 置换 |
| ------------ | ------------ |
| `??/`  | `\` |
| `??'`  | `^` |
| `??(`  | `[` |
| `??)`  | `]` |
| `??!`  |  |  |
| `??<`  | `{` |
| `??>`  | `}` |
| `??-`  | `~` |

所有的编译器都不支持三字符组，并且由于其混乱的性质，不建议使用它们。

### `C++` 中的空格

仅包含空格（可能带有注释）的行称为空白行，而 `C++` 编译器完全忽略它。
空格是 `C++` 中用来描述空格，制表符，换行符和注释的术语。
空格将语句的一部分与另一个部分分开，并使编译器能够识别语句中一个元素（例如`int`）在何处结束以及下一个元素在何处开始。

语句1：

```c++
int age;
```

在上面的语句中，`int` 和 `age` 之间必须至少有一个空格字符（通常为空格），以便编译器能够区分它们。

语句2：

```c++
fruit = apples + oranges;   // Get the total fruit
```

在上面的语句2中，在`fruit`和`=`号之间，或在`=`号和`apples`之间，不需要空格字符，尽管出于可读性考虑，您可以自由地添加一些字符。

### 注释

程序注释是可以包含在 `C++` 代码中的说明性语句。
这些注释可帮助任何人阅读源代码。
所有编程语言都允许使用某种形式的注释。

`C++` 支持单行和多行注释。
`C++` 编译器将忽略任何注释中可用的所有字符。
`C++` 注释以 `/*` 开头，以 `*/` 结尾。
例如-

```c++
/* This is a comment */

/* C++ comments can also
* span multiple lines
  */
```

注释也可以以 `//` 开头，延伸到该行的末尾。
例如-

[代码](./c++_basic/hello.cpp)

编译以上代码时，它将忽略`//`打印 `Hello World` ，最终可执行文件将产生以下结果-

```text
Hello World
```

在 `/*` 和 `*/` 注释中，`//` 字符没有特殊含义。
在 `//` 注释中，`/*` 和 `*/` 没有特殊含义。
因此，您可以在另一种注释中“嵌套”一种注释。
例如-

```c++
/* Comment out printing of Hello World:

cout << "Hello World"; // prints Hello World

*/
```

## `C++` 变量

用任何语言编写程序时，您需要使用各种变量来存储各种信息。
变量不过是用于存储值的保留内存位置。
这意味着在创建变量时，您会在内存中保留一些空间。
您可能希望存储各种数据类型的信息，例如字符，宽字符，整数，浮点数，双浮点数，布尔值等。
操作系统根据变量的数据类型分配内存，并确定那些可以存储于剩余的内存。

###  原始内置类型

`C++` 为程序员提供了丰富的内置以及用户定义的数据类型。
下表列出了七种基本的 `C++` 数据类型-

|  类型 |  关键字 |
| ------------ | ------------ |
| Boolean  | bool  |
| Character  | char  |
| Integer | int  |
| Floating point  | float  |
| Double floating point  |  double |
| Valueless  | void  |
| Wide character	  |  wchar_t |
|   |   |


可以使用一个或多个这些类型修饰符来修改几种基本类型-

- signed
- unsigned
- short
- long

下表显示了变量类型，在内存中存储值所需的内存量以及此类变量中可以存储的最大值和最小值。

| 类型  |  典型位宽 |  典型范围 |
| ------------ | ------------ | ------------ |
| char	 | 1byte  | -127 to 127 or 0 to 255  |
|  unsigned char |  1byte |  0 to 255 |
| signed char  | 1byte  | -127 to 127  |
|  int | 4bytes  | -2147483648 to 2147483647  |
| unsigned int  |  4bytes |  0 to 4294967295 |
| signed int  |  4bytes |  -2147483648 to 2147483647 |
| short int  | 2bytes  | -32768 to 32767  |
| unsigned short int  | 2bytes  |  0 to 65,535 |
| signed short int  | 2bytes  | -32768 to 32767  |
|  long int |  8bytes | -2,147,483,648 to 2,147,483,647  |
| signed long int  | 8bytes  | same as long int  |
| unsigned long int  |  8bytes | 0 to 4,294,967,295  |
|  long long int |  8bytes | -(2^63) to (2^63)-1  |
|  unsigned long long int	 | 8bytes  | 0 to 18,446,744,073,709,551,615  |
| float  | 4bytes  |   |
| double  | 8bytes  |   |
| long double  |  12bytes |   |
| wchar_t  |  2 or 4 bytes | 1 wide character  |

变量的大小可能不同于上表中显示的大小，具体取决于所使用的编译器和计算机。
以下是示例，它将在您的计算机上生成正确大小的各种数据类型：

[代码](./c++_basic/data_type.cpp)

此示例使用 `endl`，它在每行之后插入一个换行符，并且 `<<` 操作符用于将多个值传递到屏幕。
我们还使用 `sizeof()` 运算符来获取各种数据类型的大小。
编译并执行上述代码后，将产生以下结果，该结果可能因计算机而异-


```text
 
## windows 10 :
size of char is :1
size of int is :4
size of short int is :2
size of long int is :4
size of float is :4
size of double is :4
size of wchar_t is :4
```

### `typedef` 声明

您可以使用 `typedef` 为现有类型创建新名称。
以下是使用 `typedef` 定义新类型的简单语法-

```c++
typedef type newname; 
```

例如，以下内容告诉编译器，`feet` 是 `int` 的另一个名称-

```c++
typedef int feet;
```

现在，以下声明完全合法，并创建一个称为 `distance` 的整数变量

```c++
feed distance;
```
[实例代码](./c++_basic/type_def.cpp)

### 枚举类型

枚举类型声明一个可选的类型名称，以及一组零个或多个可以用作该类型值的标识符。
每个枚举数都是一个常量，其类型为枚举。
创建枚举需要使用关键字 `enum` 。
枚举类型的一般形式是-

```c++
enum enum-name { list of names } var-list; 
```

在这里，枚举名称是枚举的类型名称。
名称列表以逗号分隔。
例如，以下代码定义了称为 `color` 的颜色和 `color` 类型的变量 `c` 的枚举。
最后，为`c`分配值“ `blue`”。

```c++
enum color { red, green, blue } c;
c = blue;
```

默认情况下，第一个名称的值为 `0`，第二个名称的值为 `1`，第三个名称的值为 `2`，依此类推。
但是您可以通过添加一个初始化程序来提供一个名称，一个特定的值。
例如，在下面的枚举中，绿色的值为 `5`。

```c++
enum color { red, green = 5, blue };
```
在这里，`blue` 的值为6，因为每个名称都比其前一个大一个。

[示例代码](./c++_basic/enum_type.cpp)

### 变量类型

变量为我们提供了程序可以操纵的命名存储。
`C++` 中的每个变量都有一个特定的类型，该类型确定变量的内存大小和布局。
可以存储在该内存中的值的范围；
以及可以应用于该变量的一组操作。

变量的名称可以由字母，数字和下划线字符组成。
它必须以字母或下划线开头。
大写和小写字母是不同的，因为 `C++` 区分大小写-

如上一章所述，`C++` 中的变量具有以下基本类型-

| 类型   |  描述  |
| ------------ | ------------ | 
| bool |  存储值 `true` 或 `false` 。 |
| char |  通常是一个八位位组（一个字节）。这是整数类型。 |
| int | 机器最自然的整数大小。  |
| float | 单精度浮点值。  |
| double  |  双精度浮点值。 |
| void  | 表示没有类型。  |
| wchar_t |  宽字符类型。 |

`C++` 还允许定义各种其他类型的变量，我们将在后续章节中介绍这些变量，
例如枚举，指针，数组，引用，数据结构和类。
下一节将介绍如何定义，声明和使用各种类型的变量。

## `C++` 中的变量定义

变量定义告诉编译器在何处以及为变量创建多少存储空间。
变量定义指定一种数据类型，并包含一个或多个该类型变量的列表，如下所示：

```c++
type variable_list;
```

在这里，`类型`必须是有效的 `C++` 数据类型，
包括 `char` ，`w_char`，`int`，`float`，`double`，`bool` 或任何用户定义的对象等，
并且 `variable_list` 可能包含一个或多个标识符名称，以逗号分隔。
一些有效的声明显示在这里-

当前行 `int i，j，k;`
都声明并定义变量 `i，j` 和 `k`；
它表示编译器创建名为`int`的 `i，j` 和 `k` 变量。
变量可以在其声明中进行初始化（分配初始值）。
初始化程序由一个等号和一个常量表达式组成，如下所示：

```c++
extern int d = 3, f = 5;    // declaration of d and f. 
int d = 3, f = 5;           // definition and initializing d and f. 
byte z = 22;                // definition and initializes z. 
char x = 'x';               // the variable x has the value 'x'.
```

对于没有初始化程序的定义：具有静态存储持续时间的变量隐式初始化为 `NULL`（所有字节的值均为 `0`）；
所有其他变量的初始值是不确定的。

### C++ 变量声明

变量声明为编译器提供了保证，即存在一个具有给定类型和名称的变量，因此编译器可以继续进行进一步的编译，而无需有关该变量的完整详细信息。
变量声明仅在编译时具有其含义，编译器在程序链接时需要实际的变量定义。
当您使用多个文件，并且在其中一个文件中定义变量时，变量声明很有用。在程序链接时，这些文件之一将可用。
您将在任何地方使用 `extern` 关键字声明变量。
尽管您可以在 `C++` 程序中多次声明变量，但是只能在文件，函数或代码块中定义一次。

请尝试以下示例，其中变量已在顶部声明，但已在 `main` 函数内部定义-

[代码](./c++_basic/variable_declaration.cpp)

编译并执行上述代码后，将产生以下结果-

```c++
30
23.3333
```

相同的概念适用于函数声明，在声明函数时您要提供函数名称，而其实际定义可以在其他任何地方给出。
例如-

[代码](./c++_basic/func_declaration.cpp)

### 左值和右值

C ++中有两种表达式-

- 左值：

引用内存位置的表达式称为“左值”表达式。
左值可能显示为分配的左侧或右侧。

- 右值：

术语“右值”是指存储在内存中某个地址处的数据值。
一个右值是一个不能为其赋值的表达式，这意味着一个右值可能出现在赋值的右手而不是左手。

变量是左值，因此可能出现在赋值的左侧。
数字文字是右值，因此可能无法赋值并且不能出现在左侧。
以下是有效的声明-

```c++
int g = 20;
```

但是以下内容不是有效的语句，并且会生成编译时错误-

```c++
10 = 20;
```
### C++ 作用域

作用域是程序的一个区域，从广义上讲，可以在三个地方声明变量-
- 在函数或称为内部变量的块中，
- 在函数参数的定义中称为形式参数。
- 在所有函数之外，这称为全局变量。
- 在随后的章节中，我们将学习什么是函数及其参数。
在这里，让我们解释什么是局部变量和全局变量。
  
#### 局部变量

在函数或块内声明的变量是局部变量。
它们只能由该函数或代码块中的语句使用。
局部变量在其自身之外的函数中是未知的。
以下是使用局部变量的示例-

[代码](./c++_basic/local_variable.cpp)

#### 全局变量

全局变量是在所有函数之外定义的，通常在程序顶部。
全局变量将在程序的整个生命周期内保持其值。
全局变量可以由任何函数访问。
也就是说，在声明之后，全局变量可在整个程序中使用。
以下是使用全局和局部变量的示例-

[代码](./c++_basic/global_variable.cpp)

程序的局部变量和全局变量可以具有相同的名称，但是函数内局部变量的值将优先。
例如-

[代码](./c++_basic/preferential_variable.cpp)

编译并执行上述代码后，将产生以下结果-

```c++
10
```
#### 初始化局部变量和全局变量

定义局部变量后，系统不会对其进行初始化，您必须自己对其进行初始化。
如下定义全局变量时，系统将自动初始化全局变量-

| 数据类型  | 初始化  |
| ------------ | ------------ |
| int  | 0  | 
| char  | '\0'  | 
|  float |  0 | 
| double  | 0  | 
| pointer  |  NULL | 


正确初始化变量是一种好的编程习惯，否则有时程序会产生意外的结果。


### 常量和字面量

常数是指程序不能更改的固定值，它们称为**字面量**。
常量可以是任何基本数据类型，并且可以分为整数，浮点数字，字符，字符串和布尔值。
同样，常量的处理方式与常规变量相同，只是其值在定义后无法修改。

#### 整型字面量

整型字面量字可以是十进制，八进制或十六进制常量。
前缀指定基数或基数：十六进制为`0x`或`0X`，八进制为`0`，十进制为`0`。
整型字面量也可以具有后缀，该后缀是`U`和`L`的组合，分别表示`无符号`和`长整数`。
后缀可以是大写或小写，并且可以是任何顺序。
这是整型字面量的一些例子-

[代码](./c++_basic/int_literal.cpp)

#### 浮点型字面量

浮点型字面量具有整数部分，小数点，小数部分和指数部分。
您可以用十进制或指数形式表示浮点文字。
在使用小数形式表示时，必须包含小数点和/或指数，或者在使用指数形式表示时，必须包含整数部分，小数或这两者。
有符号数由`e`或`E`引入。这是浮点文字的一些示例-


[代码](./c++_basic/int_literal.cpp)


#### 布尔字面量

有两个布尔字面量，它们是标准`C++`关键字的一部分-表示`true`的`true`值。
代表`false`的`false`值。
您不应认为`true`的值等于`1`，`false` 的值等于 `0` 。

#### 字符字面量

字符字面量用单引号引起来。
如果字面量以`L`开头（仅大写），则为宽字符字面量（例如L'x'），应存储在变量的 `wchar_t` 类型中。
否则，它是一个狭窄的字符字面量（例如'x'），可以存储在 `char` 类型的简单变量中。
字符文字可以是普通字符（例如'x'），转义序列（例如'\t'）或通用字符（例如'\u02C0'）。
在 `C++` 中，当某些字符前面带有反斜杠时，它们将具有特殊含义，并且用于表示换行符（`\n`）或制表符（ `\t` ）。
在这里，您有一些此类转义序列代码的列表-


|  转义序列 |  含义 |
| ------------ | ------------ |
| \\  |  符号本身 |
| \'  |  符号本身 |
| \"  |  符号本身 |
| \?  |  符号本身  |
| \a  |  警报或铃声 |
| \b  |  退格键 |
| \f  |  换页 |
| \n  |  换行 |
| \r  |  回车 |
| \t  |  水平制表符 |
| \v  |  垂直制表符 |
| \ooo |  八位数字（一到三位数） |
| \xhh . . .  |  十六进制的一位或多位数字 |

以下是显示一些转义序列字符的示例-

#### 字符串字面量

字符串字面量是用双引号引起来的。
字符串包含与字符文字相似的字符：纯字符，转义序列和通用字符。
您可以使用字符串字面量将长行分成多行，并使用空格分隔它们。
以下是一些字符串文字的示例。
这三种形式都是相同的字符串。

[代码](./c++_basic/string_literal.cpp)

#### 定义常量

在 `C++` 中，有两种简单的方法可以定义常量-
- 使用 `#define` 预处理程序。
- 使用 `const` 关键字。

##### `#define`预处理程序

以下是使用 `#define` 预处理器定义常量的形式-

```c++
#define [标识符] [值]
```

以下示例详细解释-

[代码](./c++_basic/define_constants.cpp)

编译并执行上述代码后，将产生以下结果-

```c++
50
```

##### `const` 关键字

您可以使用 `const` 前缀来声明具有特定类型的常量，如下所示-

以下示例详细解释-

[代码](./c++_basic/define_constants.cpp)