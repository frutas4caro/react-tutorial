<link rel="stylesheet" href="style.css">


# 🎉 React learning guide

Welcome! Navigate to specifc content that you are interested in or come on this journey and build a full blown progressive **React app**!

## 📌 Getting Started
### Set up your local environment

We will get to the fun part soon! Don't let the challeges of setting up your local environment discourage you. There is good learning in the process ✨

These instructions are assuming you are using the terminal window on a mac. If you are using a windows computer reference the [node website](https://nodejs.org/en/download).

#### Install Node

Instructions to install  Node.js in your mac:

- If you don’t have Homebrew installed, install it first ( you can check if you have it by running the `brew -v` command the result should look something like this `Homebrew 4.4.15` - the version number might differ):

```
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

- Once Homebrew is installed, use it to install Node.js:
```
brew install node
```

- Verify the installation:
```
node -v
npm -v
```

### 2. Install a code editor like VS Code.
An IDE or Integrated development environment provides great tools and support when building and running apps

### 3. Create the app!
Use `create-react-app` or Vite for a faster, lightweight setup:

- substitute `your-app-name` with a name for your app i.e. learning-platform-phase1

```
npx create-react-app npx create-react-app
cd npx create-react-app
npm start
```

The `npm start` command will start the application locally. If you navigate to `http://localhost:3000/` on your browser, you should see the service running. 

#### Potential Problems
When running `npx create-react-app app-name` you may see dependency incompatibility issues like below and there are a few ways to resolve this:
```
npm error Found: react@19.0.0
npm error node_modules/react
npm error   react@"^19.0.0" from the root project
npm error
npm error Could not resolve dependency:
npm error peer react@"^18.0.0" from @testing-library/react@13.4.0
```
In the case above the dependency @testing-library/react@13.4.0 version expects a version of React that is compatible with ^18.0.0, but you are using React 19.0.0, which is not compatible with this peer dependency.

#### Potential Resolutions

1. **Solution 1:** Downgrade React to a Compatible Version. In the example above you can downgrade to v 18 as follows:
```
npm uninstall react react-dom
npm install react@18 react-dom@18
```
2. **Solution 2:** Update Testing Library:
```
npm info @testing-library/react versions

npm install @testing-library/react@<compatible-version>
```

### Pushing to Vercel Repository 

Imaging the obscure process of deploying a web application to the web can be intimidating. So let's get that going right away! By using the free tier of vercel, we can easily publish a web service in minutes.
 
 #### What will you need?

 - A [github](https://github.com/signup) account
 - A [vercel](https://vercel.com/signup) account

 If you don't have these, click on the links above and go ahead and create the accounts. It will probably take you a couple of minutes for each!

 #### Create your git repository

 Navigate to your [github](https://github.com) account and click on the `New` button in the repository section on the page, to create a new repository. 

Enter your app's name as the repository name i.e. `learning-platform-phase1`

And click `Create Repository`
