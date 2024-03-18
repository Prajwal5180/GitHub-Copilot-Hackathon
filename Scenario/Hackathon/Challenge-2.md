# Challenge 2: Develop an App with GitHub Copilot

### Estimated Time: 60 mins
  
## Introduction  

At **Contoso Ltd.**, a leading software development company, you, as a **software developer**, are given the task of exploring the capabilities of **GitHub Copilot**, an AI-powered coding assistant, and leveraging them in the company's software development process. The company believes that integrating AI into the development process can significantly enhance the efficiency and productivity of the development teams.

As part of this mission, you are assigned to develop a **Contact Database Application** using **GitHub Copilot**. The aim of this challenge is to understand the potential of AI in software development and to familiarize you with GitHub Copilot's capabilities. With the assistance of GitHub Copilot, you are expected to generate the necessary code, guided by the comments provided in the file. You will utilize GitHub Copilot at every stage of the development process, from generating code for empty methods to building essential features and testing the application thoroughly.

Throughout the challenge, you'll leverage Copilot's ability to understand context and provide relevant code suggestions. By engaging with Copilot Chat, you'll enhance collaboration and receive insightful coding recommendations, further enriching your coding experience.

By the end of this challenge, your goal is to have a fully functional **Contact Database Application**, developed mainly with the assistance of **GitHub Copilot**. Upon completion, you'll have not only developed a feature-rich application but also gained valuable insights into how AI can be seamlessly integrated into the development workflow. This hands-on experience with GitHub Copilot will empower you to explore its vast capabilities and unlock its potential in various development scenarios. This will demonstrate the potential of AI in software development and provide valuable insights into its practical implementation at **Contoso Ltd**.
  
## Prerequisites

Make sure you have the following from the CloudLabs-provided integrated environment:

> **Note**: Prerequisites are already set up in the CloudLabs-provided environment. If you're using your personal computer or laptop, please make sure that all necessary prerequisites are installed to complete this hackathon.

