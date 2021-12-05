# LetsLearnPython

# Introduction

Alrighty, this is a repo for the three of us to go over some python basics and see if we can learn a bit more together.

In the same vein that you've not learnt python before I haven't taught it, but I'm hoping to impart at least some knowledge to you both. However if you have any issues or questions do let me know.

Firstly, this file is called a "README" and is done in a language called "Markdown" it's a standard and fairly basic form of code that holds information on the repo and usually allows uses to get an idea of what the programs on the repo are meant to do.

You can see an example of a relatively well formed on on the main branch of my [PythonProjects repo](https://github.com/rd144/PythonProjects)

The formatting of Markdown is pretty simple, here is a pretty useful cheat sheet for it [here](https://www.markdownguide.org/cheat-sheet/).

Secondly, I recommend finding an Integrated Development Environment (or IDE) in which you can develop your code.

I personally use PyCharm ([Download Link](https://www.jetbrains.com/pycharm/download/download-thanks.html?platform=windows&code=PCC)), and that works prett well for me.

# Structure

So the general structure I'm thinking of going with is very similair to how I was taught, a very much learn by doing approach.

I will assign problems for you to solve, and once you have created a Merge Request I'll review it, ask you questions on it, and if it looks good, we'll merge it into your respective folder.

The skills I'll look to cover include:

- Learn how to use GIT (Add, Remove, Review, Merge etc.)
- Learn how to use the .gitignore
- Printing to screen in Python
- Reading/Writing files
- Relative Filepaths
- Logical Statements (IF X AND Y DO Z etc.)
- Iteration Loops (WHILE and FOR and when to use them)
- Creating Methods
- Object Oriented Programming (OOP) and Creating Classes
- Importing Methods/Classes from other locations
- PIP Installing Libraries

After you are able to do all this pretty well we an try and do a project together on a common interest and see what we can build.

# Lessons

## Lesson 0 - Setup
Ok, the first thing I want you to do is to get setup in an evnironment in which you can code.

There are a number of youtube videos that will show you how to get setup in PyCharm ([Link](https://www.youtube.com/results?search_query=setting+up+pycharm+for+python)).

After that you will likely also want to install GIT ([Link](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)) so that we can properly collaborate and share code.

Like before, there are some helpful videos on youtube that, [this video](https://www.youtube.com/watch?v=USjZcfj8yxE) in particular is pretty good.

However reach out to me on WhatsApp if you get stuck and I can help you along.

Getting set up is usually painful unfortunately, but it is done very infrequently so once we do it once we'll be set for the rest of this.

Once your setup you let me know, and feel free to move onto Lesson 1

### State at End of Lesson

- [ ] - GIT Installed
- [ ] - Coding Environment Installed

## Lesson 0 - GIT and Hello World

Okay, now you're setup the first thing we're going to do is take a clone of the Repo ([LetsLearnPython](https://github.com/rd144/LetsLearnPython)) so we can begin to create some code there.

There are a couple ways to do this.

1. You can open up a command line and run a clone statement `git clone https://github.com/rd144/LetsLearnPython.git`
2. Pycharm can handle GIT statements. If you right click on the Project window on the right, go down to the GIT menu, then repository, then clone, and follow the instructions provided in the window to clone the repo to the provided directory
![GIT Clone Image](Materials/GITClone.png)

Once you have the clone, I want you to take a branch of your own for your work.

Like taking a clone, you can do this from the command line `git checkout -b MyNewBranchName` or in PyCharm you can select the GIT menu on the bottom right of Pycharm, select the repo, select main, select "New Branch From Selected" Then just name it what you want, and it'll create a new branch for you to work on that wont affect the code on main.

![GIT Branch Image](Materials/GITBranch.png)

Once you have a branch, create ANY file into a folder named after yourself. I dont mind what it is. Copy and paste an image from the internet. Create a text file saying Hi. Do whatever. Just put it in your folder, use `git add` to add the file to your branch, use `git commit -m "Message about what you've done"` to make a commit, and then finally use `git push` to push the change to Origin. 

This is basically just syncing what's on your PC (referred to as local) with what's on the repo that we can all see (called remote)

Once the file is on remote (you'll be able to see the branch listed [here](https://github.com/rd144/LetsLearnPython/branches), let me know and we can move on to the next step (Creating a Merge Request and Starting with Hello World)

If you want to work with GIT through the command line, or understand what PyCharm is doing in the background, [this cheatsheet](https://wac-cdn.atlassian.com/dam/jcr:e7e22f25-bba2-4ef1-a197-53f46b6df4a5/SWTM-2088_Atlassian-Git-Cheatsheet.pdf?cdnVersion=99) is a pretty helpful reference tool

### State at End of Lesson

- [ ] - Repo Cloned
- [ ] - Personal Branch Created
- [ ] - File Added through GIT
- [ ] - Commit made
- [ ] - File Pushed to Origin


## Lesson 1 - Hello World

This is an entry level experience. Getting Python to print something to screen.

First we need to create a python file. Just create a new file in your directory and name it "HelloWorld.py"

Once that file is created, open it up and we can start writing code!

The first thing to know is the print command. This prints whatever text is passed to it to screen.

For example:
```
print('Ross is the best person ever')
```

When this code is run it will print the output 'Ross is the best person ever' to the command line (the screen you see the results of your code. Also called the terminal)

Firstly create a print command that prints 'Hello World', then play about with it for a bit.

## Lesson 2 - Variables and Datatypes

In code we want to store some thing so that we can call them easier later. We call these variables.

For example using the print command:

```
print_statement = 'Hey this python stuff isn't too hard'
print(print_statement)
```

in this example we have set the print_statement to a string (any combination of alpha characters), and thus when we print it we will get the output 'Hey this python stuff isn't too hard'.

the string is one of many different types of datatypes. Others common datatypes include:

1. Boolean : True and False
2. Int : Integer (...,-2,-1,0,1,2,3,4,5....)
3. float : decimal (1.231321, -1,96123 , etc.)
4. None : This is the absence of a value

You can find a list of other datatypes  [here](https://www.w3schools.com/python/python_datatypes.asp) 

## Lesson 3 - Lists and Dictionaries

Sometimes we want to store a list of multiple things, for example if we had an auto-caller we might want to store a list of phone numbers.

To do this we can use a list object to contain these.

The notation for this takes the following.

```
phone_list = ['07782-943691','07831-054949','01546-300272']
```

**Task:** Create a list of statements that you want to print to screen.

Some times we want to be able to call specific items when we know something else about them. Keeping the phone number example, we might want to have these against names.

To do this we create a dictionary object. This looks like the following:

```
phone_dict = {
    'Ross' : '07782-943691',
    'David' : '07831-054949'
}
```

We call the string on the left hand side the 'key' and the value on the right is called the 'value'. The value doesn't have to be a string it can be any othe datatypes and often other dictionaries.

If we want to return the value we pass the key to the object like the following:

```
print(phone_dict['Ross'])
```

This will print out only the number that is stored against 'Ross'. if instead we called:

```
print(phone_dict['James'])
```

it will fail because the key doesn't exist in the object. Often you want this to fail out so you know the key is incorrect, but if you don't you can instead call the value in the following way.

```
print(phone_dict.get('James'))
print(phone_dict.get('James','No Number'))
```

the first statement will print an empty line, while the second will notice that the key doesn't exist and rather than returning None will return 'No Number'

**Task:** Create a dictionary object with the numbers 1 to 10 as key's and any statement you like as the values

## Lesson 4 - Operators

### FOR Loop

There are many instances in coding where we want to loop through the objects contained in a list.

To do this we use a for loop, written as:

```
for phone_number in phone_list:
    print(phone_number)
```

This will iterate through all the phone numbers contained in the phone_list and print them to the screen

**Task:** Iterate through the dictionary you created and see what happens. Try to iterate through the dictionary and return the phone numbers with their corresponding name.

**Task:** Iterate through the dictionary and return the phone numbers with their corresponding name.

To help with the above task, you can use either the format function or the f string prefix like the following.

```
name = 'Ross'
phone_number = '07782-943691'

print(
    '{var1} : {var2}'.format(var1=name,var2 = phone_number)
)

print(
    f'{name} : {phone_number}'
)
```

Both of these return the same lines to the terminal.

### WHILE Loop

A while loop will continue the iteration until a specific criteria is met. While these loops are incredibly useful, they can be problematic if not run carefully. For example if you run while 1=1, this will NEVER end.

**Task:** Create a Variable and set it to 1.

**Task:** Using a while loop, iterate through your phone number list adding 1 to the variable you created each time, until a certain number of phone numbers have been printed to screen.


### IF Statement

These statements check for whether criteria is met and then runs the code underneath it.

There are a maximum of 3 parts to any if statement.

1. IF :  This is the initial statement that is the first check done and designates the start of the if statement.
2. ELIF : This is a secondary check for when the first fails. If there are multiple checks they happen sequentially.
3. ELSE : This is a final statement that runs if none of the criteria above it have been met.

```
x = 1
while x <= 10:
    if x == 3: # Equal to 3
        print(f'Hey I found a {x}')
    elif x == 3: # Equal to 4
        continue
    elif x == 9: # Equal to 9
        print(f'Look, its a {x}')
    elif x > 5 : # Greater than 5. Note that when the number is 9 the above line is the only one that acts
        print(f'Would you look at that its a {x}')
    else:
        print(f'What a shame {x} is not 3,6, or 9')
    x = x + 1
```

**Task:** Create a statement to look through the Phone Number dict you created and print off the numbers that correlate to only even numbered keys, except the number 9

**Hint** When you divide an even number by 2 it should equal the int of the same number (x/2 = int(x/2))

## Lesson 5 - Methods

Often in code you'll find parts of code that are repeated over and over again. Rather than copy and paste these throughout the code we create a piece called a "Method" that we can call to run that iece of code.

Methods are defined by using the "def" statement, and are provided with parameters that are to be run.

In the below I'll put together a simple method that adds a number to another number and prints whether the result is even.

```
def example_method(input_number, additive_number):

    result = input_number + additive_number
    divided_result = result/2

    if divided_result == int(divided_result):
        print(f"Hey {result} is an even number")
    else:
        print(f"Unfortunately {result} is not an even number")

    return result

result_1 = example_method(4,2)
result_2 = example_method(3,8)

print(result_1,result_2)
```

**Task:** Make a method that can add, subtract, divide, and multiply a result and return it.

##Resources

1. https://www.w3resource.com/python-exercises/ - A good website with exercises you can practice