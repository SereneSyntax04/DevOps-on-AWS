# 🚀 Building a CI/CD Pipeline with AWS DevOps Services
## 1️⃣ Write & Store Your Code **(Source Stage)**
AWS Cloud9:
- Cloud-based IDE you can access from anywhere. Write, edit, and run code in your browser. 
- Alternatives: Visual Studio Code, JetBrains, etc.

AWS CodeCommit:
- Private Git-based repository for source control. Securely stores your code and tracks changes.
> [ Your Code ] --> [ Cloud9 IDE ] --> [ CodeCommit Repository ]


## 2️⃣ Build & Test Your Code **(Build Stage)**
AWS CodeBuild:
- Compiles your source code.
- Runs unit tests and integration tests.
- Packages artifacts for deployment.
- Fully managed, scales automatically.

> [ CodeCommit Repo ] --> [ CodeBuild (Build & Test) ] --> [ Build Artifacts ]


## 3️⃣ Deploy Your Code **(Deploy Stage)**
AWS CodeDeploy: <br>
Deploys your application to:
- EC2 Instances
- On-Premises Servers
- Lambda Functions (if needed)
- Ensures smooth deployments with rollback options.

> [ Build Artifacts ] --> [ CodeDeploy ] --> [ Target Servers (EC2 / On-Prem) ]

![image alt]()



## 4️⃣ Automate Everything **(Pipeline Orchestration)**
AWS CodePipeline: 
- Connects all stages — Source → Build → Deploy
- Automates the entire release process whenever code is changed.

> [ Source ] --> [ Build ] --> [ Deploy ]  
>  |___________ CodePipeline ____________|

## 5️⃣ Simplify Setup (Optional but Handy)
AWS CodeStar:
- All-in-one dashboard to set up your projects with CodeCommit, CodeBuild, CodeDeploy, and CodePipeline.
- Good for beginners or quick project bootstrapping.

![image alt]()
