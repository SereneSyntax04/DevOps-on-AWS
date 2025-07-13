# AWS CodeBuild
So far, we’ve baked our software 🍰 (CodePipeline), and stored the recipe safely 📚 (CodeCommit). <br>
Now, we need someone to mix the ingredients, bake the code, and make sure it works. That’s where AWS CodeBuild comes in.

---

## 🧑‍🍳 Imagine a Robo-Chef in Your Coding Kitchen
You’ve got a recipe (your code), and now you want to cook it — mix it, test if it tastes right, and pack it up 🍱.
**AWS CodeBuild** is your Robo-Chef who does all this automatically.

No tired hands. No forgotten steps. No dirty dishes. Just clean builds, fast.

## 🍳 What Does CodeBuild Actually Do?
Think of it like this:
1.  Compile = Turn raw ingredients into a cooked dish (convert code into a working program)
2.  Test = Taste test the dish (check if it works correctly)
3.  Package = Wrap it nicely (create a .zip, .jar, .exe — ready to be deployed)

## 🛠️ How It Works – Step-by-Step
1.  You define a Build Project in CodeBuild (like telling the robot chef the recipe).
2.  You give it:
- Where the code is (CodeCommit, GitHub, S3, etc.)
- What tools to use (Node.js, Java, Python, Docker, etc.)
- What to do step-by-step (via buildspec.yml file)
3.  CodeBuild creates a temporary kitchen (Docker container).
4.  It runs your recipe:
- Install stuff
- Run tests
- Compile code
- Package output
5.  It stores the final dish (artifact) in S3 or passes it to CodePipeline

And just like that — your code is built, tested, and ready to roll! 💥

# buildspec.yml-
- It’s a YAML file (a kind of text file) that tells AWS CodeBuild exactly what to do during the build process.
```yml
phases:
  install:
    # Step 1: Install any tools or dependencies
  build:
    # Step 2: Run commands to build your app (compile code)
  post_build:
    # Step 3: Do stuff after the build (run tests, create reports, upload)

artifacts:
  files:
    - "**/*"  # Step 4: What files to keep as output (usually your final code package)
```
<br>

> AWS CodeBuild is like a robot chef that compiles, tests, and packages your code—fast, secure, and without needing you to manage a single server.

![image alt](https://github.com/SereneSyntax04/DevOps-on-AWS/blob/06e4d52f98672c1c22157bf28b6085a92f0ebf2d/images/codebuild.png)
