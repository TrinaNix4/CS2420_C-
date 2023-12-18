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

 