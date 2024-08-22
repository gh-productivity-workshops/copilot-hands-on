## Lab 7 - Teaching Copilot about updates

**Purpose: In this lab, we’ll see an example of what to do when Copilot does not have the most up-to-date information**

1. Create a new file called *explore.go* via the same approach as you used to create other files.

2. This file should now be open in an editor tab. Let's say we want to seed a random number generator with Go. Let's ask Copilot to write a function to do that. Prompt it through the **CMD+I** interface using the statement below. Then you can accept the suggested code.

```
write a function to seed a random number generator
```
![Asking Copilot to write function to seed a random number generator](../images/cdd117.png?raw=true "Asking Copilot to write function to seed a random number generator") 

3. Copilot has probably generated code using the rand.Seed function. The challenge is that as of Go 1.20, the Seed function is deprecated.  Ref: https://cs.opensource.google/go/go/+/refs/tags/go1.21.0:src/math/rand/rand.go;l=394

4. Let's see if Copilot understands that this is deprecrated. We'll ask it via a query. Switch to the separate chat inferface and enter the query below.

```
Is the Seed function deprecated in Go?
```
![Is Seed function deprecated?](../images/cdd118.png?raw=true "Is Seed function deprecated?") 

5. Copilot probably responded with no and some info about the function. So one way we can help Copilot understand language updates is by providing the context in our file. So let's start again. Delete the current content in the explore.go file.

6. Now, let's provide Copilot some more direct context by copying in updated code examples. After deleting the code block from step 3, copy and paste in the following example of the replacement for the Seed deprecation into your explore.go file.  This is taken from pkg.go.dev/math/rand.

```
	// Create and seed the generator.
	// Typically a non-fixed seed should be used, such as time.Now().UnixNano().
	// Using a fixed seed will produce the same output on every run.
	// r := rand.New(rand.NewSource(99))
```

7. Now, let's try the creation of the function again. Underneath the comments and code you just pasted, invoke the dialog via **CMD+I** and enter the statement below again.
```
write a function to seed a random number generator
```

8. This time, the code should be using the same format and NewSource function as you put in the file in step 6. You can just Accept the change. (If you don't see a complete function, but just a single line, try changing the prompt to be "write a complete function to seed a random number generator".

![Updated random number gen code after including updated usage](../images/cdd119.png?raw=true "Updated random number gen code after including updated usage")


## Next ➡️
[Continue to the next Lab](lab8.md)