# `run` string for the .replit file

Copy and paste the following strings into the `.replit` file as the `run` argument to run the individual projects.

> Note the use of the `\n` character to separate calls to `javac` and to `java`

## Simple project structure

>No internal structure

### projet

#### with compile

`"javac projet/App.java \n java -cp projet App"`

#### using Java 9+ single-file-project java call (no .class file generated)

`"java projet/App.java"`

### projet2

#### with compile

`"javac projet2/App.java \n java -cp projet2 App"`

#### using Java 9+ single-file-project java call (no .class file generated)

`"java projet2/App.java"`

## Standard project structure

>* Separate source and binary (`src` and `bin` directories)
>* Using packages (subdirectories)

### plusieursClasses

`"javac -d plusieursClasses/bin plusieursClasses/src/edu/djc/classes/Helper.java plusieursClasses/src/edu/djc/classes/App.java \n java -cp plusieursClasses/bin edu.djc.classes.App"`
