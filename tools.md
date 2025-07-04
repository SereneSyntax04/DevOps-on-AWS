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

# AWS CODEPIPELINE
📌 What is AWS CodePipeline?

- It’s a continuous delivery (CD) service
- Helps you **model, visualize, and automate** software release processes.

🔁 Automation & Speed

CodePipeline automates the entire release process—code, build, test, and deploy—reducing manual errors and delivering updates faster and more reliably.

🧩 Integration & Monitoring

Easily integrates with AWS and third-party tools, and can be monitored through the console, CLI, EventBridge, or CloudTrail to track performance, errors, and availability.

🔐 Security & Access Control

Supports fine-grained permissions, allowing specific users to view, deploy, or approve stages—ensuring secure and controlled pipeline access.



## ⚙️ How It Works
CodePipeline uses stages and actions:

✅ Stages – Steps in your pipeline:
Examples: Source → Build → Test → Deploy

🔄 Actions – Tasks inside each stage:
1. Can run sequentially or in parallel

2. Handled by service providers like:
   - AWS services: CodeBuild, Lambda, S3, CloudFormation
   - 3rd party tools: Jenkins, TeamCity

🧩 Action Types:

Source – Where the code comes from (e.g., CodeCommit, GitHub)

Build – How it's compiled (e.g., CodeBuild)

Test – How it's tested (e.g., unit tests)

Deploy – How it’s delivered (e.g., CodeDeploy)

Approval – Manual step (e.g., waiting for a manager’s OK)

Invoke – Run a custom function (e.g., AWS Lambda)



---
<br>


---
<br>


---
<br>


---
