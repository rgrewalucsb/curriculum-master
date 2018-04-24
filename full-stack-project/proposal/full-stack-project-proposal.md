# Fullstack Project Setup

## Phase 1: Create the Repo

1. Create a new Rails project with the following flags
  - `--skip-turbolinks=true`
  - `--database=postgresql`
2. The rails skeleton includes a .gitignore file. In addition to what is
  already there, add the following:

```
// .gitignore

// ... a bunch of preloaded ignores

// To add:
node_modules/
bundle.js
bundle.js.map
.byebug_history
.DS_Store
npm-debug.log
```

3. Create a new repo and give it a good name.

![Screenshot: naming repo][name_repo]

4. Commit your files and push to your remote.

## Phase 2: Create Your Design Document Files

Your fullstack project design docs are a documentation of your planning
process in the form of a Github Wiki. Look [here](./) for an explanation
of each of the design docs below.

Also, see the [sample design docs][sample].

In your new fullstack repo, create a wiki.

![Screenshot: create wiki][create_wiki]

Create these pages:

* MVP List
* Database Schema
* Routes
* Sample State
* Component Hierarchy with Wireframes

On the home page, create links to each of these pages.

Make sure to use the layout menu to give the appropriate styling to your
documents (e.g. code should be in code blocks). Your project advisor will
review your design docs and give you feedback on any major issues.

![Screenshot: add page in wiki][design-docs-wiki]

## Phase 3: Complete Your Design Docs

Go back over all of the design docs you did for homework and make any
necessary changes. Also complete any of the above docs that were not
completed for homework.

Lastly, add your project advisor as a collaborator to your repo. To do
this, go the 'Settings' tab, and click 'Collaborators'.

![Add Collaborators][add_project_manager]

[sample]: https://www.github.com/appacademy/bluebird/wiki

## Phase 4: During the Project

To see what you'll be doing during the project, take a look at
[these instructions](../project/during-the-project.md)

[create_new_repo]: ./assets/create_new_repo.png
[name_repo]: ./assets/name_repo.png
[copy_git_url]: assets/copy_git_url.png

[add_project_manager]: assets/add_project_manager.png

[create_wiki]: assets/create_wiki.png
[design-docs-wiki]: assets/proposal_wiki.png

[issues]: assets/issues.png

[labels]: assets/labels.png
