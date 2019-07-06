Paper is a minimal Jekyll theme. Perfect for hosting your personal site, blog, or portfolio on GitHub or self-hosting on your own server. The styling is purposely minimalistic so that you can add your own flare to the website.

## Features
- Compatible with Jekyll 3.x and **Github Pages**
- Live local reloading for faster development
- **Responsive layout** built-in
- Supports Jekyll's built-in Sass/SCSS preprocessor
- Supports **Google Analytics**
- Supports **Disqus** for commenting
- Minimum Dependencies
- Rakefile for automation
    - `rake check`    - Check links/html files of the generated site
    - `rake clean`    - Clean up generated site
    - `rake post`     - Begin a new post in `./_posts`
    - `rake preview`  - Preview with livereload on local machine

### Customization
To customize various details - title/description of the website, your SNS accout names, etc - edit the `_config.yml` file. 

### Adding posts
```
rake post title="A Title" [date="2012-02-09"] [tags=[tag1,tag2]] [category="category"]
```
This will create a markdown file in the default folder where all posts are stored in Jekyll; `_post`.

If you wish to **change the directory where posts are saved**, go to the `Rakefile` and edit the `CONFIG = { 'posts': CUSTOM_PATH_HERE }`. This will allow `rake post` to know where to save the new posts to.

The **drafts** you are working on can be saved in the `_drafts` directory. When you push your code to the server, files in this directory will NOT be included to the list of posts.

# License

Please see [LICENSE](./LICENSE)

