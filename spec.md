background

an active account for todoist is available

### feature : register project
#### scenario

when I want to create a project with a name, purpose, start and end date
then the project gets created

given that there exists a project
when I want to delete the project
then the project gets deleted
 
given that there exist one or more projects
when I want to see them all
then I am able to see the list of projects 

### feature : manage task and corresponding subtask
#### scenario

given that there exists a project
when I want to create a task with id (projectId + taskId), title, purpose, due, priority, dependsOn, effort, priority and parent id (the containing task)
then the task gets created

(default)
given that there exists one or more task 
when I want to view the list ordered by due date
then the tasks are shown ordered by due date
(variation1)
when I want to view the list ordered by priority 
then the tasks are shown ordered by priority
(variation2)
when I want to view the list resolved by dependsOn attribute
then the tasks are shown in form or a graph

#### scenario

given a specific time of the day
and priority of the ongoing projects
and priority of the tasks of the projects
and having the information of dependsOn attribute
when I issue 'next' command
then the option for next set of tasks are displayed with respective project, id (of the task) and content (of the task)

#### scenario

given a task has associated effort
and the task has been initialized
when I pause the task
then the timer for the task is paused for configurable period

#### scenario

given a task has associated effort
and the task has been paused
when I unpause the task
then the timer for the task is unpaused

### feature : work on the task in focused mode using pomodoro technique

#### scenario

given that there exists a task
when I want to focus on it (see GeekBot)
then I am able to initialize the task

### feature : receive automatic reminder based on criteria
#### scenario

given a specific task has a due date
when the time approaches 
then I start receiving whatsapp notification 

### feature : generate productivity report
#### scenario

when I want to see my productivity report
then I am able to see my productivity report