- Basic understanding of the C# programming language.  
- GitHub account.  
- [GitHub Copilot extension is installed in Visual Studio 2022.](https://docs.github.com/en/copilot/using-github-copilot/getting-started-with-github-copilot?tool=visualstudio#installing-the-github-copilot-extension-in-visual-studio)
- [GitHub Copilot chat extension is installed in Visual Studio 2022.](https://docs.github.com/en/copilot/github-copilot-chat/using-github-copilot-chat-in-your-ide#installing-the-github-copilot-chat-extension-in-visual-studio)

## Setting Up Visual Studio 2022

1.  To install GitHub Copilot extension, you can follow the below steps.

      - In the Visual Studio menu bar, click Extensions, then click Manage Extensions.

      - In the "Manage Extensions" window, click Visual Studio Marketplace, search for the GitHub Copilot extension, then click Download.

      - Close the "Manage Extensions" window, then exit and relaunch Visual Studio.

      - Optionally, to check that GitHub Copilot is installed and enabled, go back to Manage Extensions, click Installed to view your currently installed extensions, then click GitHub Copilot to see status information.

2. To install GitHub Copilot Chat extension, you can follow the below steps.

      - In the Visual Studio menu bar, click Extensions, then click Manage Extensions.

      - In the "Manage Extensions" window, click Visual Studio Marketplace, search for "GitHub Copilot Chat", then click Download.

      - Close the "Manage Extensions" window, then exit and relaunch Visual Studio.

3. Navigate to the below-provided link and fork the repository into the CloudLabs-provided GitHub account.

      ```
      https://github.com/CloudLabsAI-Azure/Contact-Database-Application
      ```

4. Clone the forked repository into Visual Studio using the CloudLabs-provided GitHub account.

5. Once the repository is cloned, locate and open the `CRUD application.sln` file from the Solution Explorer.

6. Navigate to Tools on the top panel of Visual Studio. Then click on "Nuget Package Manager," and then click on "Package Manager Console." Run the below command on the console.

      ```
      Update-Package Microsoft.CodeDom.Providers.DotNetCompilerPlatform -r
      ```

## Challenge Objectives  
1. **Develop an app:** 

      - You will be creating an application named **Contact Database Application**, a C# application, with the help of **Github Copilot**, which will let the users save the contact details of people as per requirements and also carry out the basic functions like editing their details, deleting their profiles, and so on. You will be provided with the skeleton of the application already, but you will need to build the functionalities inside the **UserController.cs** file by yourself. Your task is to complete these methods by utilizing GitHub Copilot to generate the necessary code, guided by the comments provided in the file.

      - Explore Copilot's ability to understand your context and provide relevant code suggestions.  

      - Test the application thoroughly and ensure all functionalities work as expected.

1. **Generate unit test case scripts and validate them**:

      - For each of the features in the **Contact Database Application** you built inside the **UserController.cs** file, generate the scripts for unit test cases with the help of **Github Copilot**.

      - Run the required scripts generated by the **Github Copilot** and verify that the output is coming as required.

1. **Develop and test features:** 

      - Once the methods are completed, the next step is to develop the required features for the application and test them thoroughly.

      - Utilize GitHub Copilot to generate code snippets for building essential features.

      - Test the application and make necessary modifications based on Copilot's suggestions.

1. **Use GitHub Copilot at each stage of the challenge:** 

      - Use GitHub Copilot to assist in writing meaningful commit messages that clearly describe the changes made.

      - Throughout the development process, engage with Copilot Chat to enhance collaboration and receive insightful coding recommendations.
  
## Success Criteria  

- Verify that the methods in the `UserController.cs` file are completed successfully using GitHub Copilot.  
- Verify that the developed features are working as expected.  
- Verify that all the test cases generated by Copilot have passed.  
- Make sure to successfully utilize GitHub Copilot to write commit messages.

## Additional Resources:

- Refer to the [GitHub Copilot Documentation](https://github.com/github/copilot-docs) for any clarifications or guidance during the challenge.
  
### Challenge Validation
 
1. After completing the challenge, you need to visit the **Lab Validation (1)** tab and click on the **VALIDATE (2)** button under Actions to perform the validation steps. Verify that you have met the success criteria of the challenge. 
 
    ![azure](../../media/validate01.png)
 
1. If the validation status displays **SUCCESS** for all the validation steps, **congratulations!** This means that you have completed the challenge.
 
     ![azure](../../media/validate02.png)
   
1. If the validation status displays **FAIL**, **don't worry!** This could mean that you did not perform the challenge correctly.
 
     ![azure](../../media/validate03.png)
 
1. Hover your mouse over the `i` **(1)** icon to see the error message and determine the root cause of the failure. Based on the error message, revisit the challenge as necessary, and redo the validation by clicking on the **VALIDATE (3)** button again.
   
     ![azure](../../media/validate04.png)
   
1. If you are still having trouble, you can reach out to the support team via `labs-support@spektrasystems.com` for further assistance. The support team is available to help you troubleshoot and resolve any technical issues or validation issues that may arise while the lab environment is live.

## Conclusion  
In this challenge, you've managed to develop a fully functional Contact Database application predominantly with the assistance of GitHub Copilot, demonstrating its practical usefulness in a real-world software development scenario.
You've successfully navigated through the development process, from generating code for empty methods in the UserController.cs file to building essential features for the application. You've utilized GitHub Copilot to understand your context and provide relevant code suggestions, enhancing your coding experience.

The engagement with Copilot Chat has enriched your collaboration and provided insightful coding recommendations, showcasing how AI can be seamlessly integrated into the development workflow. The test cases generated with GitHub Copilot's assistance have ensured the robustness and reliability of your application. Your achievements in this challenge have demonstrated the potential of AI in software development and provided valuable insights into its practical implementation. You've shown that with the right tools, such as GitHub Copilot, the development process can be made more efficient and productive.
  


