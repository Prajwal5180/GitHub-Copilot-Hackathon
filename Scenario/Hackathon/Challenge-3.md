# Challenge 3: Deploy the App to Azure

### Estimated Time: 90 minutes

## Introduction

In the previous challenge, you successfully developed a fully functional **Contact Database application**, developed mainly with the assistance of **GitHub Copilot** and also gained valuable insights into how AI can be seamlessly integrated into the development workflow.

As a software developer at **Contoso Ltd.**, a leading software development company, in this challenge, you are tasked with exploring innovative technologies and tools that can enhance the company's software development process and infrastructure management. **Contoso Ltd.** recognizes the potential of Infrastructure as Code (IaC) in managing and provisioning its computing resources and is particularly interested in Azure Resource Manager (ARM) templates for deploying applications to Azure.

In this challenge, you will utilize **GitHub Copilot** to streamline the development of an **Azure Resource Manager (ARM)** template to deploy the fully functional **Contact Database application** which you developed earlier. ARM templates are Infrastructure as Code (IaC) files used to deploy and manage resources in Azure. By leveraging Copilot's code generation capabilities, you'll expedite the creation of an ARM template for deploying an application to Azure. In addition to this, you will also automate the build and testing process of your code. You will create a GitHub Actions pipeline, with GitHub Copilot assisting in generating the necessary scripts. To document the knowledge and insights gained from this exercise, you will use **GitHub Copilot** to generate comprehensive and accurate documentation for this challenge. This documentation will serve as a guide for creating the ARM template, setting up the GitHub Actions pipeline, and deploying the fully functional **Contact Database application** application to Azure.

By completing this challenge, you aim to demonstrate to Contoso Ltd. how **GitHub Copilot** can streamline the development of ARM templates, automate build and testing processes with GitHub Actions, and generate insightful documentation. This will further highlight the value of integrating AI into the development workflow, following the successful development of the Contact Database application in the previous challenge.

## Prerequisites

Make sure you have the following from the CloudLabs provided integrated environment:

> **Note**: Pre-requisites are already set-up in the CloudLabs provided environment. If you're using your personal computer or laptop, please make sure that all necessary prerequisites are installed to complete this Hackathon.

- [Visual Studio Code](https://code.visualstudio.com/)
- [GitHub account](https://github.com/)
- [GitHub Copilot extension](https://marketplace.visualstudio.com/items?itemName=GitHub.copilot) installed in VS Code.

## Challenge Objectives:

1. **Develop ARM Template to deploy an app to Azure:**
   - Use GitHub Copilot to assist you in generating the initial structure of an ARM template for deploying the **Contact Database application** application to Azure.
   - Define the necessary Azure resources in the ARM template, that is, a Web app present in Azure App Services required to deploy your application.

2. **Create GitHub Actions Pipeline with Copilot**
   - Create a GitHub Actions pipeline using GitHub Copilot to automate the build and testing process of your code using Copilot-generated scripts.

4. **Generate Documentation with Copilot:**
   - Use GitHub Copilot to assist you in generating a detailed and accurate documentation specifically for this challenge.
   - Create a MD file which guides in creating the ARM template to deploy the app, create GitHub actions pipeline and getting the app working on Azure.

6. **Get the app working on Azure.**
   - Deploy the application to Azure using the ARM template you've created and test the **Contact Database application's** functionality.
   - Verify that the deployed resources match the specifications outlined in your ARM template.
     
## Success Criteria:

- Verify that the web app from Azure App Services containing your application code is present in Azure.
- Veify that the Github action pipeline is created successfully.
- Verify that the documentation is created successfully.
- Verify that the **Contact Database application** is deployed successfully on Azure and test the functionality.

## Additional Resources:

- Refer [here](https://learn.microsoft.com/en-us/azure/developer/github/deploy-to-azure) for additional help.
- If you encounter any challenges or have questions, refer to the [GitHub Copilot Documentation](https://github.com/github/copilot-docs) for guidance.

### Challenge Validation
 
1. After completing the challenge, you need to visit the **Lab Validation (1)** tab and click on the **VALIDATE (2)** button under Actions to perform the validation steps. Verify that you have met the success criteria of the challenge. 
 
    ![azure](../Media/validate01.png)
 
1. If the validation status displays **Success** for all the validation steps, **congratulations!** This means that you have completed the challenge.
 
     ![azure](../Media/validate02.png)
   
1. If the validation status displays **Fail**, **don't worry!** This could mean that you did not perform the challenge correctly.
 
     ![azure](../Media/validate03.png)
 
1. Hover your mouse over the `i` **(1)** icon to see the error message and determine the root cause of the failure. Based on the error message, revisit the challenge as necessary, and redo the validation by clicking on the **VALIDATE (3)** button again.
   
     ![azure](../Media/validate04.png)
   
1. If you are still having trouble, you can reach out to the support team via `labs-support@spektrasystems.com` for further assistance. The support team is available to help you troubleshoot and resolve any technical issues or validation issues that may arise while the lab environment is live.

## Conclusion

In this challenge,  You've demonstrated how AI can significantly aid in the development and deployment of applications, specifically through the use of GitHub Copilot. Not only did you develop a fully-functional Contact Database application in the previous challenge, but you also effectively deployed it to Azure using an ARM template generated with the help of GitHub Copilot. You've utilized GitHub Copilot to streamline the creation of the ARM template, which is a powerful example of Infrastructure as Code (IaC) and also automated the build and testing process of your code by creating a GitHub Actions pipeline, with GitHub Copilot assisting in generating the necessary scripts. Furthermore, you've produced comprehensive and accurate documentation for this challenge, serving as a valuable guide for future projects.

Through this challenge, you've showcased to Contoso Ltd. the potential of integrating AI into the development workflow. You've demonstrated how GitHub Copilot can aid in not only the development of applications but also in the deployment and management of infrastructure, thus highlighting its versatility and value. By successfully deploying the Contact Database application to Azure and verifying its functionality, you've provided a tangible demonstration of the benefits of AI in software development.
