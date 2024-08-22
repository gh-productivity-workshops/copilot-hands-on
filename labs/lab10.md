## Lab 10 - Agents and Terminal

**Purpose: In this lab, we'll get some practice using GitHub Copilot agents and the Copilot CLI.**

1. Now let's see how Copilot can help with tasks using agents. First, we'll have Copilot help us commit a change.  Let's use the *explore.go* file we created in a previous lab. If you haven't already, make sure that file is saved. You can do this by:
- Select the *explore.go* file
- Click on the *three-line menu* in the top left.
- From the menu that comes up, select *File* and then select *Save* (or use the shortcut).
2. Now, let's invoke the **@terminal** agent to ask a common question about how to stage your code changes. Go to the *chat* interface and enter the prompt below. Afterwards, the command to do the staging should show up in the chat output.

```
@terminal how do I stage explore.go?
```
![query output](../images/cdd134.png?raw=true "query output") 

3. Hover over the window with the commands in it, and then click on the icon that pops up for the terminal. Click on that to insert the command into the terminal. Then hit return.

![insert into terminal](../images/cdd135.png?raw=true "insert into terminal")

4. Now let's commit our change through the interface and have Copilot suggest a commit message for us. Click on the source control icon in the sidebar (#1 in the figure below). Your *explore.go* file should be selected. In the box titled "Message" above the *Commit bar*, click on the *sparkle icon* at the far right side (#2 in the figure below).

![insert into terminal](../images/cdd136.png?raw=true "insert into terminal")
5. After this, Copilot should (hopefully) generate an appropriate commit message in that box. You can then copy the message and paste it into a *git commit* command in the terminal. **If you started your codespace from a fork, you can hit return to complete the commit if you want. This is optional. If you started your codespace via the one-click button, you will not have permissions to commit.**
```
git commit -m "<contents of generated commit message from Copilot goes here>"
```
![commit with generated message](../images/cdd137.png?raw=true "commit with generated message")

6. Now, let's switch gears and use the **@workspace** agent to help identify where we use certain things in our code. With the *explore.go* file still active in your editor, in the separate *chat* interface , enter the following prompt:

```
Which files are using SQL?
```

7. After executing this, you'll likely have some suggested information on how to search for files that use SQL in your project with search functionality for Visual Studio Code.
![initial query response](../images/cdd138.png?raw=true "initial query response")   
8. This is not the kind of answer we were looking for. Let's repeat the query with the *@workspace* agent.
```
@workspace Which files are using SQL?
```
9. After executing this, you should see Copilot assessing all of the files in the workspace and then returning a more specific and expected answer.
![more specific response](../images/cdd139.png?raw=true "more specific response")


## Next ➡️
[Continue to the next Lab](lab11.md)