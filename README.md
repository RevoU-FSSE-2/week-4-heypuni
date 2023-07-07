
# Welcome to Match Dog!

A website specially dedicated to all dog lovers who want to adopt a dog, or two. Here, you will find a collection of adorable photos of dogs, be able to know your type of dog-mate some testimonials, and cute videos. Last but not least, fill the sign-up form to snatch one of our lovely dogs to your home now! Featuring photo collection, testimonials, cute videos, and a registration form, feel free to explore!

Go to [matchdog.site](matchdog.site) now, or check out the deployment process below.

# Development Process

This section will documentation the whole processes of deployment: how to sign up for Netlify, connect it to GitHub project, enable auto deployment, and connect a custom domain with DNS. Stay tune!

# Netlify Sign Up Process and connect Netlify to Github Project
1. Visit the [Netlify website](https://app.netlify.com/signup) and click on the "Sign Up button". 
2. You can choose to sign up with your github account or Gitlab. Here, I used my own github account.
![Signup](images/signup1.png)
3. Github will be asking for your authorization to access your account. Click "Authorize Netlify" to continue.
4. You will asked several questions. Answer and follow the instructions.
![Survey](images/signup5.png)
5. You will be redirected to the Netlify homepage. On the Connect to Git Provider section, click on the "Github"
6. As before, github will ask for authorization. Click "Authorize" and proceed to Install Netlify. 
![Install Netlify](images/deploy2.png)
7. Next, pick the repository you want to deploy. Here, I picked week-4-heypuni.
![repository](images/signup3.png)
8. Customize the deployment settings based on your requirements, including selecting the branch you want to deploy. Then deploy the site. 
8. Your site is deployed, now you will be redirected to the homepage.
![Netlify deployed](images/signup4.png)
9. After successfully linking your repository, Netlify will automatically initiate deployments whenever there are any changes in your GitHub repository.

# Custom Domain and DNS

## Buy Custom Domain
1. Go to [Niagahoster](https://www.niagahoster.co.id/) to buy your domain
2. In the search box, enter the domain you desire. For example, matchdog.site. 
![Buydomain 1](images/buydomain1.png)
3. Click "Check Now" to check the availability of your chosen domain name. 
4. If your domain is available, proceed to click "Choose".
![Buydomain 2](images/buydomain2.png)
5. Click "Choose". Then, you can also choose to change the rental duration according to your preferences. 
![Buydomain 3](images/buydomain3.png)
6. Once you click "Continue", you will be redirected to the payment page.
![Buydomain 4](images/buydomain4.png)
7. Choose your preferred payment options (bank transfer, QRIS, etc) and click "Checkout Now".
8. Fill in your identity, and follow further instructions by Niagaholster to proceed the payment process. 

## Add Custom Domain to Netlify
1. Open [Cloudfare](https://www.cloudflare.com/) in your web browser. 
2. Sign up on Cloudfare if you don't have an account yet.
3. Afterwards, click on "Add a website or an application".
![Cloudfare 1](images/cloudfare1.png)
4. Enter your domain in the search box. Click "Add site".
![Cloudfare 2](images/cloudfare2.png)
5. Choose your preffered package (Free, Pro, Business, Enterprise) according to your needs.
![Cloudfare 3](images/cloudfare3.png)
6. Review your DNS records and then "Continue", and "Confirm" to set up your DNS.
![Cloudfare 4](images/cloudfare4.png)
![Cloudfare 5](images/cloudfare5.png)
7. Cloudfare will ask you to change your nameservers on the registar's service page. 
![Cloudfare 6](images/cloudfare6.png)
8. Copy the two nameservers given by Cloudfare to your Netlify account.
![Cloudfare 9](images/cloudfare9.png)
9. Afterwards, copy your Netlify's original domain, and go back to Cloudfare.
![Cloudfare 13](images/cloudfare13.png)
10. Go back to Cloudfare, on the left-side menu, go to DNS - Records.
![Cloudfare 12](images/cloudfare12.png)
11. The DNS will be displayed if you've successfully changed your nameservers. The process might take a few minutes or maximum of 24 hours to complete.
12. The next step is to add DNS record on Cloudfare. Click "Add Record" and choose your DNS record types.
13. On the name field, type "@" and copy the Netlify domain name to the "target" field.
![Cloudfare 15](images/cloudfare15.png)
14. Proceed to "Save".
15. Go back to Netlify - Domains section and click "Add a domain".
![Cloudfare 16](images/cloudfare16.png)
![Cloudfare 17](images/cloudfare17.png)

# Pull Request and Merge on Github.

In this documentation, you will be guided through the process of creating a new branch within a GitHub repository, adding files, committing changes, pushing them to GitHub, creating a pull request, and ultimately merging the changes into the main branch.

## Pull Request
1. Sign in to your Github account.
2. On your local machine, open a terminal and use the git clone command to clone the repository to your local storage.
    ```
    git clone https://github.com/your-username/repository-name.git
    ```
3. Move into the cloned repository's directory.
    ```
    cd repository-name
    ```
4. Go to your github repository from web browser. Click on "main" branch, and create a new branch by typing the name.
![PullRequest2](images/pullreq2.png)
5. After the branch is created, feel free to make the necessary changes to the code or files in your local repository.
6. If you're still on main branch, change your branch through terminal by 
    ```
    git checkout branch-name
    ```
7. Use **git status** to check the modified files and git diff to view the specific changes. Once satisfied, use **git add .** to stage the changes and **git commit -m "Commit message"** to commit them.
8. Push the changes to your github repository **git push origin branch-name**.
9. Go to the original repository's GitHub page and click on the "Compare & Pull Request" button. 
![PullRequest3](images/pullreq3.png)
10. The repository owner or reviewers will review your pull request. They may suggest changes or ask for more information. Once approved, they will merge your changes into the main branch.


## Merge
1. Ensure that the pull request contains the desired changes and that there are no conflicts.
2. Click on the "Merge" button in the pull request discussion. 
3. After merging, add a descriptive commit message and confirm the merge.


That's all! Have a nice day folks!