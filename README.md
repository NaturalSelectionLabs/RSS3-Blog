# RSS3-Blog
This is RSS3 blog repository. All edits should be made in files located under `/_app`. 

## Blogs   
Blog posts md files are located under `/_app/_posts`.

### Compose A Blog
1. Add new md file with formatted file name `YYYY-MM-DD-title-of-the-blog.md`.   
2. All post md file must start with the following table in the md file:
    ```
    ---
    layout: post
    title: [put title here]
    author: [put author here]
    ---
    ```

### About Authors
1. Current legible values for `author` are: `joshua`, `diygod`, `anny`, `tu`, `atlas`; if not specified, then it will be `rss3` by default.   
2. New authors can be added in `/_app/_data/authors.yml`; any edit to existing author info also need to be done in this file.

## Template
This blog adapts from the template [Almace Scaffolding](https://github.com/sparanoid/almace-scaffolding).