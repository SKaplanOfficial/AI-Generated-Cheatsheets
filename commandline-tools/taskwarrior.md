# Taskwarrior Cheatsheet

## Unique Features
* Command-line task manager
* Supports task prioritization and due dates
* Supports task annotations and tags
* Supports recurring tasks and dependencies
* Can be extended with plugins and hooks
* Available on most operating systems

## Basic Usage
* Add a task: `task add [description]`
* List tasks: `task list`
* Complete a task: `task [task_id] done`
* Delete a task: `task [task_id] delete`
* Modify a task: `task [task_id] modify [attribute]=[value]`

## Advanced Usage
* Filter tasks by status: `task [status]`
* Filter tasks by project: `task project:[project_name]`
* Filter tasks by tag: `task +[tag_name]`
* Filter tasks by due date: `task due.before:[date]`
* Filter tasks by priority: `task priority:[priority_level]`
* Recurring tasks: `task add [description] recur:[recurrence_interval]`
* Dependencies: `task [task_id] modify depends:[task_id]`
* Hooks: `task config hook.[hook_name].command [command]`

## Output Options
* Customize output format: `task [filter] rc.verbose:[output_format]`
* Set default output format: `task rc.defaultwidth=[width] rc.defaultheight=[height] rc.defaultcommand=[command]`

## Resources
* [Taskwarrior User Guide](https://taskwarrior.org/docs/)
* [Taskwarrior Wiki](https://taskwarrior.org/projects/taskwarrior/wiki)
* [Taskwarrior Hooks and Scripts](https://github.com/GothenburgBitFactory/taskserver/wiki/Hooks-and-Scripts)
