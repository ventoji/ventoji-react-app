# ventoji-react-app
Deploying an react app

This an example of how to deploy a react app. In order to do that, follow the steps below:

1. Add to package.json: "homepage":"https://yourusername.github.io/repository-name", in this case https://ventoji.github.io/ventoji-react-app.
2. Installl gh-pages package running the command: yarn add gh-pages --dev or npm install --save gh-pages.
3. In case you do not have the github repository, create one and name it (ventoji-react-app for this case).
4. Execute on the current local directory: git remote add origin https://github.com/ventoji/ventoji-react-app.git. 
    note: (git remote add origin https://github.com/yourusername/repository-name.git).
5. Add deploy commands to package.json: 
  "scripts":{
    "predeploy": "npm run build",
    "deploy": "gh-pages -d build",
   }
6. Execute deploy commands: npm run deploy or yarn deploy.
7. You can check on GitHub Pages settings that the source is set to gh-pages branch.
8. You should see your app lives on https://yourusername.github.io/repository-name/ (https://ventoji.github.io/ventoji-react-app/).
