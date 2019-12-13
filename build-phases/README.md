# Build phases

## Configuration vs execution time

The `build.gradle` script in this exercise contains a property and two tasks:

- `setTheValue` changes the value of `theValue`
- `printTheValue` prints the value of `theValue`

Predict the outcome of the following commands:

- `./gradlew printTheValue`

```
Value initialized as: 100
The value currently is: 100
```

- `./gradlew setTheValue printTheValue`

```
Value initialized as: 100
theValue was doubled
The value currently is: 100
```

Run the commands and note the printed values.

- Q: Did the output match your expectations? If not, what tripped you up?
- A: I thought the value would double, but it did not. I assume because of the `def` statement.

Make a small change to the `build.gradle` such that:

- the `printTheValue`-task ends up printing `The value currently is: 200`,
- when run after the `printTheValue` task and
- while still using the `theValue` variable
