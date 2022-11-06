# General bash script notes
Bash scripts are helpful as shortcuts for many everyday things I do regularly. Usually, by the time I have run the command a couple of times, I think I should probably write a script for this. This is especially true when the command arguments are long and easy to mistype (especially bad for dyslexics like me). for this reason, I have compiled some notes of things I have learned along the way with working with bash scripts.

## Setting up a bash script
You need to create a new file for your bash script. I will have all my bash scripts end with an extension of ".bash".  I do this so that they are easy for me to spot and put filters in tools like editors. So this is how I start with creating a bash file:

```
touch myscript.bash
chmod 775 myscript.bash
```

This will create a new empty file and name it "myscript.bash". The second command sets the permission of the file to be executable (user/group writable and all readable/executable)

Next, I will add the following line at the beginning of a file:

```
#!/usr/bin/env bash
```

This tells the shell that this script is to be interpreted by the bash shell interpreter.

## Boiler template variables

I like to have some common variables show up in my scripts so I can use them to determine where files are, relative to this script.  For this I will add lines similar to the following:


