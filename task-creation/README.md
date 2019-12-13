# Task creation

## Hello, world

Create a task called `hello` that prints `Hello, world!` when executed.

- Run `./gradlew`
- Q: Did Gradle print `Hello, world!`? If so, what happened?
- A: No, it printed the output from the ':help' task. Set up 'defaultTasks' to change this.

- Run `./gradlew hello`
- Q: Was the output as expected?
- A: Yes

- How can you avoid `Hello, world!` be printed out in the configuration phase?
- A: Wrap the functionality in a 'doLast' block, or add the '-q' option.

## Task properties

- Run `./gradlew tasks`
- Q: Is your 'hello' task listed?
- A: No!

- Q: Can you get `./gradlew tasks` to list it anyway?
- A: Yes, with `./gradlew tasks --all`

Configure the group and description of your task.

- Run `./gradlew tasks`
- Q: Is your tasks visible and defined according to its purpose?
- A: Yes
