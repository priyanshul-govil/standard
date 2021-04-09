# CODING STYLE GUIDE

Much of this is inspired by Google's coding style guide for Java. I will try to keep this as concise as possible.

### Whitespace

Use spaces only, no tabs. Keep indentation of your code to 2-4 spaces. If you have a preference of using tabs, make sure that the editor that you use is configured to use map the tabs to spaces.

Maintain a single whitespace
1. After writing a reserved keyword such as `for`, `if`, `else`, `try`, `catch`. 
2. On both sides of the colon in an enhanced for ("foreach") statement
3. On both sides of any binary or ternary operator.

### Source file structure

Follow the section order: 

    Package statement
    Import statements
    Exactly one top-level class

Exactly one blank line separates each section that is present. Make sure that the import statements appear in lexicographically sorted order.

### Braces

Braces are used with `if`, `else`, `for`, `do` and while statements, even when the body is empty or contains only a single statement.

### Blocks

Braces follow the Kernighan and Ritchie style ("Egyptian brackets") for nonempty blocks and block-like constructs:

1. No line break before the opening brace.
2. Line break after the opening brace.
3. Line break before the closing brace.
4. Line break after the closing brace, only if that brace terminates a statement or terminates the body of a method, constructor, or named class. 

example:
```java

void doSomething() {
    doMoreWork();
    if (condition()) {
        workHere();
    }
    else {
        workThere();
    }
}
```
 
### For empty blocks: 
```java
// cool
void emptyBlock() {}

// cool
void emptyBlock() {
}

// not cool
void emptyBlock() {

}
```

### Intend blocks by 2 spaces.

Each time a new block or block-like construct is opened, the indent increases by two spaces. When the block ends, the indent returns to the previous indent level.

### Column limit: 100 characters

A "character" means any Unicode code point. Except as noted below, any line that would exceed this limit must be line-wrapped. (When code that might otherwise legally occupy a single line is divided into multiple lines, this activity is called line-wrapping.)

`package` and `import` statements are an exception to the above rule.

When line-wrapping, each line after the first (each continuation line) is indented at least +4 from the original line.

### Variables

One variable per declaration. Every variable declaration (field or local) declares only one variable: declarations such as int a, b; should be avoided. Exception: Multiple variable declarations are acceptable in the header of a for loop. 
 
Declare when needed. Local variables are not habitually declared at the start of their containing block or block-like construct. Instead, local variables are declared close to the point they are first used (within reason), to minimize their scope.

Avoid C-style arrays.
The square brackets form a part of the type, not the variable: String[] args, not String args[]

### Naming
Method and variable names: lowerCamelCase
Class names: UpperCamelCase
Constant names: All uppercase letters, with each word separated from the next by a single underscore.

### Comments

For single-line comments, use any form. (/\*...\*/ or //) 
 
For multi-line comments, just use /\*...\*/