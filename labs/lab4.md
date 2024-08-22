## Lab 4 - Using Copilot after the coding

**Purpose: In this lab, we’ll see a few other ways to leverage Copilot after the initial coding is done**

1. Now that we have some code to work with, let's see what else Copilot can do for us. Let's have it explain the current code in our *prime.py* file.  Select the code. Then, use the **Cmd+I** keys to bring up the Copilot interactive chat dialog.

![Interactively telling Copilot to explain code](../images/cdd40b.png?raw=true "Interactively telling Copilot to explain code")


2. Tell Copilot to explain the code by typing the command below in the dialog. Hit Enter. Then, you should see the output in the dialog. Click on the *View in Chat* button to see the output in the separate chat window.

```
/explain
```
![Output of interactively telling Copilot to explain code in dialog](../images/cdd144.png?raw=true "Output of interactively telling Copilot to explain code in dialog")
![Output of interactively telling Copilot to explain code](../images/cdd41b.png?raw=true "Output of interactively telling Copilot to explain code")

3. Now, let's do the same request but through a comment. In the *prime.py* file, below the code, enter the following comment and hit Enter.
```
# explain the code above line-by-line
```
4. After this, Copilot should start showing the explanation in comments. Just hit tab to accept each line and then Enter to move to the next one.

![Output of telling Copilot to explain code via comment](../images/cdd42b.png?raw=true "Output of telling Copilot to explain code via comment")

5. We can also query Copilot inline via asking a question in a comment. Delete the commented explanation and try out the question below. To be clear you can prefix it with :q but that is not required with the chat feature installed.

```
# q: what does the function above do?
```

![Prompting for what code does with q:](../images/cdd43b.png?raw=true "Prompting for what code does with q:")

6. Finally, let's see how to use the doc feature to automatically document our code. Highlight the actual code.

7. Now, enter **Cmd+I** and enter the **/doc** command. After a few moments, Copilot should generate some documentation for the code. You can go ahead and *Accept* the changes.

![Generated doc for the code](../images/cdd44d.png?raw=true "Generated doc for the code")  

8. While this is useful documentation for the start of the function, we'd like to have more extensive comments in the function body. So,let's get Copilot's help with that. Bring up the chat dialog again with **Cmd+I** and enter the text "verbosely comment this code". After Copilot completes its suggestions, if you're happy with them, you can just click *Accept*. 

![Regenerating doc](../images/cdd110.png?raw=true "Regenerating doc")  

9. Once you find a doc example you like, go ahead and click **Accept**.


## Next ➡️
[Continue to the next Lab](lab5.md)