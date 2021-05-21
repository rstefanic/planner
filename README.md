# Planner

A script used to manage todo files. Inspired by [Carmack's plan files](https://garbagecollected.org/2017/10/24/the-carmack-plan/), this script is used to manage files laid out in the same way. The system's simple and lightweight, but I find myself doing the same maintenance over and over. This script helps with that maintenance.

## Usage

```
    new                       Create a new plan file for today
    outstanding               List all tasks left and their task number
    copy [task_number]        Copy a task to today
    complete [task_number]    Mark a task as complete
    reject [task_number]      Decide against doing a task
```

# Commands

## new

```bash
planner new
```

Create a new plan file for the day.

## outstanding

```bash
planner outstanding
```

List all outstanding tasks in the current directory. Outstanding tasks are uniquely listed and numbered. The number listed next to the task can then be used to reference that task.

## complete

```bash
planner complete [task_number]
```

Mark a task as complete by task number. The task number can be discovered through the `outstanding` command. Tasks completed today are marked with a "\*". Tasks from other days are marked with a "+".

## copy

```bash
planner copy [task_number]
```

Copies a task to the current plan file. If a plan file for today does not exist, it will be created.

## reject

```bash
planner reject [task_number]
```

Decide against doing a task in all files in the current directory.
