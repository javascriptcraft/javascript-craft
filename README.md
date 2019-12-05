

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


## Setting up your fork

#### To get this project up and running on your computer perform the following:

```Bash
Fork the repository by clicking "fork" in the upper right of the reposity page on github

Create a local clone of the forked repository
 >> git clone https://github.com/YOUR_USERNAME/javascript-craft.git

 Go to the project root directory
 >> cd javascript-craft

 Configure Git to sync your fork with the original repository
 >> git remote add upstream https://github.com/javascriptcraft/javascript-craft.git
 Install  your dependencies
 >> yarn install
 
 Start the app in http://localhost:3000
 >> yarn start
```


#### Submiting PR's

```Bash
# TODO
```

Front End will be built in `ReactJS` with Typescript. But since each component will have examples in `Vanilla JavaScript`, `ReactJS`, `VueJS`  and `AngularJS`, you can still contribute and learn no matter what stack will be.  
Backend technologies are expected to be `NodeJs`, `ExpressJS`, `MangoDB` and `GraphQL`


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
