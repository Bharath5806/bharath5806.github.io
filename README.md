
# What is GitHub Pages?

GitHub is one of the most popular tools that companies and individuals use to host and version control source code repositories. The platform runs by using using Git software, which helps track code changes and streamline development collaboration. GitHub has been constantly improving the software developer experience and keeps launching new features to enhance automation and encourage even more collaboration between dev teams — with one of those features being GitHub Pages. 

GitHub Pages is a feature of GitHub that lets us host static websites from GitHub repositories and make them publicly available or even privately accessible within your team and organization. From our personal website and portfolio to our project’s documentation, GitHub Pages can help us launch websites in a matter of minutes. we will even get a URL in the form https://.github.io that we can share with the world to make your website(s) accessible to others.

## Objective:  
Deploying a simple HTML website using GitHub Pages.

### Tools used: 
 GitHub Pages

## Step 1: Creating an index.html file.

Write a HTML code: For a simple website,  with the following basic structure:

```bash
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Website</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <h1>Welcome to My Website</h1>
    <p>This is a simple static website hosted on GitHub Pages.</p>
</body>
</html>
```
Save the file as index.html: surely we have to save it with the .html extension only 
## Step 2: Pushing it to a new GitHub repo.
### Create a new repository on GitHub:
Go to github.com and log in.

Click the "+" icon in the top right corner and select "New repository."

Give our repository a name 

Choose "Public" or "Private" (Public is fine for our static website).

check "Add a README file" (for explaning our task details
)

Click "Create repository."

### Push our index.html file to the repository:

### Using Git command line:

```bash
git init
git add index.html
git commit -m "Initial commit with index.html"
git remote add origin https://github.com/Bharath5806/bharath5806.github.io.git
git branch -M main 
git push -u origin main
```

## Step 3: Go to repo → Settings → Pages → enable GitHub Pages.

1. Navigate to our repository on GitHub.

2. Click on the "Settings" tab.

3. Scroll down and click on "Pages" in the left sidebar.

4. Under "Build and deployment," in the "Source" section, Go to repo → Settings → Pages → enable GitHub Pages.

5. we have Choose the branch to deploy from (usually main or master).

6. Select the root folder (usually / (root)).

7. Click "Save."

![IMG_20250415_200158](https://github.com/user-attachments/assets/6ba33f6f-2985-49a6-be68-b24fe4bc5995)

## Step 4: Access live website from the link GitHub gives.

1. After saving in Step 2, GitHub will start building our site.

2. Once the build is complete, we'll see a message with the live website link: "our site is live at  https://bharath5806.github.io/" 

3. Click on this link to view our website.

![IMG_20250415_200134](https://github.com/user-attachments/assets/5a459594-3dde-48a9-91fc-3f7cc5e0119e)

## Step 6: Try customizing with CSS.

1. Create a new file named style.css in the same directory as our index.html file.

2. Add some CSS styles to style.css:

```bash
body {
    font-family: Arial, sans-serif;
    text-align: center;
    margin: 50px;
}
h1 {
    color: #333;
}
p {
    color: #666;
}
```

3. Link the CSS file to our index.html file by adding the following line within the <head> tags:
```bash
<link rel="stylesheet" href="style.css">
```
4. Commit and push the changes to our GitHub repository.

5. Refresh our live website to see the updated styles.

![IMG_20250415_200336](https://github.com/user-attachments/assets/362d26a3-f3df-486e-96e9-5c50f9ff50bc)


