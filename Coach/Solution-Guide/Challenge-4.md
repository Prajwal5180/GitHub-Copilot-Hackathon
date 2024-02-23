# Challenge 4: Using GitHub Copilot workspace, file reference and advanced context window - Solution Guide

### Task 1: Utilizing Github Copilot Workspace

In this task, you will be utilizing the Github Copilot Workspace to enhance coding efficiency by providing contextually relevant code suggestions.

1. Open your project in VS Code where you are signed in using the CloudLabs provided Github account details.

1. From the left pane, select **Chat** icon. You will be provided with the **Github Copilot** welcome chat window.

1. In the textbox, enter **@** and select **Workspace** to start working with the **Github Copilot Workspace** agent.

1. Now, you can provide your own prompts and select **Submit** to get the response. To start with, you can ask **Github Copilot Chat** on how to start your current project by providing this prompt: `how do I start the current project?`. As you submit your prompt, Copilot would automatically analyze the current workspace files and directories split into a chunk of steps:

    1. Scans the files/directories names to understand which of them are potentially relevant to provide a response.

    1. Reads the files contents. Sometimes the whole files, sometimes only parts of them (due to the token memory limits).

    1. Creates a context from everything it was able to collect.

    1. Starts responding combining the context from the prompt and the one it was able to gain.

1. The **Github Copilot** would provide you with a step-by-step explanation of how to run your project. You can follow the same steps and verify that your project is running successfully.

    Besides that, you can also run the command `how do I start the current project?` without taking the help of the **Workspace agent** and compare the outputs.

    The output provided is extremely abstract and in the end it tells you to provide more specific information about your project type for a more accurate answer.

1. After this, you can also get the complete information about your current working project by providing the following prompt: `@workspace Tell me about the current workspace structure`.

    Analyze the generated output and verify that the structure is aligned with your actual project structure.

1. You can also try out the following example prompts and provide your own prompts as well as per yoyr curiosity and requirements, and verify the output:

    ```
    @workspace Create a new lazy-loaded page with a path “/faq”.
    ```
    ```
    @workspace How can I add a new route to my ASP.NET MVC application?
    ```
    ```
    @workspace How can I handle form submissions in ASP.NET MVC?
    ```

### Task 2: Utilize the capabilities of File referencing

In this task, you will be 