# Challenge 2: Develop an App with GitHub Copilot - Solution Guide

## Task 1: Develop an App

### Login to GitHub

- Login to [GitHub](https://github.com/login) with the CloudLabs provided GitHub account. Ensure that you are logged in to the correct GitHub account provided for this lab session.

### Fork the Repository

- Navigate to the provided GitHub repository link: [CloudLabs-CRUD-application](https://github.com/CloudLabsAI-Azure/CloudLabs-CRUD-application).

- Fork the repository into the CloudLabs provided GitHub account.

### Open Visual Studio and Clone Repository

- Launch Visual Studio and log in using the CloudLabs provided GitHub account credentials.

- Clone the forked repository by clicking on "Clone a repository" and then selecting "GitHub" under Browse a repository.

- Choose the repository you forked earlier and click on "Clone".

### Navigate to Project Files

- Once the repository is cloned, locate and open the `Contact Database application.sln` file from the Solution Explorer.

### Implement Methods using GitHub Copilot

- Navigate to the `UserController.cs` file within the `Controllers` folder.

- Use GitHub Copilot to generate code for each empty method in the `UserController.cs` file. To generate code for each empty method using GitHub Copilot, Select/highlight the lines of the empty method and then Right-click on the highlighted lines to open the context menu. From the context menu, choose the "Ask Copilot" option. In the Prompt box, type "Fill in the Index method"

- GitHub Copilot will generate a code suggestion based on the context of the method.

- Review the suggestion provided by GitHub Copilot and you can choose to accept or discard the suggestion based on its relevance to your requirements.

- Repeat this process for each empty method in the UserController.cs file until all methods are implemented.

- Following these steps will allow you to efficiently utilize GitHub Copilot to generate code for each empty method in the UserController.cs file.

### Run and test the Application

- Locate the IIS Express button (a green play button) in the toolbar and click on it. This action starts the application on localhost in a web browser.

### Create a New Contact

- In the opened web browser, navigate to the homepage of the application.

- Locate the "Create New" button and click on it.

- Fill in the required fields for Name and Email in the form provided.

- Click on the "Create" button to submit the form and create a new contact.

### Edit a Contact

- After creating a contact, return to the homepage.

- Find the contact you created in the list and locate the "Edit" button associated with it.

- Click on the "Edit" button.

- Modify the existing details (Name or Email) as desired.

- Save the changes by clicking on the "Save" button.

### Verify Details of a Contact

- Once again, return to the homepage.

- Locate the contact whose details you want to verify.

- Click on the "Details" button associated with that contact.

- Verify that the displayed details match the information you entered earlier.

### Delete a Contact

- From the homepage, find the contact you wish to delete.

- Click on the "Delete" button associated with that contact.

- A confirmation dialog will appear asking if you're sure you want to delete the contact. Confirm the action.

- Ensure that the contact is removed from the list after deletion.

By following these steps meticulously, you can thoroughly test the CRUD (Create, Read, Update, Delete) functionalities of the application and ensure its proper functioning..

## Task 2: Develop and Test Features

1. For developing features for the application we will utilize GitHub Copilot Chat. On the top panel click on View and from the options click on GitHub Copilot Chat to open the GitHub Copilot Chat.

1. Let's ask GitHub Copilot Chat "How can we add search feature/functionality to our application?"

1. GitHub Copilot will generate a response accordingly, in this case GitHub Copilot suggested us to add a new method to accept a search string as a parameter. Then, filter the userlist based on this search string before passing it to the view. It has provided us the below code that we need to add in to the `UserController.cs` file. In this code, if a searchString is provided, the userlist is filtered to only include users whose Name contains the searchString. If no searchString is provided, all users are returned.

    ```
    // GET: User
    public ActionResult Index(string searchString)
    {
        var users = from u in userlist
                    select u;
        if (!String.IsNullOrEmpty(searchString))
        {
            users = users.Where(s => s.Name.Contains(searchString));
        }
        return View(users.ToList());
    }
    ```

1. GitHub Copilot also suggested us to modify your Index view to include a form for the search string. It has provided us the below code that we need to add in the `Index.cshtml` file which is present in the path **Views\User\Index.cshtml**. This form sends a GET request to the Index action method, passing the search string as a query string parameter.


    ```
    @using (Html.BeginForm("Index", "User", FormMethod.Get))
    {
        <p>
            Find by name: @Html.TextBox("searchString") 
            <input type="submit" value="Search" />
        </p>
    }
    ``` 

1. Save both the files after making the changes. Run the application by clicking on the IIS Express button. This action starts the application on localhost in a web browser.

1. 