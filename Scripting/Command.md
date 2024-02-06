# Basic of Shell Script
### Create file Shell script

```touch hello_world.sh
```

### Find the path to your bash shell.

```which bash
```
In my case, the path is ` /usr/bin/bash ` and I will include this in the shebang.

### Write the command.

```echo "Hello World"
```
Edit the file hello_world.sh using a text editor of your choice and add the above lines in it.

### Provide execution rights to your user.

```chmod u+x hello_world.sh
```
`chmod` modifies the existing rights of a file for a particular user. We are adding `+x` to user u.
