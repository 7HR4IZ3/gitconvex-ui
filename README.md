# gitconvex react project
This is the front end react source for the [gitconvex](https://github.com/neel1996/gitconvex) project.

![gitconvex-react](https://user-images.githubusercontent.com/47709856/87220396-e72df380-c380-11ea-9b2b-e156402842bb.png)

## Dependencies

The depedency packages used by this project can be found [here](https://github.com/neel1996/gitconvex-ui/network/dependencies)

- **Styling** - For styling, the project used [tailwind]() css framework 
- **Syntax Highlighting** - [prismjs](https://github.com/PrismJS/prism) is used for syntax highlighting within the *Git Difference* section
- **Icon set** - [FontAweomse for react](https://github.com/FortAwesome/Font-Awesome)

## Contribute!

If you are interested in contributing to the project, fork the repo, submit a PR. Currently its just a single dev working on the project. Hopefully will get couple more on board to maintain the repo

### Guidelines 

Fork the repo and raise a new Pull Request to merge your branch with the `development` branch of this repo. Once the review is complete, the PR will be approved and merged with `master`

### Setup

After cloning the repo, follow the steps mentioned below to setup the react app,

- **Installing dependencies**

```
$ cd gitconvex-ui
$ npm install
```

- **Building the css file**

The project uses `tailwindcss` for styling all the elements, so it is mandatory to build the CSS file which is not included in the git tree. Follow the steps to build the css file

```

$ cd gitconvex-ui
$ npm install --global tailwindcss 

$ npm run build:tailwind

## This will generate a default tailwind css bundle

```

- **Starting the app**

After completing the setup process, use `npm start` to start the react app


## Project directory tree

```

├── LICENSE
├── README.md
├── package.json
├── public
│   ├── favicon.ico
│   ├── gitconvex.png
│   ├── index.html
│   ├── logo192.png
│   ├── logo512.png
│   ├── manifest.json
│   ├── prism.css
│   └── robots.txt
└── src
    ├── App.css
    ├── App.js
    ├── Components
    │   ├── DashBoard
    │   │   ├── Dashboard.js
    │   │   ├── DashboardPaneComponents
    │   │   │   ├── LeftPane.js
    │   │   │   └── RightPane.js
    │   │   ├── Help
    │   │   │   └── Help.js
    │   │   ├── Repository
    │   │   │   ├── GitComponents
    │   │   │   │   ├── GitDiffViewComponent.js
    │   │   │   │   ├── GitOperation
    │   │   │   │   │   ├── CommitComponent.js
    │   │   │   │   │   ├── GitOperationComponent.js
    │   │   │   │   │   ├── PushComponent.js
    │   │   │   │   │   └── StageComponent.js
    │   │   │   │   └── GitTrackedComponent.js
    │   │   │   └── RepoComponents
    │   │   │       ├── AddRepoForm.js
    │   │   │       ├── RepoCard.js
    │   │   │       ├── RepoComponent.js
    │   │   │       ├── RepoDetails
    │   │   │       │   ├── FileExplorerComponent.js
    │   │   │       │   ├── RepoDetailBackdrop
    │   │   │       │   │   ├── AddBranchComponent.js
    │   │   │       │   │   ├── AddRemoteRepoComponent.js
    │   │   │       │   │   ├── BranchListComponent.js
    │   │   │       │   │   ├── CommitLogComponent.js
    │   │   │       │   │   ├── CommitLogFileCard.js
    │   │   │       │   │   ├── FetchPullActionComponent.js
    │   │   │       │   │   └── SwitchBranchComponent.js
    │   │   │       │   ├── RepoInfoComponent.js
    │   │   │       │   ├── RepoLeftPaneComponent.js
    │   │   │       │   ├── RepoRightPaneComponent.js
    │   │   │       │   ├── RepositoryDetails.js
    │   │   │       │   ├── TopPaneGridComponent.js
    │   │   │       │   └── backdropActionType.js
    │   │   │       ├── RepositoryAction.js
    │   │   │       └── RepositoryDetails.js
    │   │   └── Settings
    │   │       └── Settings.js
    │   ├── SplashScreen.css
    │   └── SplashScreen.js
    ├── actionStore.js
    ├── assets
    │   └── gitconvex.png
    ├── context.js
    ├── index.js
    ├── logo.svg
    ├── prism.css
    ├── reducer.js
    ├── serviceWorker.js
    ├── setupTests.js
    ├── tests
    │   ├── App.test.js
    │   └── Dashboard.test.js
    └── util
        ├── apiURLSupplier.js
        └── env_config.js

```

