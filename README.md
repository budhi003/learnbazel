# HelloWorld Bazel Project

A minimal Java project built with Bazel.

## Build
```bash
bazel build //:hello_world
```

## Run
```bash
bazel run //:hello_world
```

## Clean
```bash
bazel clean
```

## Simple Java Example

This section provides a simple example of a Java program built with Bazel, including build and run instructions.

### Step 1: Create the Java file

Create a file named `HelloBazel.java` with the following content:

```java
// HelloBazel.java
public class HelloBazel {
    public static void main(String[] args) {
        System.out.println("Hello, Bazel!");
    }
}
```

### Step 2: Create the BUILD file

Create a `BUILD` file in the same directory with the following content:

```python
# BUILD
java_binary(
    name = "hello_world",
    srcs = ["HelloBazel.java"],
    deps = [],
)
```

### Step 3: Build and Run

1. Build the program:
```bash
bazel build //:hello_world
```

2. Run the program:
```bash
bazel run //:hello_world
```

### Use Case

This simple example demonstrates the basics of building and running Java code with Bazel. You can extend this example by:

1. Adding more Java classes and organizing them into packages
2. Including external dependencies using the `java_import` rule
3. Adding unit tests using the `java_test` rule
4. Configuring code coverage
5. Setting up continuous integration

This example provides a foundation for learning Bazel's Java toolchain and how to manage Java projects with Bazel.
