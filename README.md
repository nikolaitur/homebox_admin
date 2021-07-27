# Site Details

## Project info
* Team: 
  * PM: Anya Dikih
  * Lead Designer: Trisha Angeles 
  * Lead Dev: Antonis Mazellari
* Launched (Date)


## Helpful Links
* [Store url](https://tomorrows-laundry.myshopify.com/)
* [Repo](https://starter-theme.myshopify.com/)
* [Asana Board](https://app.asana.com/0/1199692001989694/board)
* [Training Docs]()
* [Test Plans]()


## Built With
* __Slate-v0__  
* __Webpack-4__ 

  

## Dependencies
1. Node version v10.13.0)

## getting Started

### Repo setup
  * Clone project via ssh from git@github.com:ecomdept/starter-theme.git
  * Remove git
  * Initalize git 
  * Update README.md
  * Commit changes
  * Add branch Main
  * Add remote origin
    > Ensure that you can hadle multiple git accounts 
      [reference](https://gist.github.com/Jonalogy/54091c98946cfe4f8cdab2bea79430f9)
      For multiple git accounts please use git remote add origin git@github.com-[username]:ecomdept/[repo-name].git
  * Push changes in github
  
    ```bash
    rm -rf .git
    git init
    git add .
    git commit -m "Initial commit"
    git branch -M main
    git remote add origin git@github.com:ecomdept/[repo-name].git    
    git push -u origin main
    ```
### Theme setup
  * Duplicate live theme in Shopify to use as dev theme
### Local setup
  * Clone project via ssh git@github.com:ecomdept/[repo-name].git
  * Create + checkout new branch  
  * Switch to node v10.13.00
  * Install dependencies with yarn
  * Update `config.yml`
  * Ensure that `settings_data.json` is ingored and will not be overwritten

  ```bash
  git clone git@github.com:ecomdept/[repo-name].git
  cd repo-name  
  nvm use 10.13.00
  yarn install
  ```

### Developing
  * Always perform git pull before you start development
  * Use watch command 

  ```bash
  git pull
  yarn watch
  ```

  * Once you are done for the day please commit your changes and log you hours in Asana ticket

    ```bash
    git add
    git commit -m "Commit message"
    git push    
    ```    

## Running tests QA
*High level things to keep in mind while doing QA and test cases that should be tested before deploy*
*Details should be found in test plan doc in client GDrive Folder [TBD]*


## Deploying
  * Build js and css and deploy files into the dev theme

  ```bash
  yarn build
  yarn deploy
  ```    

  * Commit changes in the branch
  * Merge Main into dev branch
    > Resolve any conflicts
  * Checkout master and merge dev branch into master

    ```bash    
    git checkout main
    git pull
    git checkout branch-name
    git merge main --no-ff -m "Merging Main in the branch"
    git push
    git checkout main
    git merge branch-name --no-ff -m "Merging branch-name in Main"
    git push    
    ```    
  * Merge `settings.json` from live theme
  * Publish theme

---

## __THEME FEATURE__:
* __Base Theme__
  * __Performance__: Code splitting + vendor bundling
  * __Front_End__: Ability to use vue.js
  * __layout__: It is using flexbox and grid helper classes to build layout
    >  `src/styles/base/global/_layout.scss`
  * __Image__: Utilizing lazysizes + lazyloading library
    >  `src/snippets/responsive-img.liquid`
  * __Data__: 
  * __Tags__: 
  * __Metafields__: 
  * __Additional relevant info__: 


*Fill out this information when applicable:*
* __Custom Features__
  * __Using__: 
    ___Rivet-cart.js for Minicart___
  * __Integrations__:
  * __Data__: 
  * __Tags__: 
  * __Metafields__: 
  * __Additional relevant info__: 
### Third Party
* If not mentioned above, what additional third party solutions were integrated to the site, for what feature/template and any brief relevant note*
* [app name] (link) - used for [features / solutions] 
---

## For reference

[Markdown Cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)
