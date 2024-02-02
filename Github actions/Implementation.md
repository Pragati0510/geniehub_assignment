## Making a CI/CD pipeline using github actions

## first go to repository and then go in .github and make workflows directory and inside that durectory make .yml file

![image](https://github.com/Pragati0510/geniehub_assignment/assets/92318379/67934041-ae56-4c8b-8e88-07a4e8c17203)

## or else you can also go to actions and create a new workflow github will automatically make you a .yml file where you can write your code
![image](https://github.com/Pragati0510/geniehub_assignment/assets/92318379/00285109-d6c7-414a-9f82-a2eebc851f6f)

## then write your CI/CD code in your .yml file 

![image](https://github.com/Pragati0510/geniehub_assignment/assets/92318379/8265dd65-f376-4770-ac92-84dd5d228898)
## the code will depends on where you files are located also on you tech stack.
```
console
name: CI/CD for React App

on:
  push:
    branches:
      - master # Change this to your main branch name

jobs:
  build:
    runs-on: ubuntu-latest

    steps:
      - name: Checkout code
        uses: actions/checkout@v2
   
        
      - name: Setup Node.js
        uses: actions/setup-node@v2
        with:
          node-version: '16'  # Adjust the Node.js version as needed
      - name: remove cache
        run: npm cache clean --force

      - name: Install dependencies
        run: npm install



      - name: Build
        run: npm run build

      - name: Deploy to GitHub Pages
        uses: JamesIves/github-pages-deploy-action@4.1.0
        with:
          branch: gh-pages
          folder: public
```

## then commit changes, code will changes according to tech stack 
## the changes will appear in actions

![image](https://github.com/Pragati0510/geniehub_assignment/assets/92318379/af10d168-83a4-467f-9c1f-7083b052549c)

## having a green tick means your pipeline has been successfully build,you will having something like this

![image](https://github.com/Pragati0510/geniehub_assignment/assets/92318379/83588e47-e089-423a-805a-7447f3ad3442)
![image](https://github.com/Pragati0510/geniehub_assignment/assets/92318379/956f227d-a9c1-4082-9c64-17fed62144f4)
![image](https://github.com/Pragati0510/geniehub_assignment/assets/92318379/4046dc76-39b7-4269-ba5f-7d57f492d21f)
![image](https://github.com/Pragati0510/geniehub_assignment/assets/92318379/ea2ec921-1e77-43a0-9bd1-d7413f36bd56)

# also to deploy your application you will have to go to pages and then choose deploy from branch and choose branch as gh-pages and then save

#then you have to go to package.json and have to paste your url as homepage there

```
console

"homepage" : "your_url"
```
## now you CI/CD pipeline using github actions has been built successfully and when you push anything it will automatically go through the stages and deployed successfully.

## For reference
![image](https://github.com/Pragati0510/geniehub_assignment/assets/92318379/db92f1c6-4529-4fdc-8115-71130fb805ca)


## like i have updated package.json automatically it has gone through process




