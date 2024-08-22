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
![Kubernetes manifest](../images/cdd120.png?raw=true "Kubernetes manifest")

4. Suppose we don't know how to execute this code. Let's ask Copilot. Highlight the generated YAML in the deployment.yaml file.  Then go to the larger Chat interface and ask it. Put the following in the Chat interface.

```
How do I execute this?
```

5. Copilot should respond with something like the following:

![How to execute deployment](../images/cdd121.png?raw=true "How to execute deployment")


6. While we're in the Chat interface, let's ask it for the latest K8s version. Put the following into the dialog.

```
what is the latest Kubernetes version?
```

7. Notice that it identifies the latest version as 1.28 as of October 2023. This highlights the out-of-date issue with the LLM.

![Answer to latest K8s version](../images/cdd122.png?raw=true "Answer to latest K8s version")

However, GitHub Copilot has evovled to realize that the cuurent model may not have the absolute latest information. So, the response may include a link to the Kubernetes release page: https://github.com/kubernetes/kubernetes/releases. This is an example of how Copilot can help you find the most up-to-date information. Go to that page and see what the latest version is. 


8. Let's have Copilot generate some code to work with Kubernetes through the API. In the chat interface, enter the following.

```
How do I call the K8s API for scaling a deployment to 5 replicas with Python?
```

9. The results may tell us that we first need to make sure something like PIP is installed. If so, we don't need to worry about this at the moment. Go to the actual generated code in the chat output. Click in that output area and paste the code into a new file via clicking on the "..." and then the *Insert into new file* menu option.

![Add code to new file](../images/cdd124.png?raw=true "Add code to new file")


10. Suppose we change our mind and want to convert this code to Go. Click in the new file, and highlight the new code. Then, in the Chat interface tell it to translate to Go. Then, look in the separate chat output and you should see the equivalent Go code available.

```
translate to Go 
```

11. If you look at the output from the Chat interface, you should now have the equivalent Go code available.

![Go translation](../images/cdd125.png?raw=true "Go translation")


## Next ➡️
[Continue to the next Lab](lab9.md)