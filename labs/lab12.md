## Lab 12 - Being specific in your prompts

**Purpose: In this lab, we'll start with a simple command and then add more and more specificity and see how that impacts the suggestions we receive.**

1. The context for this exercise is that we want to create a **GitHub Actions** workflow to build a **.NET Core** application and deploy it to **Azure Web Apps**. This will also demonstrate that **GitHub Copilot** goes beyond traditional programming and can help you with many other things like CI/CD workflow files. Enter the prompt below in the chat interface.

```
Create a GitHub Actions workflow to build a .NET Core application and deploy it to Azure Web Apps.
```
![Generate a GitHub Actions Workflow](../images/pic009.png?raw=true "Generate a GitHub Actions Workflow")

Take some time to analyze the resulting **GitHub Actions** workflow. You can see that it is referencing several Actions that come from the **GitHub Marketplace**, what a time saver! We did not have to manually figure out and look up the multiple Actions that need to be used, GitHub Copilot did that for us. Your suggestion may include an important note insturucting you to properly manage the `AZURE_WEBAPP_PUBLISH_PROFILE`. This is a form of a **secret** that we would want manage very diligently to ensure that it does not fall into the hands of a hacker. We can use **Azure OpenID Connect** to avoid having to manage and store secrets like an `AZURE_WEBAPP_PUBLISH_PROFILE`. 

2. Let's refine the prompt to be more specific and see what happens. Enter the refined prompt below in the chat interface.

```
Create a GitHub Actions workflow to build a .NET Core application and deploy it to Azure Web Apps.
Use "OpenID Connect" to authenticate with Azure.
```
![Generate a GitHub Actions Workflow](../images/pic010.png?raw=true "Generate a GitHub Actions Workflow")

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

![Generate a GitHub Actions Workflow](../images/pic011.png?raw=true "Generate a GitHub Actions Workflow")

The key takeaways from this lab are that you can iterate via **GitHub Copilot Chat** by adding more and more specifics to end up with a very comprehensive suggestion. So, as you are crafting prompts be sure to think about what specifics you should add to help ensure that **GitHub Copilot** provides suggestions that meet all of your requirements for scalability, maintainability, robustness, etc. Also, **GitHub Copilot** can be used to generate a lot more than just traditional "code". Where else might you want to leverage **GitHub Copilot**? Creating Infrastructure as Code files such as Terraform files? Writing PowerShell scripts? **GitHub Copilot** is your AI Pair Programmer for just about anything. 


## Next ➡️
[Continue to the next Lab](lab13.md)