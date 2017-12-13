## Welcome to Expect scripting Tutorial

The tutorial can be used as a reference while creating expect scripts



## Some of the basic commands used in Expect are 
*spawn*     Starting a script or a program.

*expect*    Waiting for program output.

*send*       Sending a reply to your program.

*interact*   Allowing you in interact with your program.

## Example 1:
** How to create a sample expect script **

```
#!/usr/bin/expect -f

set timeout -1
spawn root@remoteserver
expect "Password:"
send "****\r"
expect "#"
interact
```


#!/usr/bin/expect -f
> Guiding the interpreter to run it as expect program.

set timeout -1
> Setting the timeout to infinity 

spawn ssh root@remoteserver
> Run a program to perform a ssh to the remote server

expect "Password:"
> Expect a "Passoword:" prompt

send "****\r"
> Send the password, \r is carriage return (enter)

interact
> Terminal will be remained open for you to perform operations on remote server







### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/manoharendla/ExpectScriptExamples/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://help.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.
