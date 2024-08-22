# Hands-on Workshop
## GitHub Copilot - The World’s Most Widely Adopted AI Developer Tool
Revision 1.3 - 08/22/24 (Damian Brady)

**Versions of dialogs, buttons, etc. shown in screenshots may differ from current version of Copilot**

**NOTE: To copy and paste in the codespace, you may need to use keyboard commands - `CTRL-C` and `CTRL-V` (Or, the appropriate keyboard commands for your OS).**

## Introduction
Welcome to the GitHub Copilot Hands-On Workshop! In this workshop, you will learn how to use GitHub Copilot, the world's most widely adopted AI developer tool. GitHub Copilot is an AI pair programmer that helps you write code faster and with fewer errors. It is powered by OpenAI's Large Language Model (LLM), which is a state-of-the-art language model trained on a diverse range of data sources, including publicly available code from GitHub. GitHub Copilot is available as an extension for Visual Studio Code and can be used in any language, including Python, JavaScript, TypeScript, Go, Ruby, Java, C++, and many more.

## Before you begin

### 1. Follow the startup instructions in [the README.md file](README.md) IF NOT ALREADY DONE!

### 2. Review the GitHub Copilot Extension installation

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


## The Labs

1. [Using GitHub Copilot to learn about GitHub Copilot](labs/lab1.md)
2. [Learning how to create good prompts for Copilot](labs/lab2.md)
3. [Using Copilot to simplify and explain code](labs/lab3.md)
4. [Using Copilot after the coding](labs/lab4.md)
5. [Using Copilot to generate tests](labs/lab5.md)
6. [Using Copilot to help with SQL](labs/lab6.md)
7. [Teaching Copilot about updates](labs/lab7.md)
8. [Kubernetes, YAML generation and ensuring you are using the latest version](labs/lab8.md)
9. [Exploring JavaScript, regular expression generator, auto-generating data](labs/lab9.md)
10. [Agents and Terminal](labs/lab10.md)
11. [GitHub Copilot CLI](labs/lab11.md)
12. [Being specific in your prompts](labs/lab12.md)
13. [Stay in the flow with GitHub Copilot](labs/lab13.md)

## Next ➡️
[Continue to the first Lab](labs/lab1.md)