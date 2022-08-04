# Development Wiki 🖥

This a guide for development best practices.


- English for everything! Code, commit messages, issues, tickets etc...
- Simplicity is key, avoid "overengineering", solve one problem at the time. 
- Test! if a piece of code will affect an end user it needs to be tested.
- Rely on tools to keep your code linted and according to a style guide.
- There's only one way of doing things: The right way.
- Remember: Single Responsibility and Do Not repeat Yourself
- Pull Request your work, two heads think better than one
- Commit and push your code at least once a day, anything can happen tomorrow.


## Definition of Done
 1. Tested by code and human
 2. Approved by a Pull Request 
 3. Accomplishes the ticket definition
 
 ---

## Resources

**Index**

+ [git](#git)
+ [Post-Mortems](Post-Mortems)
---

### **git**

#### **Run `rubocop` on pre commit:**
Rename `.git/hooks/pre-commit.sample` to `.git/hooks/pre-commit` with the following contents:


```
#!/usr/bin/env bash
echo "Running pre-commit hook"
bundle exec rubocop
# $? stores exit value of the last command
# 0 = Success
if [ $? -ne 0 ]; then
 echo "Oops, clean your code before committing!"
 exit 1
fi
```

`git` will now run this script everytime the user attempts to commit checking whether or not `rubocop` succeeds.
