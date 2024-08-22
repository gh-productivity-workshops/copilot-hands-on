## Lab 13 - Stay in the flow with GitHub Copilot

**Purpose: In this lab, we'll show how you can use GitHub Copilot Chat to get answers to programming related questions without leaving your editor.**

1. Use the chat interface to ask a question about a programming topic. For example, you can ask about the latest version of a programming language, how to use a specific function, or how to solve a specific problem. Enter the question below in the chat interface.

```
What is the latest LTS version of Node.js?
```
![Use Copilot to ask programming questions](../images/pic002.png?raw=true "Use Copilot to ask programming questions")

The response is based on the information available to Copilot at the time the models were trained. There may be a link to an online source for the most current information, e.g. `official Node.js website`. 

[As of June 2024, there is a new **GitHub Copilot Enterprise** feature](https://github.blog/changelog/2024-06-14-new-copilot-enterprise-features-in-vs-code-preview/): **GitHub Copilot Enterprise** can now search Bing within chat conversations in VS Code to answer questions and find information outside of its general knowledge or your codebase. To get answers enriched with Bing search results, start your message with `@github`. Copilot will intelligently decide when to use Bing. **This feature is CURRENTLY ONLY available in GitHub Copilot Enterprise**  so, the presenter will show you how this works as this is not available in **GitHub Copilot Individual**.

2. Let's try using `@github` to get an answer based on a Bing search. Enter the question below in the chat interface.

```
@github What is the latest LTS version of Node.js?
```
![Use Bing with Copilot to ask programming questions](../images/pic003.png?raw=true "Use Bing with Copilot to ask programming questions")

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
![Visual for step 1](../images/pic006.png?raw=true "Visual for step 1")

This provides a wealth of information. To save the response, right-click anywhere in the response and select `Copy`. Now you can paste the response somewhere that you can reference later such as a **GitHub Issue** or, a **GitHub Discussion post**.

5. While we can use `@github` to get answers to programming questions, we cannot use GitHub Copilot Chat to ask general questions. For example, you cannot ask about the weather or the latest sports scores. Enter the question below in the chat interface.

```
@github Who won the Super Bowl in 1986?
```
![GitHub Copilot is only for programming](../images/pic004.png?raw=true "GitHub Copilot is only for programming")

That's ok. Everyone knows that [the Chicago Bears won Super Bowl XX in 1986](https://www.chicagotribune.com/2016/01/26/chicago-bears-win-super-bowl-xx/). 😉

![Chicago Bears win Super Bowl XX](https://www.chicagotribune.com/wp-content/uploads/migration/2016/01/26/QP6TV57DS5ABJDLYCFXR6BGJEM.jpg?w=1200 "Chicago Bears win Super Bowl XX")


## Next ➡️
[Continue to the wrap-up](labs-wrapup.md)