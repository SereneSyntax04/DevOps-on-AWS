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

![image alt](https://github.com/SereneSyntax04/DevOps-on-AWS/blob/626ba92b2e5372283492da1df408474bee3285c4/images/pipeline.png)


---
<br>


# AWS CODECOMMIT
A fully managed, secure Git-based source control service to store and manage your project files, code, and version history.
Think of it like GitHub, but inside AWS — secure, private, scalable.

- AWS CodeCommit = Git + Security + No Management Headache + AWS Integration

## Why Use CodeCommit?

- Fully managed – No need to set up or maintain your own Git server.
- Handles large repos – Unlimited files, branches, history.
- Collaborative – Team can work with Git commands they already know.
- Integrates easily – Works smoothly with AWS tools (CodePipeline, CodeBuild, etc.), IDEs, and 3rd-party tools like Jira.
- Pipeline-ready – Can trigger CI/CD pipelines when code changes.

## 🖥️ How It Works
Create a CodeCommit repository.

Users clone the repo locally using Git.

Make changes → git add / commit / push → changes go back to CodeCommit.

Repo changes can trigger pipelines, actions, or notifications.

## 🔍📢 Monitoring & Security
You can monitor AWS CodeCommit by setting up notifications for events like branch creation, new commits, and pull requests, helping teams stay updated and automate workflows. On the security side, CodeCommit uses IAM-based access control to manage permissions, supports secure access through HTTPS or SSH, encrypts data both at rest and in transit, and integrates with AWS CloudTrail for detailed audit logging.

![image alt](https://github.com/SereneSyntax04/DevOps-on-AWS/blob/626ba92b2e5372283492da1df408474bee3285c4/images/codecomit.jpg)


---
<br>


# AWS CODEBUILD
AWS CodeBuild is a fully managed service that automates the process of compiling code, running tests, and generating build artifacts.

## 🔥 Why Use CodeBuild?
- Fully managed – no need to manage or patch build servers.
- Automatically compiles source code, runs tests, and creates build artifacts.
- Supports parallel builds – faster feedback for multiple developers.
- Allows custom or preconfigured build environments (.NET, Java, Python, Node.js, Docker, etc.).
- Pulls code from CodeCommit, GitHub, S3, Bitbucket, etc.
- Works with Jenkins for simplified build pipelines.

## 🔍📢 Monitoring & Security
You can monitor AWS CodeBuild through the console, CloudWatch Logs, or other services, with real-time log streaming and optional notifications for build events. On the security side, build artifacts are encrypted both at rest and in transit, and access to build projects is controlled using fine-grained IAM resource-level permissions.

## ⚙️ How It Works

- You define a build project with source location, environment, and commands.
- CodeBuild creates a temporary Docker container for each build.
- Runs commands from a buildspec file (buildspec.yml) through different phases.
- Outputs (like packages) are uploaded to an S3 bucket.

![image alt](https://github.com/SereneSyntax04/DevOps-on-AWS/blob/626ba92b2e5372283492da1df408474bee3285c4/images/codebuild.png)

---
<br>


# AWS CODEDEPLOY
AWS CodeDeploy is a fully managed deployment service that automates software releases to AWS compute services like EC2, Lambda, ECS, and on-premises servers. It enables rapid, reliable updates with features like traffic shifting, auto rollback, and zero-downtime configurations.

## 🔥 Why Use CodeDeploy?

- Automates deployments to EC2, Lambda, Fargate, ECS, and even on-premises servers.
- Supports server, serverless, and container apps.
- Helps eliminate manual errors, enabling fast and reliable feature releases.
- Minimizes downtime with smart deployment configs (e.g., half-traffic rolling updates).
- Supports auto rollback if deployments fail.
- Scales to deploy to one or many instances at once.

## 🔍📢 Monitoring & Security
You can monitor AWS CodeDeploy using the CodeDeploy console, Amazon CloudWatch alarms, and other AWS tools to track the health and status of your deployments. For security, CodeDeploy supports IAM roles and policies to control access, is fully configurable to meet compliance requirements, and requires the CodeDeploy agent to be installed on EC2 or on-premises instances to execute deployment instructions securely.

## ⚙️ How It Works

- You define a CodeDeploy application to manage what, where, and how to deploy.
- Include an AppSpec file with deployment instructions (e.g., what scripts to run, where to copy files).
- Use deployment groups to specify target environments (e.g., EC2 instances, Lambda functions).
- Use deployment configuration to control rules—like % of healthy instances required, whether to update existing ones or swap with new.

![image alt](https://github.com/SereneSyntax04/DevOps-on-AWS/blob/626ba92b2e5372283492da1df408474bee3285c4/images/codedeploy.png)

---

<br> <br>

📌 **AWS DevOps tools** help you build, test, and deploy applications faster and more reliably. CodeCommit manages your code, CodeBuild handles building and testing, CodeDeploy automates deployments, and CodePipeline ties everything together into a smooth, automated workflow. It’s all fully managed, secure, and designed to make your software delivery easy and efficient.
