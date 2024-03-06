# Challenge 4: Using GitHub Copilot workspace and File reference - Solution Guide

>**Note:** The results produced by **Github Copilot** in this particular task may not precisely align with your outcomes. This discrepancy occurs because **Github Copilot** is an AI-driven tool, which can yield variable outputs from time to time.

### Task 1: Utilizing Github Copilot Workspace

In this task, you will be utilizing the Github Copilot Workspace to enhance coding efficiency by providing contextually relevant code suggestions.

1. Open your project in VS Code where you are signed in using the CloudLabs provided Github account details.

    ![](../../media/vscode-launch.png)

1. From the left pane, select **Chat** icon. You will be provided with the **Github Copilot** welcome chat window.

    ![](../../media/vscode-copilot-chat.png)

1. In the textbox, enter **@** and select **Workspace** to start working with the **Github Copilot Workspace** agent.

    ![](../../media/@workspace.png)

1. Now, you can provide your own prompts and select **Submit** to get the response. To start with, you can ask **Github Copilot Chat** on how to start your current project by providing this prompt: `how do I start the current project?`. As you submit your prompt, Copilot would automatically analyze the current workspace files and directories split into a chunk of steps:

    1. Scans the files/directories names to understand which of them are potentially relevant to provide a response.

    1. Reads the files contents. Sometimes the whole files, sometimes only parts of them (due to the token memory limits).

    1. Creates a context from everything it was able to collect.

    1. Starts responding combining the context from the prompt and the one it was able to gain.

    ![](../../media/workspace-prompt1.png)

1. The **Github Copilot** would provide you with a step-by-step explanation of how to run your project. You can follow the same steps and verify that your project is running successfully.

    ![](../../media/workspace-solution1.png)

1. Besides that, you can also run the command `Tell me the current workspace structure.` without taking the help of the **Workspace agent** and compare the outputs.

    ![](../../media/basic-prompt.png)

    The output provided is extremely abstract and in the end, it tells you it can't provide you with the exact solution and generates only a generic solution.

1. After this, you can try the prompt using **workspace** feature and get the complete information about your current working project by providing the following prompt: `@workspace Tell me the current workspace structure`.

    ![](../../media/workspace-solution2.png)

    Analyze the generated output and verify that the structure is aligned with your actual project structure.

1. You can also try out the following example prompts and provide your own prompts as well as per your curiosity and requirements, and verify the output:

    ```
    @workspace Create a new lazy-loaded page with a path “/faq”.
    ```
    ```
    @workspace How can I add a new route to my ASP.NET MVC application?
    ```
    ```
    @workspace How can I handle form submissions in ASP.NET MVC?
    ```

### Task 2: Utilizing Github Copilot Workspace for creating a new application workspace

The Github Copilot Workspace can not only provide the instructions, answers or the detailed code snippets regarding the queries you submit to it, but it can also create the complete workspace of an application from scratch. Here, you will be creating a new simple react app named **Expense tracker** to track the expenses of the users and also modify (edit) or delete them, all by taking the help of **Github Copilot workspace**. You will be debugging the app using this feature itself, and verify the app to run successfully in your local environment. To create the `Expense Tracker` app using **Github Copilot workspace**, follow the below steps:

1. Open a new window in the **VS code** by choosing **File** from the topmost bar and then selecting **New Window**.

    ![](../../media/new-window.png)

1. Now, select **Open Folder** from the **Welcome** page and browse to the DemoApp folder, and double click to open it in your VS Code.

    ![](../../media/vscode-open-folder.png)

1. From the left pane, select **Chat** icon. You will be provided with the **Github Copilot** welcome chat window.

    ![](../../media/vscode-copilot-chat.png)

1. In the textbox, enter **@** and select **Workspace** to start working with the **Github Copilot Workspace** agent.

    ![](../../media/@workspace.png)

1. Provide the prompt `@workspace Create a workspace for an Expense tracker application with all necessary files and code.` in the test box and select **Submit** to generate the complete workspace of your Expense tracker application along with a couple of component files.

    ![](../../media/expense-tracker-workspace.png)

    >**Note:** The **Github Copilot Workspace** will not literally create the workspace with all the file structure on your disk, rather will only provide you with the blueprints you need for creating the worskspace for your application. Thus, you need to manually create the workspace in your directory by yourself.

1. Now, create the workspace for your **Expense Tracker** application by creating the required files and folders. To do so, select **Explorer** from the left pane, and choose the appropriate file/folder icons to create a new file/folder as per the workspace structure of your application.

    ![](../../media/vscode-explorer.png)

1. The workspace structure for your **Expense Tracker** application would look similar to this, as per the output generated by the **Github Copilot Workspace**:

    ![](../../media/created-workspace.png)

1. Now, generate the code for all the required components of your application by providing the relevant prompts to the **Github Copilot** under the **Chat** section. For instance, to create code for the **ExpenseForm.js** component of your application, write `@workspace How can I add functionality to the ExpenseForm component to handle user input and save expenses?` and select **Submit**.

    The **Github Copilot** will provide you the related code for the referenced component.

    ![](../../media/expense-form.png)

1. Select the **Copy** icon to copy the code and paste it in the related **ExpenseForm.js** component. Save the file.

    ![](../../media/expense-form-completed.png)

    >**Note:** Read the output generated by the **Copilot** properly and make sure you install all the required package, if asked by the Copilot, before running your application.

1. Do the similar for all the required components of your applications suggested by the **Github Copilot Workspace** in the **Github Copilot Chat**, and complete all the components.

