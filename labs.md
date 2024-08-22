# Hands-on Workshop
## GitHub Copilot - The World’s Most Widely Adopted AI Developer Tool
Revision 1.2 - 08/12/24

**Versions of dialogs, buttons, etc. shown in screenshots may differ from current version of Copilot**

**NOTE: To copy and paste in the codespace, you may need to use keyboard commands - `CTRL-C` and `CTRL-V` (Or, the appropriate keyboard commands for your OS).**

## Introduction
Welcome to the GitHub Copilot Hands-On Workshop! In this workshop, you will learn how to use GitHub Copilot, the world's most widely adopted AI developer tool. GitHub Copilot is an AI pair programmer that helps you write code faster and with fewer errors. It is powered by OpenAI's Large Language Model (LLM), which is a state-of-the-art language model trained on a diverse range of data sources, including publicly available code from GitHub. GitHub Copilot is available as an extension for Visual Studio Code and can be used in any language, including Python, JavaScript, TypeScript, Go, Ruby, Java, C++, and many more.

## Before you begin

### 1. Follow the startup instructions in [the README.md file](README.md) IF NOT ALREADY DONE!

### 2. Reivew the GitHub Copilot Extension installation

One of the advantages of using **GitHub Codespaces** for this workshop is that **GitHub Copilot** is preconfigured for you.  
1. Open `.devcontainer/devcontainer.json`.

2. If it is not visible, scroll down until you see the `"extensions"` section. 

3. Notice how the `GitHub.copilot` and `GitHub.copilot-chat` extensions are already installed. 

![GitHub Copilot Extensions are already installed](./images/pic005.png?raw=true "GitHub Copilot Extensions are already installed")

