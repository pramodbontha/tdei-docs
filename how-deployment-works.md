# Deployment workflow

![tdei-docs workflow](https://user-images.githubusercontent.com/58882551/196048920-404c3be9-d0bd-4231-9c5d-bb73738a564a.png)

1. **Creating or Regenerating docs**
After making the local development changes and changes are looking fine in the local server. Run the command *hugo* in the terminal. This will create a build content, which are static html files converted from markdown files by hugo.

2. **Commit and Push to github repo**
Once the docs folder content is updated from the above step, commit and push the docs folder content to github repo.

3. **github-pages bot workflow job-1**
The pushed changes will trigger the gihub pages bot workflows. Initially, it will copy the content from *docs* folder to *gh-pages* branch. From here other jobs with process the content.

3. **github-pages bot workflow job-2**
The content is build and deployed by github-pages workflow *"pages build and deployment"* which uses in built jekyll builder for static sites build and deployment from github.