1. Make sure to utilize the **Github Copilot Workspace** in case of any error coming in any of the components of your application. Let's say, an issue appears in **app.js** file of your application, then you can provide a similar prompt as given to know the reason behind the error, and use the advanced capabilities of the **Github Copilot Workspace** to rectify the error: `@workspace Fix the issue in app.js file.`.

    >**Note:** Make sure you use the **@workspace** command in the chatbox to utilze the workspace feature so as it can analyze the whole workspace files and directories of your application and provide you the best resolution for the error which doesn't conflict with any other component.

1. You will get an output similar to this:

    ![](../../media/error-fix.png)

    Go through the response and resolve the errors using the steps provided in it.

1. Now, when all the errors have been fixed, you can ask Copilot on how to run your application by prompting `@workspace How can I run this app?` and submitting it.

    Follow the steps provided by it and run your application.

    ![](../../media/run-app.png)

1. You can also check if all the pre-requisites required to run your **Expense tracker** app are already in place by providing the Copilot with the prompt `@workspace what are the prerequisites i should install to run this app.`

    ![](../../media/app-prerequisites.png)

    Closely review the response generated by the **Github Copilot** using its workspace feature and make sure that all these pre-requisites are installed. If not, install them using the steps mentioned in your answer.

1. Run the application and it will open in your **Edge** browser as below:

    ![](../../media/app-working.png)

### Task 3: Utilize the capabilities of File referencing

**File referencing in GitHub Copilot** refers to the AI's ability to understand and interpret the context of your project by considering the information in other files within your workspace.

When you're working on a specific file in your codebase, **GitHub Copilot** can take into account the information, functions, classes, or variables defined in other files of your project. This means it doesn't just provide suggestions based on the current file you're working on, but it can also reference other files to give you more accurate and relevant code completions. This feature is particularly useful when you're working on large projects where code is spread across multiple files. **GitHub Copilot's** ability to reference other files allows it to better understand the bigger picture of your project, resulting in more context-aware suggestions. This can significantly improve your coding efficiency and the overall quality of your code.

In this task, you will be utilizing the **Github Copilot File referencing** capability to enhance coding efficiency by providing contextually relevant code suggestions. To use the File referencing feature, follow the below steps:

1. Open your Expense Tracker project in **VS Code** where you are signed in using the CloudLabs provided Github account details.

    ![](../../media/vscode-launch.png)

1. From the left pane, select **Chat** icon. You will be provided with the **Github Copilot** welcome chat window.

    ![](../../media/vscode-copilot-chat.png)

1. In the textbox, enter **@** and select **Workspace** to activate the **Github Copilot Workspace** agent. You need this agent to analyze your whole workspace so that it can provide accurate answers and the related code blocks by referencing the correct files.

    ![](../../media/@workspace.png)

1. Now, you can use the following prompt to to understand how the file referencing feature in **Github Copilot** can accurately provide the answer for the file which you refer to it: `What is the purpose of the index.js file in my project?`

    The **Github Copilot** will take reference of the information, functions, classes, or variables defined in the file you asked the question about, and will provide you a detailed explanation of what all is there in the **index.js**. Not just the explanation, it will also provide you the related code accompanied with the answer, referenced from the provided file.

    The **Github Copilot** also automatically references the additional files in your project that may be required to provide you the best answer. To get information of those files, select **Used n references** (where **n** is the total number of files referenced from your current project) present at the start of the answer and see all the files that **Github Copilot** referenced tp provide yoy the answer.

    ![](../../media/files-referred-2.png)

    Some more prompts that you can provide to understand the feature of file referencing are:

    ```
    @workspace What does the ExpenseList.js file do in my application?
    ```
    ```
    @workspace What is the purpose of the app.js file in my project?
    ```
    ```
    @workspace How can I change the CSS for my application?
    ```
    
#### **Adding a new feature in the application using File Reference:**

In this task, you will be utilizing the File reference capability to integrate a new feature in your **Expense Tracker** application. You wil include a **Date** field in **ExpenseForm** document and display it in **ExpenseItem** and then, will be able to sort the expenses by date in the **ExpenseList** component.

To do so, follow the below steps:

1. Open your project in VS Code where you are signed in using the CloudLabs provided Github account details.

    ![](../../media/vscode-launch.png)

1. From the left pane, select **Chat** icon. You will be provided with the **Github Copilot** welcome chat window.

    ![](../../media/vscode-copilot-chat.png)

1. In the textbox, enter **@** and select **Workspace** to activate the **Github Copilot Workspace** agent. You need this agent to analyze your whole workspace so that it can provide accurate answers and the related code blocks by referencing the correct files.

    ![](../../media/@workspace.png)

1. Now, provide this prompt to include a new **Data** field in the components and let users sort their expenses accordingly: `How can I modify the ExpenseForm component to include a date field, display this date in the ExpenseItem component, and sort the expenses by date in the ExpenseList component?`

1. The **Github Copilot**  feature will reference the files you asked in the prompts as well as analyze your whole workspace and will provide you with the best possible answer. It will provide you with the code snippets that you can add in the **ExpenseForm**, **ExpenseItem** and **ExpenseList** components accordingly. You can also view the files it referenced while providing you with the answer by selecting **Used n references** (where n is the number of files referred) present at the starting of the respone.

    ![](../../media/files-referred.png)

1. You can go through the response and make the changes suggested by the **Github Copilot** using its file referencing feature and edit the components as provided in the answer.

1. Run the app and verify the **Date** component is added and working properly.

    ![](../../media/app-working-date.png)