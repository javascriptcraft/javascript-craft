
##  Project Concept

  
##  MVP
We will build a platform where we can keep collection of custom UI elements/components in different categories.

For example in `Select` category, we will have different types of Select components such as `Simple Select`, `Searchable Select`, `Multi-Select`.

Each component will have different options listed below it.

  

- View code

- Open code in editor (either external editor like codepen or our cloud editor)

- Save/Bookmark Component

- Discuss (which will open a discussion page like in guthub issues)

- Upvote/Like

- Component Creator account/ top contributors ??? (TBD)


Front End will be built in `ReactJS` with Typescript. But since each component will have examples in `Vanilla JavaScript`, `ReactJS`, `VueJS`  and `AngularJS`, you can still contribute and learn no matter what stack will be.  
Backend technologies are expected to be `NodeJs`, `ExpressJS`, `MangoDB` and `GraphQL`

## Setting up project
> We use yarn as our package manager

## 1. Clone project
```
git clone https://github.com/javascriptcraft/javascript-craft.git
```

## 2. Install yarn
- Read the [Installation Guide](https://yarnpkg.com/en/docs/install) on website for detailed instructions on how to install Yarn.

  

## 3. Run the app in development mode 
In the project directory, you can run:
```
yarn start
```
  

Runs the app in the development mode.<br  />

Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

  

The page will reload if you make edits.<br  />

You will also see any lint errors in the console.

  

### `yarn test`

  

Launches the test runner in the interactive watch mode.<br  />

See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

  

### `yarn build`

  

Builds the app for production to the `build` folder.<br  />

It correctly bundles React in production mode and optimizes the build for the best performance.


The build is minified and the filenames include the hashes.<br  />

Your app is ready to be deployed!

  

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.


## Learn More

You can learn more in the [Create React App documentation](https://facebook.github.io/create-react-app/docs/getting-started).

  

To learn React, check out the [React documentation](https://reactjs.org/).


## Folder Structure Conventions
============================


### A typical top-level directory layout

    .
    ├── src                     # The main source   
    │   ├── assets              # Static files such as images
    │   ├── components          # Reusable components
    │   ├── constants           # All constant values used in Project
    │   ├── hooks               # Reusable custom hooks
    │   ├── routes              # Containers which includes all Business Logic like data fetching
    │   ├── utils               # Includes helper functions for reusable methods
    │   ├── App.js              # Top level component
    │   ├── index.js            # Entry point
    └── README.md

### Routes for Business Logic

Routes are Each Pages to be shown to users separately.

    .
    ├── routes                        
    │   ├── Home              
    │   │   ├── hooks               # Custom hooks that only be used locally
    │   │   ├── components          # Simple components which only receives props and renders views using data
    │   │   ├── HomeContainer.js    # Containers include all data fetching
    │   │   ├── index.js            # to export component and import in other React components
    │   ├── About          
    │   ├── ...          
    │   └── index.js
    │__ ...


Often it is beneficial to include all related files like `actions` and `components` in each Route container itself, so that if project becomes large, it will be easy to keep all files clean and neat

> **_NOTE:_**
Reusable `hooks` and `components` are kept in `src/hooks` and `sr/components` respectively to reduce repetition (DRY)
