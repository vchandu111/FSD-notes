**Why Use the Command Line?**

Both the GUI(Graphical User Interface) and CLI(Command Line Interface) are ways you can interact with your computer.
But when it comes to the command line, once you learn the commands, it is faster and more powerful to navigate and use your computer. This is why many programmers prefer the command line.

***Graphical user interfaces make easy tasks easy, while command line interfaces make difficult tasks possible***

### What is the shell?

Simply put, the shell is a program that takes commands from the keyboard and gives them to the operating system to perform.

## List of Commands

| Navigation commands |                         Description                          |
| :-----------------: | :----------------------------------------------------------: |
|       `date`        |                Displays current date and time                |
|        `df`         |            Displays the amount of free disk space            |
|       `free`        |              Displays the amount of free memory              |
|        `pwd`        |                   Print working directory                    |
|        `cd`         |     Change directory (to move between files and folders)     |
|       `cd ..`       |    Working directory parent (to go back to parent folder)    |
|   `cd ~` or `cd`    |                        Home directory                        |
|        `ls`         |                List all files in that folder                 |
|       `ls -l`       |                Show detailed info in columns                 |
|       `ls -a`       |   List all files in that folder including **hidden files**   |
|       `ls-R`        |               Recursively list subdirectories                |
|       `ls-aR`       |   Recursively list subdirectories along with hidden files    |
|       `ls -t`       |           Sort by last modified date newest first            |
|       `ls -S`       |                         Sort by size                         |
|       `ls -F`       | Indicator at the end of each file ``/`` if it is a directory |
|       `ls a*`       | It shows the list of all files that start with character 'a' |

|      Manipulation commands       |                         Description                          |
| :------------------------------: | :----------------------------------------------------------: |
|     `mkdir <directory name>`     |        `mkdir test` (creates a folder with name test)        |
|   `mkdir <dir1><dir2><dir3> `    |                 Creates multiple directories                 |
| `mkdir -p <dir1>/<dir2>/<dir3> ` |                Create intermediate directory                 |
|       `cp <item1><item2>`        |      Copies the single file or directory item1 to item2      |
|      `cp file1 file2 dir1`       |             Copy file1 and file2 into directory              |
|         `cp dir1/* dir2`         | Using a wildcard, copy all the files in dir1 into dir2. The directory dir2 must already exist. |
|        `cp -r dir1 dir2`         |    Copy the contents of directory dir1 to directory dir2.    |
|       `mv <item1> <item2>`       | Performs both file moving and file renaming `mv file1 file2` - Move file1 to file2. If file2 exists, it is overwritten with the contents of file1. If file2 does not exist, it is created. In either case, file1 ceases to exist. `mv file1 file2 dir1` - Move file1 and file2 into directory dir1. The directory dir1 must already exist. |
|          `mv dir1 dir2`          | If directory dir2 does not exist, create directory dir2 and move the contents of directory dir1 into dir2 and delete directory dir1.If directory dir2 does exist, move directory dir1 (and its contents) into directory dir2. |
|           `rm <item>`            |        used to remove (delete) files and directories         |
|           `rm -r dir1`           |                Delete dir1 and its contents.                 |
|        `rm -r file1 dir1`        |            Delete file1 and dir1 and its contents            |

#### Extra Commands:

`wget <location>` - command-line program for file downloading
`unzip <file>` - command to unzip a file