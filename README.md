# week-9-challenge
README Generator

##Description

This is a command-line application that runs with Node.js that dynamically generates a README.md file from a user's input using the Inquirer package. 

You can use this application to generate a professional README file to be used in your GitHub projects.

##Installation

Steps required to install project and how to get the development environment running: 
To generate your own README, first run npm install in order to install the following npm pacakge dependencies as specified in the package.json: 
- inquirer that will prompt you for your inputs from the command line
- axios to fetch your info from the GitHub API 
The application itself can be invoked with node index.js . 

##Usage

![Gif demo of README-generator](readme-demo.gif)

When you run node index.js, the application uses the inquirer package to prompt you in the command line with a series of questions about your GitHub and about your project. 
The application then takes your responses and uses axios to fetch your GitHub profile from the GitHub API, including your GitHub email. From there, the application will generate markdown and a table of contents for README conditionally based on your responses to the Inquirer prompts (so, if you don't answer the optional questions, such as Installation, an Installation section will not be included in your README).
Finally, fs.writeFile is used to generate your project's README.md file. Check out the ExampleREADME.md in this repo as an example.

##Methodology

The application utilizes modularization by separating the GitHub API call and generation of the markdown into separate modules: api.js and generateMarkdown.js, respectively, inside the utils folder. 

The application also utilizes, as much as possible, syntax and paradigms, including arrow functions, const, let, template literals, and async/await to handle the inquirer, axios and fs.writeFile promises. 

##License

MIT License

##Questions? 

If you have any questions about the project, contact me at: basnyat.ojashri@gmail.com 

Check out rest of my work on GitHub via: [Ojashri-Basnyat] (https://github.com/Ojashri-Basnyat)






