# Website of the Visual+Interactive Data group at the University of Edinburgh

[visualinteractivedata.github.io](https://visualinteractivedata.github.io/)

## Adding new publications

- The publications page is located at [visualinteractivedata.github.io/publications](https://visualinteractivedata.github.io/publications).
- To add a new publication, please follow the instructions in the [Google Sheet](https://docs.google.com/spreadsheets/d/1r_9by7qJYC7DSvtqsNnaNqEeZ2MYKUJj7jMEiL5-7YA/edit#gid=0) located in the `vishub group/website` folder.
- DO NOT edit the csv directly. **Your changes will be overwritten** as soon as the next person uses the Google Sheet to update the list.

## Adding people

To add a new group member, edit the [`_data/people.json`](_data/people.json) file.

To add a masters student or alumnus, edit the [`people.md`](./people.md) file.

## Adding a project

To add a new project page, create a new `.md` file in [`\_projects/](./_projects).

You can also edit [`_config.yml`](./_config.yml) to set the order in which projects are listed on the homepage; projects without a specified position will appear at the end of the list.

## Adding new pages

To add a new page, simply create a new `.md` (Markdown) file. The structure of the website generally mirrors the folder structure in the repo. For example, if you create a new file at `resources/newpage.md`, the link to that page on the website will be `vishub.net/resources/newpage`.

If you want the page to have a URL different from this, you can manually set a permalink. To do this, add the permalink tag to the frontmatter (the header enclosed by `---`) of the page. The markdown file should start like this:

```yaml
---
permalink: custom_newpage
---
```

This would make the link on the website `vishub.net/custom_newpage`.

Permalinks have been used in the `resources` and `jobs` folders to preserve the URL of pages that were initially created in the root of the page and later moved into the folder.

## Main navigation

To edit the main navigation, edit the html in the default layout at [`_layouts/default.html`](_layouts/default.html).

## How to work on this site locally

- Make sure you have [Ruby and Jekyll installed](https://jekyllrb.com/docs/installation/)
- Clone this repo to your computer
- Open a command line in that folder, run `bundle update` then `bundle exec jekyll serve`
- The website should now be available at `localhost:4000`

Alternatively, you can run Jekyll inside docker using:

    docker run -v $(pwd):/srv/jekyll -it jekyll/builder jekyll build
