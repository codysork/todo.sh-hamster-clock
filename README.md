# todo.sh-hamster-clock
A [todo.txt-cli](https://github.com/todotxt/todo.txt-cli) extension that lets you track time for tasks in Hamster, the GNOME time tracker.

## Requirements

- [todo.txt-cli](https://github.com/todotxt/todo.txt-cli)
- [hamster-time-tracker](https://github.com/projecthamster/hamster)

## Setup

1. Put the clock script in your ` .todo.actions.d/ ` directory.
2. Edit the variables ` TODO_FILE ` and ` TODO_SH ` in the clock script and point 
   them to the proper paths in your system.

## Usage

Let's see what tasks are in our todo list first.
```
$ ./todo.sh ls
2 (A) Fight crime +Fighting
1 (B) Get milk +Errands
3 (B) Go to the post office +Errands
```

Clock in a task
```
$ ./todo.sh clock in 2
Clocking in Fight Crime...
```

To see our current clock
```
$ ./todo.sh clock cur
2020-04-23 12:56 Fight Crime@Fighting 00:01
```

Clock out a task
```
$ ./todo.sh clock out
Clocking out Fight Crime...
```

To see a report of today's clock totals
```
$ ./todo.sh clock report
Start | End      | Duration | Activity     | Category
--------------------------------------------------------
12:56 | 12:57    | 1min     | Update clock | Fighting
--------------------------------------------------------
Fighting: 1min
Total:  1min
```
