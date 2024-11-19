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

## Updating news

To update the news displayed on the homepage, edit the [`news.md`](news.md) file. Add new items at the top of the list, since they are displayed in the order shown in the file.

The homepage shows all items until the `<!-- more news -->` line in between the bullet points. Move this line to where you want the news on the homepage to cut off. The cut off older news will still be available when following the 'More news...' link.

## Adding new pages & permalinks

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

## GitHub Actions

The site is automatically rebuilt using GitHub Actions when a commit is pushed to the `master` branch. There is one exception: it does not rebuild the page when only `README.md` (this file) is edited. The GitHub Actions workflow is located at [`.github/workflows`](.github/workflows).

If the workflow fails (for example because of formatting issues in the newly committed code), a red X will be displayed next to the commit and there may be warning emails to the repository owners. However, an unsuccessful build will not make the website go offline, GitHub will just continue serving the most recent successful build. Any updates will only go online once a successful build has happened, i.e., once the issues that caused the build to fail have been resolved.

## How to work on this site locally

Small to medium content changes that only concern one or a few files can easily be done on the GitHub website. For bigger changes involving many files, potentially broken links, and new features, it is better to test these locally first.

- Make sure you have [Ruby and Jekyll installed](https://jekyllrb.com/docs/installation/)
- Clone this repo to your computer
- Open a command line in that folder, run `bundle update` then `bundle exec jekyll serve`
- The website should now be available at `localhost:4000`

Alternatively, you can run Jekyll inside docker using:

    docker run -v $(pwd):/srv/jekyll -it jekyll/builder jekyll build
