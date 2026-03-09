# Learning_Cpp_Basic_Facilities
The C++ programming language - Part II: Basic Facilities
## 6 Types and Declarations
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
- Signed and Unsigned characters
- Character literals
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
#### 6.3.1 The Structure of Declarations
#### 6.3.2 Declaring Multiple Names
#### 6.3.3 Names
- Keywords
#### 6.3.4 Scope
#### 6.2.5 Initialization
- Missing Initializers
- Initializer Lists
#### 6.2.6 Deducing a Type: auto and decltype()
- The `auto` Type Specifier
- `auto` and `{}`-lists
- The `decltype()` Specifier
### 6.4 Objects and values
#### 6.4.1 Lvalues and Rvalues
#### 6.4.2 Lifetimes of Objects
### 6.5 Type aliases
### 6.6 Advice
