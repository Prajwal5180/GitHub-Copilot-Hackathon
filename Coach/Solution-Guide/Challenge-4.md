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

**File referencing in GitHub Copilot** refers to the AI's ability to understand and interpret the context of your project by considering the information in other files within your workspace.

When you're working on a specific file in your codebase, **GitHub Copilot** can take into account the information, functions, classes, or variables defined in other files of your project. This means it doesn't just provide suggestions based on the current file you're working on, but it can also reference other files to give you more accurate and relevant code completions. This feature is particularly useful when you're working on large projects where code is spread across multiple files. **GitHub Copilot's** ability to reference other files allows it to better understand the bigger picture of your project, resulting in more context-aware suggestions. This can significantly improve your coding efficiency and the overall quality of your code.

In this task, you will be utilizing the **Github Copilot File referencing** capability to enhance coding efficiency by providing contextually relevant code suggestions. To use the File referencing feature, follow the below steps:

1. Open your project in **VS Code** where you are signed in using the CloudLabs provided Github account details.

1. From the left pane, select **Chat** icon. You will be provided with the **Github Copilot** welcome chat window.

1. In the textbox, enter **@** and select **Workspace** to activate the **Github Copilot Workspace** agent. You need this agent to analyze your whole workspace so that it can provide accurate answers and the related code blocks by referencing the correct files.

1. Now, you can use the following prompt to to understand how the file referencing feature in **Github Copilot** can accurately provide the answer for the file which you refer to it: `What is the purpose of the RouteConfig.cs file in my project?`

    The **Github Copilot** will take reference of the information, functions, classes, or variables defined in the file you asked the question about, and will provide you a detailed explanation of what all is there in the **RouteConfig.cs**. Not just the explanation, it will also provide you the related code accompanied with the answer, referenced from the provided file.

    The **Github Copilot** also automatically references the additional files in your project that may be required to provide you the best answer. To get information of those files, select **Used n references** (where **n** is the total number of files referenced from your current project) present at the start of the answer and see all the files that **Github Copilot** referenced tp provide yoy the answer.

    Some more prompts that you can provide to understand the feature of file referencing are:

    ```
    @workspace What does the BundleConfig.cs file do in my ASP.NET MVC application?
    ```
    ```
    @workspace What is the purpose of the CRUD application 2.sln file in my project?
    ```
    ```
    @workspace How can I change the CSS for my application?
    ```
    
