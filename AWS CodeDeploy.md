# AWS CodeDeploy
The final piece of the puzzle! 🧩 <br>
You've written the code (CodeCommit),
You've built & tested the code (CodeBuild),
You've assembled the delivery line (CodePipeline)...

Now it's time to deliver the code to the real world.

## 🏠 Imagine You’re Running a Pizza Chain
You’ve got:
- A new recipe (your latest code)
- Built it in the test kitchen (CodeBuild)
- Now you want to deliver hot, fresh pizzas to 100 stores (servers, Lambda, ECS, EC2, etc.)

But if something goes wrong—like bad cheese 🧀 or wrong toppings—you don’t want to ruin everyone’s dinner.

## 🤖 Meet CodeDeploy — Your Smart Pizza Delivery Bot 🍕
AWS CodeDeploy is your automated delivery system. It knows:
- What to deliver (your app/code)
- Where to deliver it (EC2, Lambda, ECS, even your own servers)
- How to deliver it safely (no downtime, rollback if issues)

## ⚙️ How CodeDeploy Works – Step-by-Step
1.  You create a CodeDeploy Application – like a delivery plan.
2.  Add an AppSpec file – this is the instruction sheet:
- What files to copy
- What scripts to run before/after deployment
3.  Create a Deployment Group – choose the destinations:
- EC2 instances
- Lambda functions
- ECS tasks
4.  Choose Deployment Config – how it should roll out:
-  All-at-once (risky!)
-  One-by-one (rolling)
-  50/50 traffic shifting (safe & smart)

## 📦 AppSpec File = Delivery Instructions
Example (for EC2):
```yml
version: 0.0
files:
  - source: /
    destination: /var/www/html

hooks:
  BeforeInstall:
    - location: scripts/setup.sh
  AfterInstall:
    - location: scripts/restart.sh
```
<br>

> AWS CodeDeploy takes your built app and ships it to real servers or services — safely, automatically, and without breaking anything. If it smells smoke, it hits “undo” and saves the day.


![image alt](https://github.com/SereneSyntax04/DevOps-on-AWS/blob/89f61adde4c2f943cfdeddbd34c0e9b750e0d105/images/codedeploy.png)
