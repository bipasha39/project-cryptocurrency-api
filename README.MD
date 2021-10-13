## Project Cryptocurrency-Api

### The goal of this project is to create a cryptocurrency finance price tracker app with React.We will use React Hook(mainly use useEffect and useState) and Axios(Optional) for this project. 

**Basic functionality:** You will be able to search currencies and have it display on the browser. Also, the prices will be updated live whenever you refresh the page. We will get all of the data from a public API. .

A simple example looks like this:  

<img src="SampleImage.png" width="550" /> 

---

### For more advanced students

1. Create a new project on your local computer using `npx create-react-app project-cryptocurrency'
1. Delete the css from the App.css and index.css files and use `index.css` for your css (look at your previous projects how you set the initial general CSS)
1. Delete the code in the App.js file between `<div className="App">` and the closing `</div>`
1. Create a `components` folder inside your `src` folder
1. Create a functional component Coin inside this file (remember the React syntax!) and a `css ` file in same name.
1. In the `return` of the component, add `<h1>Search Currency</h1>` to test the component
1. To test if your React app is working, make sure you are in the project folder in your terminal and type `npm start` (you should see the text "Search Currency?" as title on the page)

### For Fetching API

1. Use `Use effect` to fetch the data from the API
```js
fetch("https://api.coingecko.com/api/v3/coins/markets?vs_currency=USD&order=market_cap_desc&per_page=100&page=1&sparkline=false")
```

1. Create a search input that will help you to find currency by there name.
1. Create a `div` with class name `image-container`.
1. Create a `handleClick()` function that uses the `setImage` hook (you can test if this works by doing a console.log)
1. Now this can be difficult: you have to create a path to the images that changes when you click the button! You can use a **template literal** for this. In the `image-container` div, add `<img>` with `src={}` and inside the curly brackets add a template literal that holds the path to the images in your project's public/images folder (hint: you already have the variable `image` ...)
1. Add CSS to style the page as you like (the color used for the title and the search input 
1. 

1. **If you would like to build this app more interactive** and add more column, you can add more information using the same api.   


## Please note:
If you want to download a project on your local machine, do not fork it but clone the repo locally, on your computer. After that, create a new repo in your own GitHub account *with exactly the same project name*, and link the local repo to the remote repo in your GitHub account (see below). Why should you clone and not fork? It will show the project as **your own project** and not a fork of someone else's project. You can use it as a project for your portfolio.

You can connect a local project to a new, empty GitHub repo [as follows](https://docs.github.com/en/github/importing-your-projects-to-github/adding-an-existing-project-to-github-using-the-command-line). We can do this together during a CodeWomen coding session: it is very good to know this so that you can start a project locally and afterwards link it with a remote GitHub repo.

If you clone the project without forking it, you will have to change the 'remote origin' repository after cloning. Check the remote of your local project using `git remote -v`. You will probably see:  
`origin  https://github.com/CodeWomen-Barcelona/some-codewomen-project.git (fetch)`  
`origin  https://github.com/CodeWomen-Barcelona/some-codewomen-project.git (push)`

To link your local project to your own GitHub repo, you need to change the remote origin. Have a look at this article: https://devconnected.com/how-to-change-git-remote-origin/. With `git remote -v` you can again check if remote origin has been reset and now shows the name of your GitHub account.


PS: if you work for a company that has a corporate social responsibility policy and wants to support women in tech, then here is the link to the [fundraising overview of MigraCode](https://docs.google.com/spreadsheets/d/1Zs-Mmi39bcjVw2U-iEQWSHSjkb-EmET-j1WB2oJF45Q/edit#gid=0).

---
