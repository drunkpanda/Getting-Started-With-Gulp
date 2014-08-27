> Reference from:  Travis, M. (December, 17th 2013). Getting Started With Gulp. Retrieved from [http://travismaynard.com/writing/getting-started-with-gulp](http://travismaynard.com/writing/getting-started-with-gulp)

# Getting Started With Gulp

> This article will make the assumption that you have never used a task runner or command-line interface before and will walk through every step required to get up and running with gulp.

## Step One - Install Node
First - we need our most important requirement, Node. To install Node - simply visit http://nodejs.org and then click that big green “Install” button. Once your download completes, run that application and you should be all ready to go. The Node installer also includes npm, which we will come back to a little later.

## Step Two - Get To Know Your Command Line
Now, you may not be very familiar with your command-line interface (Terminal for OSX, Command Prompt for Windows) but you should be! It may seem intimidating at first, but once you get the hang of it you will have the ability to run many different command line applications such as Sass, Yeoman and Git. All of which are very useful tools that your workflow could benefit from!

> If you are familiar with your command-line interface, then feel free to skip to step four.

As a quick example, open up your command line and we will throw a couple commands at it to ensure that Node is properly installed.

'node -v'

> node -v

## Questions and Solutions
What the difference task return and task not return 

### example of task without return 

> gulp.task("XXXX", function() {
>    gulp.src("....

### example of task with return

> gulp.task("XXXX", function() {
>    return gulp.src("....

### Answer
You return to indicate that the task is async. gulp.src() returns a stream, so it's async.
Without it the task system wouldn't know when it finished. read (Async task support)[https://github.com/gulpjs/gulp/blob/master/docs/API.md#async-task-support]