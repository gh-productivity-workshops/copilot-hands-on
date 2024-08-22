## Lab 3 - Using Copilot to simplify and explain code

1. Create a new file named prime.py. Create it via the same process as we used in Lab 2 by entering the line below in the terminal.

```
code prime.py
```

2. Start typing a function definition as below
```
def is_prime(n):
```
3. Leave the cursor at the end of the line.

![starting point](../images/cdd104.png?raw=true "starting point") 

4. Hit **Ctrl+Enter** to see options

5. Pick one of the options that is longer and/or more complex (if there is one) and **Accept suggestion #**. If there's not one that's longer/more complex, just pick an alternative one and **Accept suggestion #**.

![alternative suggestions](../images/cdd34b.png?raw=true "alternative suggestions") 

6. Highlight the code and select the Chat extension icon to open the chat window.  Tell Copilot to simplify the code by typing in the chat window.
```
simplify
```

![simplifying via chat box](../images/cdd35.png?raw=true "simplifying via chat box") 

7. Hover over the simplified text and tell Copilot to insert the suggestion at the cursor to replace the text that's currently there. 

![replace from chat suggestion](../images/cdd143.png?raw=true "replace from chat suggestion")    

8. Now, let's introduce an error into the code to see how Copilot can fix it. Pick an instance of a variable name and change it to one that doesn't exist. For example, change an instance of "n" to "x". 

![introduce error](../images/cdd37b.png?raw=true "introduce error")   

9. Notice the light bulb icon that has popped up. Click on that, scroll to the bottom (if needed), and you'll have additional options to fix or explain with Copilot.

![Copilot options inline](../images/cdd38b.png?raw=true "Copilot options inline")   

10. Go ahead and click on the "Fix using Copilot" option.

11. After a few moments, it should propose a fix that you can just accept (via the Accept button). You can also click on the *Show Changes* icon to see before/after for the proposed changes. (If it doesn't propose a fix in the dialog, you can skip to step 12 and use the /fix command in chat instead.)

![Fixing with Copilot](../images/cdd107a.png?raw=true "Fixing with Copilot")       

12. (Optional) If you'd like, you can go back and make the error again, highlight the code, and then use the /fix command in the chat window to get the same results.


## Next ➡️
[Continue to the next Lab](labs/ab4.md)