# Build Github Pages from Notion content.

Based on `timovv/notion-website-template`

Automated build a website from Notion content, using Loconotion, and deploy into GitHub Pages.

### configuration

1. Create a Notion page to be your website. Must be a single home page, but can have subpages, databases, anything supported by [Loconotion](https://github.com/leoncvlt/loconotion).

1. Share your Notion page **publicly**:   
go to your Notion project, find the page you want to share, press the `share` button and copy the link. In my case, `https://mangrove-kumquat-e2f.notion.site/M-sica-b0a1a76be739495798fea6e8f11c2ce4`

4. update `site.toml` in your repo to point to it.

5. Run the `Publish Notion website to GitHub Pages` action under the Actions tab of your repo.

6. Update your repo's `Pages` settings to use the `gh-pages` branch, hit save, and voila!

`site.toml` can be updated to use any of the settings specified in the [Loconotion README](https://github.com/leoncvlt/loconotion/blob/master/README.md).

### execution

To resync the website, simply run the GitHub action again. 

Or right from the command line, with  `gh --repo palbcn/notion-website workflow run main.yml`

