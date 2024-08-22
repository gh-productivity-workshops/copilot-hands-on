## Lab 5 - Using Copilot to generate tests

**Purpose: In this lab, we'll see some examples of having Copilot generate tests**

1. Start out in the *prime.py* file we've been using. Position the cursor below the code.

2. Enter a comment to create unit tests
```
# create a function to do 5 unit tests of the code above
```

3. *If you don't get a suggestion*, enter code below to start nudging. Otherwise you can just accept the suggestion.

```
def test_is_prime():
```
![generating tests via comment](../images/cdd46a.png?raw=true "generating tests via comment") 

4. What if we didn't know how to test the code at all? Let's ask Copilot. Highlight the *is_prime()* function.

![selecting code](../images/cdd111.png?raw=true "selecting code") 

5. Now, switch to the chat interface and ask Copilot using the following prompt:

```
#selection: How do I test this code?
```
![prompting on how to test](../images/cdd112.png?raw=true "prompting on how to test") 

6. After entering this, you should see an explanation of how to test the code along with suggested testing code. If you expand the reference in the chat output, you can see that it only used the selected lines.

![testing explanation](../images/cdd113.png?raw=true "testing explanation") 

7. Let's see what the shortcut command would do. In the chat dialog enter "/tests" and then Enter. Copilot will want to add the *@workspace* agent onto the command. Just remove the *@workspace* from the beginning of the command. **Do not hit enter yet**.
```
/tests
```
8. Type a hash/sharp sign after /tests. At this point, Copilot should present a selection dialog. Choose #file from the menu.
```
/tests #
```
   
![shortcut test command](../images/cdd140.png?raw=true "shortcut test command")

9. A dialog will pop up near the top of the codespace with a selection of files. Select the *prime.py* file to complete the command. 

![file choice dialog](../images/cdd141.png?raw=true "file choice dialog")

10. Once the command looks like */tests #file:prime.py*, go ahead and hit enter to see the suggested test results.

![file choice dialog](../images/cdd142.png?raw=true "file choice dialog")

11. We can put this into a new file by hovering over the output in the Chat window, then selecting the "..." from the pop-up menu and selecting "Insert into new file". Go ahead and select that option and then you'll have a new file in your editor with the code that you can save as needed.

![Insert tests into new file](../images/cdd115a.png?raw=true "Insert tests into new file") 


## Next ➡️
[Continue to the next Lab](lab6.md)