# AWS DevOps Tools:  
AWS tooling and infrastructure resources for DevOps practitioners.

---

To do DevOps well, you need the right tools that boost your team’s workflow and help deliver faster. AWS offers many services that support every stage of the app lifecycle. Your DevOps setup can include both AWS tools and third-party solutions, depending on your needs.

![image alt](https://github.com/SereneSyntax04/DevOps-on-AWS/blob/7fdc6ecb40c1225f769441308117d9bb8bd8a93d/images/tool.png)

# 🔁 DevOps Pipeline Phases:
## 👨‍💻 Developers

- Write code using tools like AWS Cloud9, AWS CDK, or SDKs
- Code is checked into AWS CodeCommit (Git repo)

## 💻 Code

- AWS CodeCommit stores the source code

## 🔧 Build

- AWS CodeBuild compiles the code and runs builds

## 🧪 Test

- Testing is done using CodeBuild or third-party tools

## 🚀 Deploy

- AWS CodeDeploy pushes code to servers, containers, or Lambda

## 📈 Monitor

- AWS X-Ray traces requests
- Amazon CloudWatch monitors metrics, logs, and alarms

## 🔄 Automation:

- AWS CodePipeline ties all stages together into one continuous workflow (CI/CD).

---
<br>
<br>

# AWS CODEPIPELINE
- It’s a continuous delivery (CD) service
- Helps you **model, visualize, and automate** software release processes.
- A continuous delivery (CD) service that automates your entire software release workflow—from code to production.
- Connects CodeCommit → CodeBuild → CodeDeploy into a smooth, fast, reliable pipeline.
- ![Read More]()

![image alt](https://github.com/SereneSyntax04/DevOps-on-AWS/blob/626ba92b2e5372283492da1df408474bee3285c4/images/pipeline.png)

---
<br>


# AWS CODECOMMIT
- AWS CodeCommit = Git + Security + No Management Headache + AWS Integration
- A fully managed, secure Git-based source control service for storing and managing your code.
- Think: GitHub inside AWS – private, scalable, and easy to integrate with CI/CD pipelines.
- ![Read More]()
  
![image alt](https://github.com/SereneSyntax04/DevOps-on-AWS/blob/626ba92b2e5372283492da1df408474bee3285c4/images/codecomit.jpg)

---
<br>


# AWS CODEBUILD
- A fully managed build service that compiles your source code, runs tests, and creates deployable packages.
- No servers to manage. Works with any language and scales automatically for fast feedback.
- ![Read More]()
  
![image alt](https://github.com/SereneSyntax04/DevOps-on-AWS/blob/626ba92b2e5372283492da1df408474bee3285c4/images/codebuild.png)

---
<br>


# AWS CODEDEPLOY
- A deployment automation service that ships your application to EC2, Lambda, ECS, or on-prem servers.
- Supports zero-downtime updates, traffic shifting, and automatic rollback if something breaks.
- ![Read More]()

![image alt](https://github.com/SereneSyntax04/DevOps-on-AWS/blob/626ba92b2e5372283492da1df408474bee3285c4/images/codedeploy.png)

---

<br> <br>

📌 **AWS DevOps tools** help you build, test, and deploy applications faster and more reliably. CodeCommit manages your code, CodeBuild handles building and testing, CodeDeploy automates deployments, and CodePipeline ties everything together into a smooth, automated workflow. It’s all fully managed, secure, and designed to make your software delivery easy and efficient.
