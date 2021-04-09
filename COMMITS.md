# WRITING GOOD COMMITS

### What is good?

1. A good commit message is detailed.
2. It focusses on the why more than the what or the how. What do you do is tracked by Git already. How do you do it is visible to the reader in your code already. 


### Use the editor method to write commits 

We are used to writing: 
```bash 
git commit -m "a message"
```
Avoid that.

Just run `git commit` and it will open up an editor.
 
To configure your "default" editor:
```bash
git config --global core.editor <name>

# name could be nano/emacs/vim/whatever you like
```

### Writing in the editor

A good commit message is broken down into three parts.

the top 
< line break >
the middle 
< line break >
the bottom 
 
the top 
should follow the format:
\<type\>:\<summary or the subject line\> 

where type is:

    feat: The new feature you're adding to a particular application
    fix: A bug fix
    style: Feature and updates related to styling
    refactor: Refactoring a specific section of the codebase
    test: Everything related to testing
    docs: Everything related to documentation
    chore: Regular code maintenance. 

The net length of the top should not be more than 50 characters.

Do not end the subject line with a period.

the middle (or the body)
Elaborate your work.Do not assume the reviewer understands what the original problem was, ensure you add it. Do not think your code is self-explanatory.

the bottom 
this is optional. Use it if you want to link this commit to an issue. 