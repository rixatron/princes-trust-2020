# Setting up GitHub 

**View this in your browser: http://bit.ly/gswd-1**

## About this session
In this session you'll create a GitHub account so that you can get the material we've prepared for you.

## 1. Sign up for an account
Before you can do anything else you'll need to sign up for a GitHub account if you don't have one already.

1. Go to the [GitHub join page](https://github.com/join)
2. Fill in the form
    - Choose a username
    - Enter your email address (make sure it's one you have access to as you'll get a verification email later)
    - Choose a password
    - Follow the verification steps
3. Click Create an account at the bottom of the page once you've done the above
4. You'll be prompted to select a subscription, just choose the Free one and click Continue
5. On the next page you'll be asked some questions about programming experience, you should be able to leave these and just click "Skip personalization" to continue near the bottom of the page
6. You should get a verification email to the address you used to sign up with, click the link in the email to confirm your account or copy the launch code and enter if prompted
7. You'll get a page asking if you want to create a repository, you can ignore this page as you'll fork an existing repository in the next exercise

## 2. Fork the starter repository
Now that you have an account you will need to copy the starting repository we have created to your account. This will allow you to make your own changes to it throughout the week. This concept of copying is called "forking" in GitHub.

1. Go to the [starter repository](https://github.com/OmNomRarg/pt-web)
2. Click the "Fork" button at the top right of the page. You'll need to wait a little while for it to copy
3. You should now be taken to the page for your copy of the repository
    - If you accidentally close the browser at any point you can find your repository again by going to the [GitHub page](https://github.com/) whilst logged in. You'll see a list of repositories on the left, click the one that has your username in it

## 3. Use your repository for GitHub pages
GitHub can host a webpage for you. By enabling this you will be able to view your blog page on the internet as you develop it.

1. From your fork of the starter repository, click the "Settings" section near the top
2. Scroll down to the "GitHub Pages" section
3. In the "Source" dropdown choose "master branch"
4. You should now be able to go to your GitHub page. If you scroll back down to the GitHub pages settings you can get the url from there (it will say "Your site is published at..."). Click on the link
5. You should now see a page with "Your blog!"

## 4. Make a minor edit

GitHub lets you edit files in the browser and see the changes after a few minutes, but doesn't give fast feedback as you work on your site, so we'll use a site called Codesandbox for the editing.

1. In a new browser tab go to [Codesandbox - Sign In](https://codesandbox.io/signin)
2. Click "Sign in with GitHub"
3. You should now be prompted to Authorize CodeSandbox, click "Authorize CodeSandbox"
   - You'll be asked to login in GitHub if not logged in the current browser. Enter your sign details created in the previous steps.
4. Once your account is created you'll be prompted to confirm your chosen username and display name. Update as desired or you can leave it as it is and then click on "Finish Sign Up".
5. You should be redirected to the home dashboard with an option to create a new sandbox, click "New Sandbox" then a popup window should appear, on the left click "Import Project".
6. Go to Github where you forked a repository and copy the URL from the root of the repository and go back to CodeSandbox and paste that URL into the textbox with a placeholder of "GitHub Repository URL...", then click "Import and Fork".
7. You should now see a code editor with files listed on the left, a code view in the middle and the browser view on the right.
8. In the code editor for file 'index.html', try changing the part where it has `<h1>My blog!</h1>` to have your name in it, e.g. `<h1>Bob's blog!</h1>`. Be careful to change the contents of the `<h1>` tags and NOT the `<title>` tag!
9. Press "Ctrl + S" to save changes which should immediately appear on the right web page view.
10. To save the changes you need to commit them. Click on the Github icon on the far left menu which should bring up a small tab titled "Link to GitHub repository" and click "Link Sandbox".
11. This should update the small tab on the left where you can make commits to your forked repository. You should see a textbox with a placeholder of "Summary (required)". Enter any summary you like in this textbox. 
12. Check that "Commit directly to the master branch" option is selected and click "Commit changes"
13. If you wait a few minutes you'll now be able to see the changes reflected in your blog page if you go to the url from step 4 in the previous section. In case you've forgotten:
    - From your fork of the starter repository, click the "Settings" section near the top, scroll down to the "GitHub Pages" section and click the link where it says "Your site is published at..."
14. You should now see your page with the updated heading. If you don't see the change right away then don't worry, just give it a minute then try refreshing the page.