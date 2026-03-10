# Learning_Cpp_Basic_Facilities
The C++ programming language - Part II: Basic Facilities
## 6 Types and Declarations (Need to review)
### 6.1 The ISO C++ Standard
Each implementation must provide a specific, well-defined behavior for a construct and that behavior must be documented.

When writing real-world programs, it is usually necessary to rely on implementation-defined behavior. 

To maximize portability, it is wise to be explicit about what implementation-defined features we rely on and to isolate the more subtle examples in clearly marked sections of a program.

It is worth spending considerable time and effort to ensure that a program does not use something deemed unspecified or undefined by the standard.
#### 6.1.1 Implementations
A C++ implementation can be either hosted or freestanding (§iso.17.6.1.3).
#### 6.1.2 The basic source character set
The C++ standard and the examples in this book are written using the basic source character set called ASCII.

To use an extended character set for source code, a programming environment can map the extended character set into the basic source character set in one of several ways, for example, by using universal character names (§6.2.3.2).
### 6.2 Types
#### 6.2.1 Fundamental types
Arithmetic types (integral types (boolean, character, integer types), floating-point types), `void`, pointer types, reference types, user-defined types. 
#### 6.2.2 Booleans
#### 6.2.3 Character types
A char variable can hold a character of the implementation’s character set. For example: `char ch = 'a'`.
##### Signed and Unsigned characters:
##### Character literals: 
A character literal is a single character enclosed in single quotes, for example, `'a'` and `'0'`.

For example, if you are running on a machine using the ASCII character set, the value of '0' is 48. 
#### 6.2.4 Integer types
- Integer literals
- Types of integer literals
#### 6.2.5 Floating-point types
- Floating-point literals
#### 6.2.6 Prefixes and suffixes
#### 6.2.7 `void`
#### 6.2.8 Sizes
#### 6.2.9 Alignment
### 6.3 Declarations
Before a name (identifier) can be used in a C++ program, it must be declared. That is, its type must be specified to inform the compiler what kind of entity the name refers to.

A definition is a declaration that supplies all that is needed in a program for the use of an entity. In particular, if it takes memory to represent something, that memory is set aside by its definition.

There must always be exactly one definition for each name in a C++ program.
#### 6.3.1 The Structure of Declarations
we can consider a declaration as having five parts:
- Optional prefix specifiers (e.g., static or virtual)
- A base type (e.g., vector<double> or const int)
- A declarator optionally including a name (e.g., p[7], n, or ∗(∗)[])
- Optional suffix function specifiers (e.g., const or noexcept)
- An optional initializer or function body (e.g., ={7,5,3} or {return x;})

Except for function and namespace definitions, a declaration is terminated by a semicolon.

A specifier is an initial keyword, such as virtual (§3.2.3, §20.3.2), extern (§15.2), or constexpr (§2.2.3), that specifies some non-type attribute of what is being declared.

The postfix declarator operators bind tighter than the prefix ones. Consequently, char∗kings[] is an array of pointers to char, whereas char(∗kings)[] is a pointer to an array of char.
#### 6.3.2 Declaring Multiple Names
#### 6.3.3 Names
##### Keywords
#### 6.3.4 Scope
#### 6.3.5 Initialization
If an initializer is specified for an object, that initializer determines the initial value of an object. An initializer can use one of four syntactic styles:
```cpp
X a1 {v};
X a2 = {v};
X a3 = v;
X a4(v);
```
Of these, only the first can be used in every context, and I strongly recommend its use. It is clearer and less error-prone than the alternatives. 

Prefer `=` when using `auto`

The empty initializer list, `{}`, is used to indicate that a default value is desired. Most types have a default value. For integral types, the default value is a suitable representation of zero. For pointers, the default value is nullptr (§7.2.2). For user-defined types, the default value (if any) is determined by the type’s constructors (§17.3.3).
##### Missing Initializers
##### Initializer Lists
#### 6.3.6 Deducing a Type: auto and decltype()
##### The `auto` Type Specifier
When a declaration of a variable has an initializer, we don’t need to explicitly specify a type. Instead, we can let the variable have the type of its initializer. For example: `auto a3 = 123`. The type of `a3` is an `int`.

The harder the type is to write and the harder the type is to know, the more useful auto becomes.
##### `auto` and `{}`-lists
##### The `decltype()` Specifier
### 6.4 Objects and values
#### 6.4.1 Lvalues and Rvalues
#### 6.4.2 Lifetimes of Objects
### 6.5 Type aliases
### 6.6 Advice
