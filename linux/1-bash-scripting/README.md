<h1 align="center">
Bash scripting

<img src="assets/bash.jpg" alt="Tools" width="300">
</h1>
<br>

# What is bash?

Bash is a scripting language that runs within the terminal on most Linux distros, as well as MacOS. Shell scripts are a sequence of bash commands within a file, combined together to achieve more complex tasks than simple one-liner and are especially useful when it comes to automating sysadmin tasks such as backups.

This is a few things among many that you will learn in this room:

- Bash syntax
- Variables
- Using parameters
- Arrays
- conditionals

Throughout this room feel free to work along with me! You can test out the commands shown or integrate them into your own projects, after all you learn by practicing and applying what you have learnt into your own scenarios. Make sure to spawn the tryhackme attackbox or use your own terminal.

I found this website very useful when I was on my journey of learning bash, feel free to use it to help you through this room and for further learning after you finish! https://devhints.io/bash 


# First simple bash scripts 

First of all let’s lay out our structure.

A bash script always starts with the following line of code at the top of the script.

`#!/bin/bash`


This is so your shell (whatever type of it) knows that it needs to run your file using bash in the terminal.

Lets get into some basic examples.

You can also perform normal Linux commands inside your bash script and it will be executed if formatted right. For example we can run the command ` “ls”`, `"id"`, `"whoami"` inside our bash script and we will see the output when we run the file. So lets make it do this!

```bash
#!/bin/bash

echo "Hello world"

whoami

id

ls

```
This will return the string <b>“Hello World”</b>, whoami, id and ls command. The command <b>“echo”</b> is used to output text to the screen, the same way as “print” in python. I suggest you test this out in your terminal to get to grips with bash!

Now to run our bash script we must first give it executable permissions

`Chmod +x yourfile.sh`

And then we run it using `./yourfile.sh`

We can see it has outputted the results of the commands "echo", “whoami”, “id” and "ls".

#  Variables 
Now we are moving onto variables, in bash these are quite simple and we create them like so:

<img src="assets/variables1.png" alt="Tools" width="300">

Where we give the value of `Jammy` and assign it to the variable `name`.

Please note that for variables to work you cannot leave a space between the variable name, the ”=” and the value. They cannot have spaces in.

So how would we now use our variable? Well its also very simple.


We have to add a `$` onto front of our variable name in order to use it.

<img src="assets/variables2.png" alt="Tools" width="300">

If we test this out in our own terminal we get something like this:

`name="Jammy"`

`echo $name`

`Jammy`

This would output “Jammy” to the screen.

Variables make it much easier to store data and rather than typing out the same thing in multiple places we could simply insert our variable with $var and then declare that to a certain value making it easier to fall back on if you do something wrong and need to change it. So how can we debug our code?


Debugging is a very important part of programming so we should get used to problem solving and fixing errors as early as possible. And bash has a few built in features that make our life simple.

When running at the command line you can do:

`bash -x ./file.sh`

You can make a simple bash script(now you know some basic syntax) and make something completely wrong. Then step through your program with debug mode and see what it looks like when it throws errors!


This tells you which lines are working and which lines are not. If you want to debug at a certain point you can insert `set -x` into your script and `set +x` to end the section like the following:

<img src="assets/variables3.png" alt="Tools" width="300">

So lets look at an example. This is our script from earlier being ran with `bash -x ./example.sh`

<img src="assets/variables4.png" alt="Tools" width="500">

You can see its outputting a + for the command and then the output of what that command executed. If there was an error it would output a - on that line this makes it easy to spot where you have gone wrong so you can fix them.


We can also use multiple variables in something like an echo statement. You aren't just limited to using 1!

<img src="assets/variables5.png" alt="Tools" width="500">

<img src="assets/variables6.png" alt="Tools" width="500">