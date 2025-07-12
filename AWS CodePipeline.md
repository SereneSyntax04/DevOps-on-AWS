# AWS CodePipeline

imagine this like a fun little story, like you're running a bakery 🍰, but instead of baking cakes, you're making software! 
 <br> And AWS CodePipeline is like your automated baking and delivery machine that makes sure your software gets built, tested, and delivered to your customers—fresh, fast, and without mistakes.

---

## 🧁 Imagine You're Running a Software Bakery
Every day, you get new cake orders (code updates), and your goal is to:

1.  Make the batter (write the code)
2.  Bake it (build the code)
3.  Taste-test it (test it)
4.  Box it up (deploy it)
5.  Send it to the customer (launch it live!)

Now, doing this by hand every time is tiring and can cause mistakes. So what do you do?

## 🤖 Meet AWS CodePipeline – Your Bakery Robot!
AWS CodePipeline is like a robot assembly line for your software.
Once you give it the recipe (pipeline), it handles the entire process on its own:

- Step-by-step Robot Stations (Stages)
The pipeline has STAGES, just like different sections in your bakery:

1. Source: Where the ingredients (code) come from – GitHub, CodeCommit
2. Build: Mix the ingredients (compile code) – CodeBuild
3. Test: Taste test (run unit tests) – CodeBuild, other tools
4. Deploy: Box it up and ship to customers – CodeDeploy, S3, EC2
5. Approval: Ask a manager for the green light if needed
6. Invoke: Do a special trick like calling a custom recipe (Lambda function)

- Each of these steps has ACTIONS, which are tasks done inside the stage. Actions can run:
1. In order (e.g., build first, then test)
2. At the same time (like test + deploy together)


> AWS CodePipeline is a fully automatic CI/CD service that kicks in the moment you change your code—automatically building, testing, and deploying without manual steps. <br>
> It's fast, reduces errors, offers full visibility through AWS tools like CloudWatch, and keeps things secure with customizable permissions. <br>
> It integrates seamlessly with both AWS services (like CodeBuild, Lambda, S3) and external tools (like GitHub, Jenkins).


**CodePipeline takes your code and walks it through a step-by-step process—automatically—until it's ready to be used by real people.**

![image alt](https://github.com/SereneSyntax04/DevOps-on-AWS/blob/308ec9dfed03787cb450510506e89da3b62e4b0c/images/pipeline.png)
