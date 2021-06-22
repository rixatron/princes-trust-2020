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
5. On the next page you'll be asked some questions about programming experience, you should be able to leave these and just click to continue near the bottom of the page
6. You should get a verification email to the address you used to sign up with, click the link in the email to confirm your account
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
GitHub lets you edit files in the browser and see the changes after a few minutes, but doesn't give fast feedback as you work on your site, so we'll use a site called jsfiddle for the editing.

1. From your fork of the starter repository, click the "Code" section near the top if you're not already in it
2. You'll see a list of files, click index.html
3. You'll now see a summary of the file, to edit it click the pencil icon
4. Highlight all of the file text (that's all of the text that's in the Edit file section) by highlighting it all with the mouse, or by clicking into the box and pressing Ctrl-A on the keyboard
5. Copy the highlighted text by right clicking and selecting "Copy", or by pressing Ctrl-C on the keyboard
6. In a new browser tab go to [JSFiddle](https://jsfiddle.net/)
7. In the HTML box, paste the copied text by right clicking inside the box and selecting "Paste", or by pressing Ctrl-V on the keyboard
8. Press the "Run" button in the top left of the page
9. You should see the current appearance of your HTML in the bottom right box
10. In the HTML box, try changing the part where it has `<h1>My blog!</h1>` to have your name in it, e.g. `<h1>Bob's blog!</h1>`. Be careful to change the contents of the `<h1>` tags and NOT the `<title>` tag!
11. Press the "Run" button again and you should see your changes in the bottom right box
12. Once you're happy with the changes, you need to copy all of the text in the HTML box in JSFiddle by highlighting it with the mouse or clicking into the box and pressing Ctrl-A
13. You should switch back to the GitHub browser tab now and select all of the text within the "Edit file" section either by highlighting it with the mouse, or clicking into the box and pressing Ctrl-A
14. Now you can paste your updated text (replacing the highlighted text) by right clicking and selecting "Paste" or by pressing Ctrl-V
15. To save the changes you need to commit them. Scroll down to the "Commit changes" box and add something to the small text box to say what you've changed (e.g. "Changed blog heading"). You can leave the big text area blank and leave the selection on "Commit directly to the master branch"
16. Click "Commit changes"
17. If you wait a few minutes you'll now be able to see the changes reflected in your blog page if you go to the url from step 4 in the previous section. In case you've forgotten:
    - From your fork of the starter repository, click the "Settings" section near the top, scroll down to the "GitHub Pages" section and click the link where it says "Your site is published at..."
18. You should now see your page with the updated heading. If you don't see the change right away then don't worry, just give it a minute then try refreshing the page