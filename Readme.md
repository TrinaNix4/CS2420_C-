# kinds of applications

- phone and other client apps (including windows) including games
- console appications
- services
- servers
- libraries

console applications are the simplest 

- write text to the screen
- read text from the keyboard
- no graphics, no controls  

# Language Basics - Variables

- C++ is a strongly typed language
  - variables can hold only certain types of values 

  - must declare variables before they're used; cannot change type 

  - fundamental types built into the language 
  - numbers, boolean, single characters 

  # User defined types 

  - strings , dates, business objects

  - structs and classes let you define types; 

  # user defined types are full participants in the language  - this sets C++ apart from other languages

  # fundamental types of variables

  - integers
    - short, long, int

  - real numbers
    - float, double 

  - character
    - char, unsigned char


  - boolean (true/false)
    - bool 

  
  # auto 

  asks teh compiler to deduce the type; 

  - in this case, variable is still strongly typed 

  - useful for ugly declarations; use it when it makes things easier to read or understand 


 # casting

 compiler will convert types;  e.g. convert int into double (generally will warn you if data will be lost - truncation)

 by casting, you make your intention clear; 

 this can backfire; logic error can still be present even though warning goes away

 always use safe casts; 

 never use round-bracket casts;

 can use suffixes to show type of a literal; 

 ```

//int i5 = d1; 
int i5 = static_cast<int>(d1); 
 // <> used around the type we want to cast to
 // () around the value you want to cast 

 ```

 * suppress the warning of any lost data by putting in the explicit cast


 # summary 

 - variables have a type and must be declared before they're used

 - different types hold different kinds of data 

    * have different lengths and maximum values 
    * compiler knows all the rules and will help you with warning and errors

- be aware that overflow can happen silently; ()
  * avoid using very small types l9ike char for numbers

* to tell compiler you know what you're doing, use a safe cast 
 - when you want to go back and forth between different types, tell the compiler you're doing it on purpose and the warnings will be suppressed

 # language basics - user defined types

 - building an app- 
  - you can make the compiler a promise; 
  - linker will ensure it is kept . makes the ocnnection between the code that uses the class, and the code that implements it

  - #include only a convenience 
   - pastes another file into source file 
  - generally called header file .h

  - put each class in its own file 

# classes and objects

syntax for declaring

class keyword;

has public and private sections; 
  - by default they will be private 
  - good practice not to have public 

declare like fundamental types; 
(e.g. Person p)  
- access these member with . operator

e.g. 

```
class Person {
  private:
    std::string firstname;
    std::string lastname; 
    int phoneNumber; 

  public:
    std::string getName();
    };

    ```

    - keyword class introduces the declaration
    - brace brackets surround the contents
    - member variables are generally private 

  