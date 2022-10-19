# tdei-docs

## Local development setup

### 1. Prequisites

To run this application, Hugo needs to be installed in system. To install Hugo based on the OS please do the following

For macOS and Linux, install hugo with *brew*

```
brew install hugo

```

For windows OS install with chocolatey.

```
choco install brew
```

To install chocolatey on window you can refer the following link [install choco](https://chocolatey.org/install)


### 2. Running application

After cloning the application, open terminal the application folder and the run the following command.

```
hugo serve

```

This will start the application and can check on localhost:1313 in the browser. For every changes done in the application, they are immediately updated.

Before starting the development, make sure you change the baseURL to empty string in **config.toml** file and do not commit this change to git. This is only for local development.

```
baseURL=""
```


### 3. How to add new markdown files to the application


- **How to add a markdown file**

To add a new markdown to the application, go to the **content** and create a new markdown file in any of the categories. The name of the file should match with page title in **sidebar.yml** file and with snake-case format. Example if the title is "CSS Variables" and the title should be "css-variables.md". Make sure you add the following template on the top of the markdown file

```
---
title: "<title>"
date: 2022-10-13T12:06:23+02:00
group: "<group name>"
draft: false
toc: true
---
```

title name should match the page title in **sidebar.yml** file which is in **data** folder. Group names should follow the snake case and match title as in **sidebar.yml** file

- **Adding a new category**

To add a new category, go to  **sidebar.yml** file which is in **data** folder use the following template to add a new category.

```
- title: Getting started
  icon: book-half
  icon_color: indigo
  pages:
    - title: Introduction
```

Replace the title names with new category names and markdown files names.


## Deployment

Currently, this application is deployed using **github workflow**. Every change to this repository triggers this workflow and application will be deployed with new changes




