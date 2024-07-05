# Challenge 5: Create Documentation using GitHub Copilot

### Estimated Time: 45 minutes

## Introduction

**Contoso Ltd.**, a leading software development company, is working on a significant software development project. You have previously developed an application that integrates several complex features and functionality. However, the project lacks comprehensive documentation, making it difficult for new team members to understand the code and contribute effectively. The project leads recognized this issue and decided to leverage GitHub Copilot to generate documentation and make the project more accessible and maintainable.

In this challenge, you, as a developer at **Contoso Ltd.**, will leverage **GitHub Copilot** to expedite the creation of documentation for a given project or codebase. Documentation plays a crucial role in facilitating understanding, collaboration, and maintenance of software projects. By using Copilot's code generation capabilities, you'll explore how it can assist in creating descriptive and informative documentation. You will also review the generated documentation, refining and customizing it to suit the specific requirements of the project. Ensure that the documentation provides clear explanations, usage instructions, and any other relevant details that would be helpful to developers.

By the end of this exercise, you will have a well-documented project that can be easily understood and maintained by other developers at **Contoso Ltd**. This scenario illustrates how **GitHub Copilot** can expedite and simplify the documentation process, thereby improving the efficiency and maintainability of software projects.

## Prerequisites

Make sure you have the following from the CloudLabs-provided integrated environment:

> **Note**: Prerequisites are already set up in the CloudLabs-provided environment. If you're using your personal computer or laptop, please make sure that all necessary prerequisites are installed to complete this hackathon.

- [Visual Studio Code](https://code.visualstudio.com/)
- [GitHub account](https://github.com/)
- [GitHub Copilot extension](https://marketplace.visualstudio.com/items?itemName=GitHub.copilot) installed in VS Code.
- GitHub repo [Azure-Samples/azure-search-openai-demo](https://github.com/Azure-Samples/azure-search-openai-demo) was forked to your GitHub user organization and cloned in your environment.

## Challenge Objectives:

1. **Generate documentation with Copilot:**
   - Utilize the GitHub Copilot chat to generate markdown documentation for the **backend** app and copy the documentation to a new file, **README.md** in the ***app/backend/*** directory.
     >**Hint:** Use **@workspace** file reference to generate a README.md file for the *app/backend* directory.
   - Make use of the GitHub Copilot **Generate Docs** feature to list out the requirements in the ***app/backend/requirements.txt*** file.
   - Generate comments for the ***app/backend/approaches/approach.py*** file through GitHub Copilot **Start in Editor** feature.
     >**Hint:** Access the GitHub Copilot Start in Editor feature by **Ctrl+I** shortcut in your VS Code.

   <validation step="96b4e044-86fc-4209-9733-e422716a27d7" />

2. **Enhance and refine documentation:**
   - Enhance the **README.md** markdown documentation generated in the previous challenge utilizing GitHub Copilot Suggestions.
     >**Hint:** Access the GitHub Copilot Suggestions window by **Ctrl+Enter** shortcut in your VS Code.
   - Use the appropriate suggestions, which will refine the documentation.

   <validation step="f42aa485-2434-4ae5-b2e5-475b215cae63" />

3. **Explore Various Documentation Styles:**
   - Utilize GitHub Copilot to generate a Javadoc to create a calculator.
   - Make use of GitHub Copilot to generate markdown documentation to deploy a VNet in Azure.

## Success Criteria:

- Verify that the markdown documentation for the backend app is generated successfully using GitHub Copilot chat.
- Verify that the requirements needed for the backend app are listed at the beginning of the *app/backend/requirements.txt* file by using the GitHub Copilot Generate Docs feature.
- Verify that the comments are generated for the *app/backend/approaches/approach.py* file through GitHub Copilot Inline Chat.
- Make sure that the README.md documentation is enhanced and refined through GitHub Copilot Suggestions.
- Explore the various documentation styles that GitHub Copilot provides.

## Additional Resources:

- Refer to [this link](https://learn.microsoft.com/en-us/shows/introduction-to-github-copilot/how-to-write-documentation-with-copilot-suggestions-5-of-6) for more information.

### Challenge Validation
 
1. After completing the challenge, you need to visit the **Lab Validation (1)** tab and click on the **VALIDATE (2)** button under Actions to perform the validation steps. Verify that you have met the success criteria of the challenge. 
 
    ![azure](../../media/validate01.png)
 
1. If the validation status displays **SUCCESS** for all the validation steps, **congratulations!** This means that you have completed the challenge.
 
     ![azure](../../media/validate02.png)
   
1. If the validation status displays **FAIL**, **don't worry!** This could mean that you did not perform the challenge correctly.
 
     ![azure](../../media/validate03.png)
 
1. Hover your mouse over the **`i`** **(1)** icon to see the error message and determine the root cause of the failure. Based on the error message, revisit the challenge as necessary, and redo the validation by clicking on the **VALIDATE (3)** button again.
   
     ![azure](../../media/validate04.png)
   
1. If you are still having trouble, you can reach out to the support team via `labs-support@spektrasystems.com` for further assistance. The support team is available to help you troubleshoot and resolve any technical issues or validation issues that may arise while the lab environment is live.

## Conclusion

In this challenge, you've utilized GitHub Copilot to generate comments and markdown documentation for the backend app through GitHub Copilot features. You have also enhanced and refined your newly generated markdown documentation for the backend app through GitHub Copilot Suggestions. Further, you explored the various documentation styles that GitHub Copilot provides by generating markdown documents to deploy a VNet in Azure and a Javadoc to create a calculator from scratch.
