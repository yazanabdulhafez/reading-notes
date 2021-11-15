# Intents, Activities, and SharedPreferences

## Tasks and the back stack

A task is group of activities ,when a user start to use the application these activities pushed to the stack in the order they opend and when finsh one activity it poped from the stack and return to previous activity.

### Lifecycle of a task and its back stack

![lifeCycle](https://developer.android.com/images/fundamentals/diagram_backstack.png)

When the current activity starts another, the new activity is pushed on the top of the stack and takes focus. The previous activity remains in the stack, but is stopped. When an activity stops, the system retains the current state of its user interface. When the user performs the back action, the current activity is popped from the top of the stack (the activity is destroyed) and the previous activity resumes.

### Back press behavior for root launcher activities

root luncher activities declare intent filters with

1. ACTION_MAIN
2. CATEGORY_LAUNCHER

and these activities are unique since it is act as entry points

### Background and foreground tasks

A task is a cohesive unit it can be moved to the background when a user begins a new task or goes to the Home screen.

### Multiple activity instances

one activity could be instantiated multiple times with diffrent tasks since the activities not arranged in the stack.

### Multi-window environments

In android 7.0 and higher the system can mange the tasks for more than one windo from the same application.

## Manage tasks

All the tasks put in the stack and processed on the principle first in last out,but some time we need to break this system and create new activity in order to do this we use  attributes in the `<activity>` manifest element and with flags in the intent that we pass to **startActivity()**.

### Defining launch modes

Launch modes allow us to define how a new instance of an activity is associated with the current task. we can define different launch modes in two ways:

1. Using the manifest file
2. Using Intent flags

### Handle affinities

An affinity indicates which task an activity prefers to belong to.all the activities from the same app have an affinity for each other.and we can modify it by using the taskAffinity attribute of the `<activity>` element.

### Clear the back stack

if the user leav the task for long time the system clear all the acticities except the root activity.

### Start a task

we can set an activity as an entry poind by giving it an intent filter with **"android.intent.action.MAIN"** as the specified action and **"android.intent.category.LAUNCHER"** as the specified category.

## Save key-value data

To save a small collection of key-values we use the SharedPreferences APIs

### Get a handle to shared preferences

To creat or accses shared preference file by calling these methods

1. getSharedPreferences() — Use this if you need multiple shared preference files identified by name.
2. getPreferences() — Use this from an Activity if you need to use only one shared preference file for the activity.

### Write to shared preferences

To write to a shared preferences file,we create a SharedPreferences.Editor by calling edit() on the SharedPreferences.

### Read from shared preferences

To get the values back from a shared preferences file, call methods such as

1. getInt()
2. getString()

## Resources used in this reading

1. [Tasks and the back stack](https://developer.android.com/guide/components/activities/tasks-and-back-stack#life-cycle)
2. [Save key-value data](https://developer.android.com/training/data-storage/shared-preferences)
