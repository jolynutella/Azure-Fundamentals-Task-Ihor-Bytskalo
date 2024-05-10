# Azure-Fundamentals-Task-Ihor-Bytskalo

This repository stores the source code of a simple personal website deployed to Azure Static Web Apps using GitHub Actions.

**Azure Fundamentals Practical Task**  
by Ihor Bytskalo

Hello! In this document, I will describe a step-by-step process of completing Azure Fundamentals Practical Task - deploying a simple personal website using Git and GitHub, GitHub Actions, and Azure Static Web Apps.

**Step 1: Creating a private GitHub repository to store source code**  
Probably every IT project starts with creating a git repository for storing the source code of an application so let’s begin with this.

*Picture 1 - Creating a private GitHub repository.*

*Picture 2 - Successfully created private GitHub repository.*

**Step 2: Cloning remote repository to local environment**  
Now let’s add this repository to a code editor - Visual Studio Code.

*Picture 3 - Cloning repository to Visual Studio Code using https web URL.*

*Picture 4 - Successfully cloned repository to Visual Studio Code.*

**Step 3: Creating a dev branch**  
After the cloning process is completed we can move further. Currently there is only one branch - main. So let’s add another branch called dev to mock a common process of software development: a developer creates a branch for his feature, writes code to implement it, creates a pull request and requests a code review from another developer. Upon code reviewing and merging checks we can merge dev branch to main branch.

*Picture 5 - Two branches now present in a repository: dev and main.*

**Step 4: Creating the personal website**  
From this point we can proceed to code a simple personal website.

*Picture 6 - Project structure of a simple personal website.*  
The next step is committing changes to a dev branch.

*Picture 7 - Committing changes to dev branch.*

Now we can go to the GitHub repository of this project and see that the dev branch is ahead of the main branch so we need to create a pull request.

*Picture 8 - Creating a pull request.*

*Picture 9 - Pull request created successfully and is ready to merge into the main branch.*

**Step 5: Deploying to Azure Static Web Apps**  
After the dev branch was successfully merged to the main branch we can continue with deployment of this personal website to Azure Static Web Apps.

*Picture 10 - Azure Static Web Apps page.*

Now let’s create a new web app.

*Picture 11 - Configuration of a new static web app.*

*Picture 12 - A successful deployment of a static web app.*

Now we can go to the resource and see a public URL for this web app there.

*Picture 13 - Overview of deployed simple personal website.*

So let’s visit that URL and see a beautiful simple personal website deployed on Azure servers.

*Picture 14 - Home section overview.*

*Picture 15 - About section overview.*

*Picture 16 - Projects section overview.*

*Picture 17 - Contact section overview.*

Now let’s hit that ‘Download CV’ button to test if it will download a CV pdf file.

*Picture 18 - CV pdf file downloaded successfully.*

**Step 6: CI/CD using GitHub actions**  
One of the major advantages of Azure Static Web Apps is that it can automatically create a GitHub Actions workflow so we don’t need to do it by ourselves.

*Picture 19 - GitHub Actions workflow file created by Azure.*

*Picture 20 - Successfully completed workflow.*

**Step 7: Creating a new feature to trigger CI/CD pipeline**  
Since the first deployment was successful, let’s code a new feature. I will add a new skill group called languages into the about section. But before this let’s visit the environments page in the static web app to ensure that we have only one deployment as of time being.

*Picture 21 - Environments page with only one deployment.*

So let’s code that new feature.

*Picture 22 - Committing changes to dev branch.*

*Picture 23 - Creating pull request.*

*Picture 24 - Pull request created successfully.*

After merging the dev branch to the main branch CI/CD pipeline started immediately and delivered the new code to Azure Static Web Apps and we now can check a new version of a personal website.

*Picture 25 - Successfully completed workflow after second merge.*

*Picture 26 - Updated about section with new skill box.*

**Step 8 (Extra): Previewing changes before merging to the main branch**  
Another amazing feature of Azure Static Web Apps is that we can preview committed changes to other branches before merging them to the main branch. So let’s repeat the whole workflow of coding a new feature and committing changes to the dev branch. I have slightly updated the home section and added one more sentence about me. After creating a pull request we can visit the environments page in Azure Static Web Apps and find out that there is a new preview environment. At this point we have two environments: production and preview. Let’s compare them.

*Picture 27 - Environments page with two deployments.*

*Picture 28 - Preview deployment.*

*Picture 29 - Production deployment.*

I’m happy with the change so I will merge the dev branch to the main branch and in a matter of seconds the new production version will be deployed.

That’s it! In the end, I want to say that I really enjoyed deploying my personal static website to Azure Static Web Apps - it was easy and fun. Also thank you for your time reading and reviewing this document!

**My website is available here:**  
[https://victorious-ground-0ff14fa10.5.azurestaticapps.net/](https://victorious-ground-0ff14fa10.5.azurestaticapps.net/)

**GitHub repository of the project:**  
[https://github.com/jolynutella/Azure-Fundamentals-Task-Ihor-Bytskalo](https://github.com/jolynutella/Azure-Fundamentals-Task-Ihor-Bytskalo)

**References**  
Personal static website was built following this tutorial available on YouTube:  
[https://www.youtube.com/watch?v=jVD9ZmWxhX8&t=202s&ab_channel=Ludiflex](https://www.youtube.com/watch?v=jVD9ZmWxhX8&t=202s&ab_channel=Ludiflex)  
Website was deployed following this tutorial available on YouTube:  
[https://www.youtube.com/watch?v=6uaiGqCwDgs&ab_channel=HarryLowton](https://www.youtube.com/watch?v=6uaiGqCwDgs&ab_channel=HarryLowton)