If you were using the **Visual Studio Code** application, you would have to manually install the **GitHub Copilot** extensions. Refer to [Set up GitHub Copilot in VS Code](https://code.visualstudio.com/docs/copilot/setup) for step-by-step instructions. 

**NOTE:** You can also use **GitHub Copilot** in [Visual Studio](https://docs.github.com/en/copilot/quickstart?tool=visualstudio) and [compatible JetBrains IDEs](https://docs.github.com/en/copilot/quickstart?tool=jetbrains). 

You can now close `.devcontainer/devcontainer.json` as we do not need this for anything else in this lab.

### 3. Configure your desktop to make LABS.MD always visible

Before we begin, we will configure the browser windows to make the labs.md file always visible. This will allow you to easily switch between the lab instructions and any editor windows you have open.
1. Select the labs.md tab and drag it down so that it moves into a separate window.

2. If you are on Windows, you can "snap" the labs.md tab to one side or another and select the Codespace tab as the adjacent window. 

3. Move the vertical slider until you can comfortably see the instructions in labs.md and the Codespace side by side. 

Now we can see the labs.md file to one side of the screen while we are executing the actions in the Codespace on the other side of the screen. If needed, adjust the zoom level in either or both windows as desired. 

![Split View](./images/pic001.png?raw=true "Split View")

### 4. Let us know how we are doing
<!-- Instruct lab participants to leverage GitHub disussions found here: https://github.com/DaveOps30/copilot-hands-on/discussions -->
<!-- Specifically reference the "Workshop Feedback & Suggestions" and "Workshop Issues" categories -->
We are leveraging [**GitHub Discussions**](https://github.com/DaveOps30/copilot-hands-on/discussions) located in this repository for real time issue reporting, feedback and suggestions.
- If you encounter any issues or need help, please post in the [`Workshop Issues` discussion category](https://github.com/DaveOps30/copilot-hands-on/discussions/categories/workshop-issues). Be sure to check the existing discussions to see if your question has already been answered. We also have several proctors in the room to help answer your questions and help with issues. Please raise your hand and we will help you. 
- If you have any feedback or suggestions for improvement, please let us know in the [`Workshop Feedback & Suggestions` discussion category](https://github.com/DaveOps30/copilot-hands-on/discussions/categories/workshop-feedback-suggestions). 
- When you encounter something you want to share, please post in the [`Show and Tell` discussion category](https://github.com/DaveOps30/copilot-hands-on/discussions/categories/show-and-tell).


## Lab 1 - Using GitHub Copilot to learn about GitHub Copilot 

**Purpose: In this lab, we’ll start to learn about GitHub Copilot by asking GitHub Copilot questions about GitHub Copilot.**

One way to interact with GitHub Copilot is to use the chat interface. This is a great way to ask questions about GitHub Copilot since it is a natural language interface and has been trained on a wide variety of resources.

1. Select the Chat extension icon to open the chat window. Let's start with a basic request about GitHub Copilot. Enter the following text in the prompt box.

```
Give me some suggestions for effective ways to use GitHub Copilot.
```
![Copilot Suggestions](./images/pic015.png?raw=true "Copilot Suggestions")  

Notice how GitHub Copilot Chat provides a suggestion for your next question. This is a great way to keep the conversation going. If you like the suggestion, just click on the link to use it. If you don't like the suggestion, just ignore it and enter your own question.

2. Now that we have some suggestions, let's ask for some **specific examples** of commands or prompts that can be used with GitHub Copilot. Enter the following question in the prompt box.

```
What are some examples of specific commands or prompts that can be used to interact with GitHub Copilot?
```
![Copilot Examples](./images/pic017.png?raw=true "Copilot Examples")   

3. We've covered some of the basics, let's ask about **how to get the most out of GitHub Copilot**. Enter the following question in the prompt box.

```
I am new to GitHub Copilot. How do I get the most our of GitHub Copilot ?
```
![Get the most from Copilot](./images/pic019.png?raw=true "Get the most from Copilot")   

4. One of the keys to getting the most out of AI models is to provide the right **context**. Let's ask about that. Enter the following question in the prompt box.

```
What does GitHub Copilot use for context when using AI to generate code suggestions?
```
![Context for Copilot](./images/pic021.png?raw=true "Context for Copilot")   

5. Speaking of context, there are some **common contextual keywords** that can be used in GitHub Copilot prompts. Let's ask about those. Enter the following question in the prompt box.

```
What are some common contextual keywords that can be used in GitHub Copilot prompts?
```
![Contextual Keywords](./images/pic022.png?raw=true "Contextual Keywords")   

6. What else can we do in the chat panel?

Let's see if we can use chat to learn more about Copilot's capabilities. Enter the following in the chat panel and press `Enter`.

```
/help
```
![Output of /help](./images/pic012.png?raw=true "Output of /help")

As you can see in the output there are a growing number of `Participants` and `Variables` that you can use in **GitHub Copilot Chat**. For example, review the output to answer these questions:
- Which `Participant` would you use to get the meaning of the selected lines in the terminal?
- Which `Variable` would you use to feed a specific file to **GitHub Copilot Chat** as context, even though that file may not be in an open editor at the moment? 


7. Another key to effectively using GitHub Copilot is to understand the basics of **prompt engineering**. Enter the following question in the prompt box.

```
Someone mentioned "Prompt Engineering". Explain to me the basics of prompt engineering.
```
![Prompt Engineering](./images/pic018.png?raw=true "Prompt Engineering")   

8. GitHub is always working to ensure that you can get the most out of GitHub Copilot. Let's ask about what version of Chat GPT is being used.

```
What version of Chat GPT are you using?
```
![Chat GPT version](./images/pic016.png?raw=true "Chat GPT version")   

9. GitHub Copilot is frequently being updated. Let's ask about how we can stay up to date with the latest features and announcements.

```
How can I stay up to date regarding new GitHub Copilot features and announcements?
```
![Stay up to date](./images/pic020.png?raw=true "Stay up to date")   

Now that GitHub Copilot has explained the basics and some of the keys to using it effectively, let's try to use it to **generate some code**.

**=========== END OF LAB ===========**

## Lab 2 - Learning how to create good prompts for Copilot

**Purpose: In this lab, we’ll start to learn about Copilot and how it generates code based on the prompts we provide**

1. Create a new file. In the terminal, enter

   ```
   code index.js
   ```

2. Afterwards this file should be open in a tab in the editor.

3. Let's see how Copilot responds to a generic request. Go to that tab and type in a comment that says

```
// function to parse data
```
4. Hit return and notice the code that Copilot suggested. This is likely more generic than we want, but hit tab to select that line. (Note that you should give Copilot a second to provide code suggestions before moving on to the next line.)
   
5. After hitting tab, Copilot will generate another part of the function. (If not, you may need to hit return.) Hit tab to accept it. Continue until you get a complete function (or Copilot stops generating additional code suggestions). One example of what code may look like is below.

![Copilot generated function](./images/cpho5.png?raw=true "Copilot generated function")
   
6. This prompt is not specific enough for Copilot to interpret what we want to do.  Highlight the code and delete it, so we can try again.

7. Now type a comment at the top that says

```
// function to parse url
```
8. Hit enter and you will probably see a similar line to

```
function parseURL(url) {
```

9. Just hit Tab to accept it and Enter again. Pause. After that Copilot may or may not offer a suggestion.  If it does, great - you can just hit Tab and accept it.  If not, it may be necessary to further "nudge" Copilot by giving more prompts. Only if you're not getting responses from Copilot, hit return and type the comment below to nudge Copilot.

```
// parse url
```
![nudge comment](./images/cdd3.png?raw=true "nudge comment")   

10. Only if needed, hit return and Copilot should start generating suggestions again. Pause after each return to give Copilot a chance to suggest code. Then you can just hit tab to accept each line and then return to get the next part of the code until the function is complete. You may get some blank lines along the way or for some lines you might need to hit Tab twice to accept the code if it is indented more. But just hit return until you get to the end of a function. (You will be at the end when the indentation is done.  Also Copilot may start to suggest another function in comments like // test...)

11. Suppose you're not happy with that suggestion. Copilot can provide other options for the code. To see those, make sure you are in the editor for the file, then delete all but the first line of the function **and** put the cursor at the end of the first line.

![reset for altenate choices](./images/cdd105.png?raw=true "reset for alternate choices")   
   
12. Hit **Ctrl + Enter**. A second window will open up with other suggestions.
Be patient - it takes a bit of time for Copilot to generate alternative suggestions. After a moment though, you will have up to 10 alternatives to pick from. These will be of varying quality and completeness. You can scan through these and then pick one if suitable by clicking on the **Accept suggestion #** button under the alternative suggestion.  Note that this will add the code to the existing set, so you may need to do some minor editing afterwards.

![alternative suggestions](./images/cdd106.png?raw=true "alternative suggestions")   

13. Let's do one more pass at getting a specific prompt for Copilot. Delete all the code currently in index.js. This time we will not enter a comment, but will enter a specific function name.
Type the following in the empty file. (There are no parentheses after the *splitURLandReturnComponents* text.)  Do not hit tab or return yet.

```
function splitURLandReturnComponents
```

14.  With this function name, Copilot should suggest a full function definition - in fact it may suggest several.  To see the options, hover over the first line and a small window should appear. This window will not how many options there are (probably 2 or 3) and provide "<" and ">" links to toggle between them.  Click on the "<" and ">" buttons to see the differences in the available suggestions.

![alternative suggestions inline](./images/cdd5b.png?raw=true "alternative suggestions inline")   

15. When you find an alternative you like, go ahead and tab to select it.

**=========== END OF LAB ===========**

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

![starting point](./images/cdd104.png?raw=true "starting point") 

4. Hit **Ctrl+Enter** to see options

5. Pick one of the options that is longer and/or more complex (if there is one) and **Accept suggestion #**. If there's not one that's longer/more complex, just pick an alternative one and **Accept suggestion #**.

![alternative suggestions](./images/cdd34b.png?raw=true "alternative suggestions") 

6. Highlight the code and select the Chat extension icon to open the chat window.  Tell Copilot to simplify the code by typing in the chat window.
```
simplify
```

![simplifying via chat box](./images/cdd35.png?raw=true "simplifying via chat box") 

7. Hover over the simplified text and tell Copilot to insert the suggestion at the cursor to replace the text that's currently there. 

![replace from chat suggestion](./images/cdd143.png?raw=true "replace from chat suggestion")    

8. Now, let's introduce an error into the code to see how Copilot can fix it. Pick an instance of a variable name and change it to one that doesn't exist. For example, change an instance of "n" to "x". 

![introduce error](./images/cdd37b.png?raw=true "introduce error")   

9. Notice the light bulb icon that has popped up. Click on that, scroll to the bottom (if needed), and you'll have additional options to fix or explain with Copilot.

![Copilot options inline](./images/cdd38b.png?raw=true "Copilot options inline")   

10. Go ahead and click on the "Fix using Copilot" option.

11. After a few moments, it should propose a fix that you can just accept (via the Accept button). You can also click on the *Show Changes* icon to see before/after for the proposed changes. (If it doesn't propose a fix in the dialog, you can skip to step 12 and use the /fix command in chat instead.)

![Fixing with Copilot](./images/cdd107a.png?raw=true "Fixing with Copilot")       

12. (Optional) If you'd like, you can go back and make the error again, highlight the code, and then use the /fix command in the chat window to get the same results.

**=========== END OF LAB ===========**

## Lab 4 - Using Copilot after the coding

**Purpose: In this lab, we’ll see a few other ways to leverage Copilot after the initial coding is done**

1. Now that we have some code to work with, let's see what else Copilot can do for us. Let's have it explain the current code in our *prime.py* file.  Select the code. Then, use the **Cmd+I** keys to bring up the Copilot interactive chat dialog.

![Interactively telling Copilot to explain code](./images/cdd40b.png?raw=true "Interactively telling Copilot to explain code")


2. Tell Copilot to explain the code by typing the command below in the dialog. Hit Enter. Then, you should see the output in the dialog. Click on the *View in Chat* button to see the output in the separate chat window.

```
/explain
```
![Output of interactively telling Copilot to explain code in dialog](./images/cdd144.png?raw=true "Output of interactively telling Copilot to explain code in dialog")
![Output of interactively telling Copilot to explain code](./images/cdd41b.png?raw=true "Output of interactively telling Copilot to explain code")

3. Now, let's do the same request but through a comment. In the *prime.py* file, below the code, enter the following comment and hit Enter.
```
# explain the code above line-by-line
```
4. After this, Copilot should start showing the explanation in comments. Just hit tab to accept each line and then Enter to move to the next one.

![Output of telling Copilot to explain code via comment](./images/cdd42b.png?raw=true "Output of telling Copilot to explain code via comment")

5. We can also query Copilot inline via asking a question in a comment. Delete the commented explanation and try out the question below. To be clear you can prefix it with :q but that is not required with the chat feature installed.

```
# q: what does the function above do?
```

![Prompting for what code does with q:](./images/cdd43b.png?raw=true "Prompting for what code does with q:")

6. Finally, let's see how to use the doc feature to automatically document our code. Highlight the actual code.

7. Now, enter **Cmd+I** and enter the **/doc** command. After a few moments, Copilot should generate some documentation for the code. You can go ahead and *Accept* the changes.

![Generated doc for the code](./images/cdd44d.png?raw=true "Generated doc for the code")  

8. While this is useful documentation for the start of the function, we'd like to have more extensive comments in the function body. So,let's get Copilot's help with that. Bring up the chat dialog again with **Cmd+I** and enter the text "verbosely comment this code". After Copilot completes its suggestions, if you're happy with them, you can just click *Accept*. 

![Regenerating doc](./images/cdd110.png?raw=true "Regenerating doc")  

9. Once you find a doc example you like, go ahead and click **Accept**.

**=========== END OF LAB ===========**

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
![generating tests via comment](./images/cdd46a.png?raw=true "generating tests via comment") 

4. What if we didn't know how to test the code at all? Let's ask Copilot. Highlight the *is_prime()* function.

![selecting code](./images/cdd111.png?raw=true "selecting code") 

5. Now, switch to the chat interface and ask Copilot using the following prompt:

```
#selection: How do I test this code?
```
![prompting on how to test](./images/cdd112.png?raw=true "prompting on how to test") 

6. After entering this, you should see an explanation of how to test the code along with suggested testing code. If you expand the reference in the chat output, you can see that it only used the selected lines.

![testing explanation](./images/cdd113.png?raw=true "testing explanation") 

7. Let's see what the shortcut command would do. In the chat dialog enter "/tests" and then Enter. Copilot will want to add the *@workspace* agent onto the command. Just remove the *@workspace* from the beginning of the command. **Do not hit enter yet**.
```
/tests
```
8. Type a hash/sharp sign after /tests. At this point, Copilot should present a selection dialog. Choose #file from the menu.
```
/tests #
```
   
![shortcut test command](./images/cdd140.png?raw=true "shortcut test command")

9. A dialog will pop up near the top of the codespace with a selection of files. Select the *prime.py* file to complete the command. 

![file choice dialog](./images/cdd141.png?raw=true "file choice dialog")

10. Once the command looks like */tests #file:prime.py*, go ahead and hit enter to see the suggested test results.

![file choice dialog](./images/cdd142.png?raw=true "file choice dialog")

11. We can put this into a new file by hovering over the output in the Chat window, then selecting the "..." from the pop-up menu and selecting "Insert into new file". Go ahead and select that option and then you'll have a new file in your editor with the code that you can save as needed.

![Insert tests into new file](./images/cdd115a.png?raw=true "Insert tests into new file") 



**=========== END OF LAB ===========**

## Lab 6 - Using Copilot to help with SQL

**Purpose: In this lab, we’ll see some examples of how to have Copilot help with writing SQL**

1. Create a new file named dev.sql. You can create it via entering the line below in the terminal.

```
code dev.sql
```
   
2. Afterwards this file should be open in a tab in the editor. Assume we want to work with a database or database definition that defines a dataset for students, staff, curriculums, courses, schools of study, locations, and registrations for a university system. Let's see what Copilot would generate for a query to get all students in a course - without any other context.

Enter the following comment below and press Tab to accept suggestions. Remember that you may have to hit Enter multiple times to get Copilot to prompt. Or if you don't get a suggestion or only get a comment, try "nudging" Copilot via typing "select". 
```
-- define a select statement to get all students enrolled in a course
```
3. Go ahead and save this file as part of the project.  You can do this from the "3-line" menu under File->Save, or just click on the X next to the file's name in it's tab and select to Save it.

![Save sql file](./images/cdd96.png?raw=true "Save sql file") 

4. If the file is no longer open in the tabs, you can select the "Explorer" icon at the top of the sidebar and select the file in the list to open it back up.

![Reopening the file](./images/cdd108.png?raw=true "Reopening the file")    
   
5. Let's see if we get any different results if we provide Copilot additional context. Open the file create-tables.sql in the editor from the GitHub repository. (You can either select and open it from the file list or use the command below from the terminal.) Scroll through it and take a quick look at the contents.

```
code create-tables.sql
```

6. Now with that file open, go back up to the top of the dev.sql file.  Highlight and delete the comment and resulting query from step 2.
  
7. Enter the same comment as before to request the query. (Basically, repeat step 2.) See what Copilot suggests this time. You can accept the suggestions or cycle through options. (If you first get a duplicate line as the query, just hit Enter and Copilot should start making more meaningful suggestions.)

```
-- define a select statement to get all students enrolled in a course
```

8. If all goes well, this second pass should generate a query with many more specific references to the names and identifiers used in *create-tables.sql*.  (If not, delete the result and try again.) Take a look at the query and then compare the names/identifiers used to the ones in the *create-tables.sql* file. **This will show that Copilot picks up on context from other files available to it to make better suggestions.** This is one of the key principles of **Prompt Engineering** - providing the right context to Copilot to get the best results. **Remember that Copilot is context-aware and will provide better results with more context.** Take some time now to learn more about Prompt Engineering, check out [Prompt engineering for GitHub Copilot](https://docs.github.com/en/copilot/using-github-copilot/prompt-engineering-for-github-copilot) from the GitHub documentation. 

![New query](./images/cdd97.png?raw=true "New query") 

   
9. In some cases, we might be able to use a separate index to speed up operations.  Let's ask Copilot to create a new index based on the last query. Add the following line after the current query in the file *dev.sql*.

```
-- write an index to improve the performance of the query
```
![index](./images/cdd98.png?raw=true "index") 

10. Let's suppose we also want to have a table to capture student attendance. We can ask Copilot to create the table definition for us.

```
-- define a table for student attendance to capture attendance by class
```

(Here again, if you don't get a meaningful response from Copilot, you may need to nudge it by typing *CREATE*.) In the definition Copilot provided, it may have added a comment for the status in the same format as the comment in the courses.registration table definition in the create-tables.sql file.

![status values](./images/cdd99.png?raw=true "status values") 

11. Copilot can also create stored procedures. Let's ask it to create a new stored procedure for getting a list of enrolled students at a particular location. Let's use the **CMD+I** shortcut. Go to the bottom of the *dev.sql* file, invoke Copilot Chat via the shortcut and then enter the line below in the dialog. You can choose to **Accept** or **Discard** the result.

```
define a stored procedure to get course enrollment by location
```
![prompt for stored procedure](./images/cdd100.png?raw=true "prompt for stored procedure") 
  
12. We can be more prescriptive with our stored procedure definition.  Let's add a more complex request. Go to the Chat interface extension via clicking on the icon on the tool bar (if its not already opened). In the Chat window, enter the prompt below.

```
define a stored procedure to get instructor details associated with a location
include instructor details, location details, and courses associated with the instructor
use instructor_id as the input parameter
```
![More extensive stored procedure definition](./images/cdd51.png?raw=true "More extensive stored procedure definition") 

13. Finally, let's see Copilot optimize a query for us. Suppose we want to get all the course registrations for September, 2023.  Enter the following query in the file.

```
select * from courses.registrations where year(registration_date) = 2023 and month(registration_date) = 9;
```

14. Ask Copilot to optimize the previous query. You can do this via highlighting the query (make sure to highlight the *entire* query), switch to the separate chat interface and entering "optimize" in the dialog. You can Accept or Discard the suggested optimization after that.

```
optimize
```
![Optimizing a query](./images/cdd116.png?raw=true "Optimizing a query") 

    
**=========== END OF LAB ===========**

## Lab 7 - Teaching Copilot about updates

**Purpose: In this lab, we’ll see an example of what to do when Copilot does not have the most up-to-date information**

1. Create a new file called *explore.go* via the same approach as you used to create other files.

2. This file should now be open in an editor tab. Let's say we want to seed a random number generator with Go. Let's ask Copilot to write a function to do that. Prompt it through the **CMD+I** interface using the statement below. Then you can accept the suggested code.

```
write a function to seed a random number generator
```
![Asking Copilot to write function to seed a random number generator](./images/cdd117.png?raw=true "Asking Copilot to write function to seed a random number generator") 

3. Copilot has probably generated code using the rand.Seed function. The challenge is that as of Go 1.20, the Seed function is deprecated.  Ref: https://cs.opensource.google/go/go/+/refs/tags/go1.21.0:src/math/rand/rand.go;l=394

4. Let's see if Copilot understands that this is deprecrated. We'll ask it via a query. Switch to the separate chat inferface and enter the query below.

```
Is the Seed function deprecated in Go?
```
![Is Seed function deprecated?](./images/cdd118.png?raw=true "Is Seed function deprecated?") 

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

![Updated random number gen code after including updated usage](./images/cdd119.png?raw=true "Updated random number gen code after including updated usage")

**=========== END OF LAB ===========**

## Lab 8 - Kubernetes, YAML generation and ensuring you are using the latest version

**Purpose: Show YAML generation and out of date content.**

1. Create a new file - **deployment.yaml**

```
code deployment.yaml
```

2. Bring up the Copilot Chat dialog via **CMD+I** and enter in the following request.

```
write spec for deployment in Kubernetes with 2 replicas and image from busybox
add command to run in containers: sleep 3600
add label app: myapp
add label type: front-end
```

3. After a few moments, you should see it respond with the code. You can just Accept this.
![Kubernetes manifest](./images/cdd120.png?raw=true "Kubernetes manifest")

4. Suppose we don't know how to execute this code. Let's ask Copilot. Highlight the generated YAML in the deployment.yaml file.  Then go to the larger Chat interface and ask it. Put the following in the Chat interface.

```
How do I execute this?
```

5. Copilot should respond with something like the following:

![How to execute deployment](./images/cdd121.png?raw=true "How to execute deployment")


6. While we're in the Chat interface, let's ask it for the latest K8s version. Put the following into the dialog.

```
what is the latest Kubernetes version?
```

7. Notice that it identifies the latest version as 1.28 as of October 2023. This highlights the out-of-date issue with the LLM.

![Answer to latest K8s version](./images/cdd122.png?raw=true "Answer to latest K8s version")

However, GitHub Copilot has evovled to realize that the cuurent model may not have the absolute latest information. So, the response may include a link to the Kubernetes release page: https://github.com/kubernetes/kubernetes/releases. This is an example of how Copilot can help you find the most up-to-date information. Go to that page and see what the latest version is. 


8. Let's have Copilot generate some code to work with Kubernetes through the API. In the chat interface, enter the following.

```
How do I call the K8s API for scaling a deployment to 5 replicas with Python?
```

9. The results may tell us that we first need to make sure something like PIP is installed. If so, we don't need to worry about this at the moment. Go to the actual generated code in the chat output. Click in that output area and paste the code into a new file via clicking on the "..." and then the *Insert into new file* menu option.

![Add code to new file](./images/cdd124.png?raw=true "Add code to new file")


10. Suppose we change our mind and want to convert this code to Go. Click in the new file, and highlight the new code. Then, in the Chat interface tell it to translate to Go. Then, look in the separate chat output and you should see the equivalent Go code available.

```
translate to Go 
```

11. If you look at the output from the Chat interface, you should now have the equivalent Go code available.

![Go translation](./images/cdd125.png?raw=true "Go translation")

**=========== END OF LAB ===========**
 
## Lab 9 - Exploring JavaScript, regular expression generator, auto-generating data

**Purpose: Show JavaScript and regular expression generation, auto-generate routine mappings**

1. Create a new file as **phone.js**

```
code phone.js
```

2. Prompt Copilot to create a function with a regular expression to validate a US phone number. You can use the **CMD+I** interface and just *Accept* the results.
```
create a function to validate any global phone number using a regular expression
```
![Regex function to validate phone #](./images/cdd127.png?raw=true "regex function to validate phone #")

3. Let's tell it to document the function by highlighting the code, invoking **CMD+I** and **/doc**.  You can just Accept the results.

![Automatic doc of function](./images/cdd128.png?raw=true "Automatic doc of function")  

4. Now let's see how Copilot can generate some data and mappings for us automatically. Enter the prompt below in the main/separate chat text entry area.
```
create a mapping of all 50 states to area codes where
the key is the state abbreviation and the value
 is an array of area codes with max 10
```
5. After running this, Copilot will generate the start of a list as shown below. Hover over the output area and click to insert the updates at the cursor in the *phone.js* file. (This assumes the cursor is below the previous function in the file.)

![Automatic gen of data](./images/cdd129.png?raw=true "Automatic gen of data") 

6. You can scroll to the bottom to confirm if you got entries for all the states. If you didn't, you could create additional prompts for specific ranges of states, change the number of values downward, etc. You could then copy these into your file if you want. In the past GitHub Copilot Chat may have also added the disclaimer at the bottom of the output that these may not be actual values.
   
![Disclaimer on actual values](./images/cdd132.png?raw=true "Disclaimer on actual values") 

7. Let's verify whether or not we have the actual area codes. We can ask Copilot whether or not there the area codes are the actual values. Enter the following in the chat interface.

```
Are those the actual area codes or, is that fabricated data?
```
![Verify Area Code data](./images/pic023.png?raw=true "Verify Area Code data") 

This is another exmaple of GitHub Copilot providing additional resoruces to help you verify the latest information. In this case, it's suggesting you go to the North American Numbering Plan Administration (NANPA) where you can find the most up-to-date information on area codes.  You can go to that source and see if the area codes generated by Copilot are accurate. Copilot has evolved to compensate for the fact that the LLM may not have the most up-to-date information.

**=========== END OF LAB ===========**

## Lab 10 - Agents and CLI

**Purpose: In this lab, we'll get some practice using GitHub Copilot agents and the Copilot CLI.**

1. Now let's see how Copilot can help with tasks using agents. First, we'll have Copilot help us commit a change.  Let's use the *explore.go* file we created in a previous lab. If you haven't already, make sure that file is saved. You can do this by:
- Select the *explore.go* file
- Click on the *three-line menu* in the top left.
- From the menu that comes up, select *File* and then select *Save* (or use the shortcut).
2. Now, let's invoke the **@terminal** agent to ask a common question about how to stage your code changes. Go to the *chat* interface and enter the prompt below. Afterwards, the command to do the staging should show up in the chat output.

```
@terminal how do I stage explore.go?
```
![query output](./images/cdd134.png?raw=true "query output") 

3. Hover over the window with the commands in it, and then click on the icon that pops up for the terminal. Click on that to insert the command into the terminal. Then hit return.

![insert into terminal](./images/cdd135.png?raw=true "insert into terminal")

4. Now let's commit our change through the interface and have Copilot suggest a commit message for us. Click on the source control icon in the sidebar (#1 in the figure below). Your *explore.go* file should be selected. In the box titled "Message" above the *Commit bar*, click on the *sparkle icon* at the far right side (#2 in the figure below).

![insert into terminal](./images/cdd136.png?raw=true "insert into terminal")
5. After this, Copilot should (hopefully) generate an appropriate commit message in that box. You can then copy the message and paste it into a *git commit* command in the terminal. **If you started your codespace from a fork, you can hit return to complete the commit if you want. This is optional. If you started your codespace via the one-click button, you will not have permissions to commit.**
```
git commit -m "<contents of generated commit message from Copilot goes here>"
```
![commit with generated message](./images/cdd137.png?raw=true "commit with generated message")

6. Now, let's switch gears and use the **@workspace** agent to help identify where we use certain things in our code. With the *explore.go* file still active in your editor, in the separate *chat* interface , enter the following prompt:

```
Which files are using SQL?
```

7. After executing this, you'll likely have some suggested information on how to search for files that use SQL in your project with search functionality for Visual Studio Code.
![initial query response](./images/cdd138.png?raw=true "initial query response")   
8. This is not the kind of answer we were looking for. Let's repeat the query with the *@workspace* agent.
```
@workspace Which files are using SQL?
```
9. After executing this, you should see Copilot assessing all of the files in the workspace and then returning a more specific and expected answer.
![more specific response](./images/cdd139.png?raw=true "more specific response")

**=========== END OF LAB ===========**

 ## Lab 11 - GitHub Copilot CLI 
1. Finally, let's work with the Copilot command line interface. The codespace already has the GitHub CLI installed, so we just need to install the Copilot extension and authenticate. Enter the following in the terminal.

```
gh extension install github/gh-copilot
```

2. After this, you can invoke the copilot command line to see the options available.

```
gh copilot
```
![Copilot CLI help](./images/cdd94.png?raw=true "Copilot CLI help")

3. To authenticate, use the command below in the terminal.

```
gh auth login --web
```

4. Follow the prompts. You'll get a one-time activation code that you should copy and then paste in the browser when prompted. (If you happen to get a message about an issue with GITHUB_TOKEN, you can use the command *export GITHUB_TOKEN=* to clear that.) You'll need to click on the "Authorize GitHub" button on the next screen and then confirm your signin after this to complete the process.
```   
export GITHUB_TOKEN=
```
![Copilot CLI auth](./images/cdd95.png?raw=true "Copilot CLI auth")

5. Once you have authenticate, you can try a couple of *gh copilot* commands like the ones below to see an example of how the CLI works.

```
gh copilot explain "ps -aux"
```

```
gh copilot suggest "install terraform"
```
 
**=========== END OF LAB ===========**

 ## Lab 12 - Being specific in your prompts

**Purpose: In this lab, we'll start with a simple command and then add more and more specificity and see how that impacts the suggestions we receive.**

1. The context for this exercise is that we want to create a **GitHub Actions** workflow to build a **.NET Core** application and deploy it to **Azure Web Apps**. This will also demonstrate that **GitHub Copilot** goes beyond traditional programming and can help you with many other things like CI/CD workflow files. Enter the prompt below in the chat interface.

```
Create a GitHub Actions workflow to build a .NET Core application and deploy it to Azure Web Apps.
```
![Generate a GitHub Actions Workflow](./images/pic009.png?raw=true "Generate a GitHub Actions Workflow")

Take some time to analyze the resulting **GitHub Actions** workflow. You can see that it is referencing several Actions that come from the **GitHub Marketplace**, what a time saver! We did not have to manually figure out and look up the multiple Actions that need to be used, GitHub Copilot did that for us. Your suggestion may include an important note insturucting you to properly manage the `AZURE_WEBAPP_PUBLISH_PROFILE`. This is a form of a **secret** that we would want manage very diligently to ensure that it does not fall into the hands of a hacker. We can use **Azure OpenID Connect** to avoid having to manage and store secrets like an `AZURE_WEBAPP_PUBLISH_PROFILE`. 

2. Let's refine the prompt to be more specific and see what happens. Enter the refined prompt below in the chat interface.

```
Create a GitHub Actions workflow to build a .NET Core application and deploy it to Azure Web Apps.
Use "OpenID Connect" to authenticate with Azure.
```
![Generate a GitHub Actions Workflow](./images/pic010.png?raw=true "Generate a GitHub Actions Workflow")

There may now be a `Login to Azure` step that is needed to work with **Azure OpenID Connect**. Also, the important notes will refer to `AZURE_CLIENT_ID`, `AZURE_TENANT_ID`, and `AZURE_SUBSCRIPTION_ID`. These are just identifiers for your specific Azure environment and not a form of a secret that a hacker could use to access and change your web app. By adding more specifics to our prompt, we've made our deployment more secure. 

3. This is a great start but, you should also include quality checks in your CI/CD workflow like running automated tests, load tests, etc. We can use the **Playwright** testing framework and **Azure Load Testing** for this. Let's add some more specifics to the prompt. Enter the refined prompt below in the chat interface.

```
Create a GitHub Actions workflow to build a .NET Core application and deploy it to Azure Web Apps. 
Use "OpenID Connect" to authenticate with Azure. 
After the app is deployed run a set of functional tests using the Playwright framework
then, run a set of load tests using Azure Load Tests.
```
Take a look at the new workflow and related notes. By adding more and more specifics to our prompt we were able to get a more comprehensive **GitHub Actions** workflow and, we did not have to break our flow, leave the IDE and go to the GitHub Marketplace to figure out which Actions to use. 

Now that we have this workflow, we can ask GitHub Copilot to insert the suggested workflow into a new file in our workspace. To do this you would hover over the top of the suggestion, click on the `...` and select `Insert into New File`. You may also want to copy the related notes from that chat window and paste those into your planning and tracking tool (e.g. **GitHub Issues and Projects**, Jira, Azure Boards, etc.).

![Generate a GitHub Actions Workflow](./images/pic011.png?raw=true "Generate a GitHub Actions Workflow")

The key takeaways from this lab are that you can iterate via **GitHub Copilot Chat** by adding more and more specifics to end up with a very comprehensive suggestion. So, as you are crafting prompts be sure to think about what specifics you should add to help ensure that **GitHub Copilot** provides suggestions that meet all of your requirements for scalability, maintainability, robustness, etc. Also, **GitHub Copilot** can be used to generate a lot more than just traditional "code". Where else might you want to leverage **GitHub Copilot**? Creating Infrastructure as Code files such as Terraform files? Writing PowerShell scripts? **GitHub Copilot** is your AI Pair Programmer for just about anything. 

**=========== END OF LAB ===========**

## Lab 13 - Stay in the flow with GitHub Copilot

**Purpose: In this lab, we'll show how you can use GitHub Copilot Chat to get answers to programming related questions without leaving your editor.**

1. Use the chat interface to ask a question about a programming topic. For example, you can ask about the latest version of a programming language, how to use a specific function, or how to solve a specific problem. Enter the question below in the chat interface.

```
What is the latest LTS version of Node.js?
```
![Use Copilot to ask programming questions](./images/pic002.png?raw=true "Use Copilot to ask programming questions")

The response is based on the information available to Copilot at the time the models were trained. There may be a link to an online source for the most current information, e.g. `official Node.js website`. 

[As of June 2024, there is a new **GitHub Copilot Enterprise** feature](https://github.blog/changelog/2024-06-14-new-copilot-enterprise-features-in-vs-code-preview/): **GitHub Copilot Enterprise** can now search Bing within chat conversations in VS Code to answer questions and find information outside of its general knowledge or your codebase. To get answers enriched with Bing search results, start your message with `@github`. Copilot will intelligently decide when to use Bing. **This feature is CURRENTLY ONLY available in GitHub Copilot Enterprise**  so, the presenter will show you how this works as this is not available in **GitHub Copilot Individual**.

2. Let's try using `@github` to get an answer based on a Bing search. Enter the question below in the chat interface.

```
@github What is the latest LTS version of Node.js?
```
![Use Bing with Copilot to ask programming questions](./images/pic003.png?raw=true "Use Bing with Copilot to ask programming questions")

This response is enriched with Bing search results. You can use this feature to get answers to questions that are not covered by Copilot's general knowledge or your codebase.

3. Let's see if we can use `@github` to learn about the advantages of using **GitHub Copilot**. Enter the question below in the chat interface.

```
@github Why is GitHub Copilot better and more secure to use than prompting ChatGPT and copy/pasting the code back into my IDE?
```
Does the response help you understand why GitHub Copilot is better and **more secure** to use than prompting ChatGPT and copy/pasting the code back into your IDE?

4. Learn how to get started with the **Azure OpenAI Service**

You can leverage the **Azure OpenAI Service** to build your own copilot and generative AI applications. But, how do you get started? Let's ask GitHub Copilot. Enter the question below in the chat interface, **be sure to replace `[language X]` with the language you are most likely to use, e.g. `JavaScript` or, `Python` or, `Java`, etc.** 

```
@github We use [language X] for application development. How would I get started with Azure OpenAI?
```
![Visual for step 1](./images/pic006.png?raw=true "Visual for step 1")

This provides a wealth of information. To save the response, right-click anywhere in the response and select `Copy`. Now you can paste the response somewhere that you can reference later such as a **GitHub Issue** or, a **GitHub Discussion post**.

5. While we can use `@github` to get answers to programming questions, we cannot use GitHub Copilot Chat to ask general questions. For example, you cannot ask about the weather or the latest sports scores. Enter the question below in the chat interface.

```
@github Who won the Super Bowl in 1986?
```
![GitHub Copilot is only for programming](./images/pic004.png?raw=true "GitHub Copilot is only for programming")

That's ok. Everyone knows that [the Chicago Bears won Super Bowl XX in 1986](https://www.chicagotribune.com/2016/01/26/chicago-bears-win-super-bowl-xx/). 😉

![Chicago Bears win Super Bowl XX](https://www.chicagotribune.com/wp-content/uploads/migration/2016/01/26/QP6TV57DS5ABJDLYCFXR6BGJEM.jpg?w=1200 "Chicago Bears win Super Bowl XX")


**=========== END OF LAB ===========**

## Wrap up and next steps

**GitHub Copilot can be used with almost any language!**
As you have seen in this lab, you can use GitHub Copilot to generate code in almost any language. You can also use it to generate Markdown. **GitHub Copilot** was used to generate the content of this lab guide.

### Check out these resources to dive in and learn more
If you have completed all the labs, and there is still time left in today's session you can check out the resources in [**GitHub-Copilot-Resources.md**](https://github.com/DaveOps30/copilot-hands-on/blob/main/GitHub-Copilot-Resources.md). 

This resource list has been carefully curated to help you to learn more about GitHub Copilot, how to use it effectively, what is coming in the future, what are GitHub customers saying and more. There is even a YouTube playlist that includes the latest videos from the GitHub Developer Relations team and others from GitHub. 

Add https://github.com/DaveOps30/copilot-hands-on/blob/main/GitHub-Copilot-Resources.md to your browser favorites for easy access to these resources at any time in the future.

### Looking to learn more? Check out "Microsoft Learn"
[Microsoft Learn](https://learn.microsoft.com/) has a plethora of learning paths. If you still have time in this session and/or you want to continue learning more about **GitHub Copilot**, check out the [**GitHub Copilot Fundamentals - Understand the AI pair programmer** learning path](https://learn.microsoft.com/training/paths/copilot/). Here are a few modules that serve as great follow ups to this lab: 
- [Introduction to prompt engineering with GitHub Copilot](https://learn.microsoft.com/training/modules/introduction-prompt-engineering-with-github-copilot/) - Discover the essentials of creating effective prompts with GitHub Copilot. Uncover techniques to transform your coding comments into precise, actionable code, enhancing your development workflow. (26 min)
- [Introduction to GitHub Copilot for Business](https://learn.microsoft.com/training/modules/introduction-to-github-copilot-for-business/) - Learn about the difference between **GitHub Copilot for Business** versus **GitHub Copilot for Individuals**, specific use cases and customer stories for GitHub Copilot for Business, and how to enable it. (23 min)
- [Introduction to GitHub Copilot Enterprise](https://learn.microsoft.com/training/modules/introduction-to-github-copilot-enterprise/) - Learn about the differences between **GitHub Copilot for Enterprise**, for Business, and for Individuals. Examine specific use cases, including how to enable and use **GitHub Copilot Enterprise**. (17 min)

Book mark **https://learn.microsoft.com/** so that you can explore other **Learning Paths** in the future such as [**Develop Generative AI solutions with Azure OpenAI Service**](https://learn.microsoft.com/training/paths/develop-ai-solutions-azure-openai/)


### Please let us know what you think of GitHub Copilot and this workshop
<!-- Instruct lab participants to answer the poll questions found here: https://github.com/DaveOps30/copilot-hands-on/discussions -->
<!-- Specifically reference the "Workshop Survey" poll questions. Also, mention that they can use the "Workshop Feedback & Suggestions" for general feedback and/or suggestions. -->
We would love to hear your thoughts on GitHub Copilot and this workshop. 
- Please take a moment to answer the poll questions in the [**Workshop Survey**](https://github.com/DaveOps30/copilot-hands-on/discussions/categories/workshop-survey). 
  - For each of the two questions, simply select your response and click the "Vote" button. 
  - Please feel free to leave a comment to let us know what you really liked and/or what we could do differently to make this workshop more valuable in the future. 
- If you have any feedback or suggestions for improvement, please let us know in the [`Workshop Feedback & Suggestions` discussion category](https://github.com/DaveOps30/copilot-hands-on/discussions/categories/workshop-feedback-suggestions).

<p align="center">
**THANKS!**
</p> 
