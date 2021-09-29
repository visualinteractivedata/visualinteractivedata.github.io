# Website of the Visual+Interactive Data group at the University of Edinburgh

[visualinteractivedata.github.io](https://visualinteractivedata.github.io/)

## Adding new publications

-   The publications page is located at [visualinteractivedata.github.io/publications](https://visualinteractivedata.github.io/publications).
-   To add a new publication, please follow the instructions in the [Google Sheet](https://docs.google.com/spreadsheets/d/1r_9by7qJYC7DSvtqsNnaNqEeZ2MYKUJj7jMEiL5-7YA/edit#gid=0) located in the `vishub group/website` folder.
-   DO NOT edit the csv directly. **Your changes will be overwritten** as soon as the next person uses the Google Sheet to update the list.

## Adding people

To add a new group member, edit the [`_data/people.json`](_data/people.json) file.

To add a masters student or alumnus, edit the [`people.md`](./people.md) file.

## Adding a project

To add a new project page, create a new `.md` file in [`_projects/](./_projects).

You can also edit [`_config.yml`](./_config.yml) to set the order in which projects are listed on the homepage; projects without a specified position will appear at the end of the list.

## How to work on this site locally

-   Make sure you have [Ruby and Jekyll installed](https://jekyllrb.com/docs/installation/)
-   Clone this repo to your computer
-   Open a command line in that folder, run "bundle update" then "bundle exec jekyll serve"
-   The website should now be available at localhost:4000

_This works on my (Sarah's) Windows setup - cannot vouch for anything else, but this is the general principle of running Jekyll sites locally_

Alternatively, you can run Jekyll inside docker using:

    docker run -v $(pwd):/srv/jekyll -it jekyll/builder jekyll build
