## Lab 11 - GitHub Copilot CLI 
1. Finally, let's work with the Copilot command line interface. The codespace already has the GitHub CLI installed, so we just need to install the Copilot extension and authenticate. Enter the following in the terminal.

```
gh extension install github/gh-copilot
```

2. After this, you can invoke the copilot command line to see the options available.

```
gh copilot
```
![Copilot CLI help](../images/cdd94.png?raw=true "Copilot CLI help")

3. To authenticate, use the command below in the terminal.

```
gh auth login --web
```

4. Follow the prompts. You'll get a one-time activation code that you should copy and then paste in the browser when prompted. (If you happen to get a message about an issue with GITHUB_TOKEN, you can use the command *export GITHUB_TOKEN=* to clear that.) You'll need to click on the "Authorize GitHub" button on the next screen and then confirm your signin after this to complete the process.
```   
export GITHUB_TOKEN=
```
![Copilot CLI auth](../images/cdd95.png?raw=true "Copilot CLI auth")

5. Once you have authenticate, you can try a couple of *gh copilot* commands like the ones below to see an example of how the CLI works.

```
gh copilot explain "ps -aux"
```

```
gh copilot suggest "install terraform"
```


## Next ➡️
[Continue to the next Lab](lab12.md)