# todo.sh-hamster-clock
A [todo.txt-cli](https://github.com/todotxt/todo.txt-cli) extension that lets you track time for tasks in through Hamster, the GNOME time tracker.

## Requirements

- [todo.txt-cli](https://github.com/todotxt/todo.txt-cli)
- [hamster-time-tracker](https://github.com/projecthamster/hamster)

## Setup

1. Put the clock script in your ` .todo.actions.d/ ` directory in your home folder.
2. Edit the variables ` TODO_FILE ` and ` TODO_SH ` in the clock script and point 
   them to the proper paths in your system.

## Usage:
```
todo.sh clock in TASK_NUM
todo.sh clock out
```
