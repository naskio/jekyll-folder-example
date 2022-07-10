# jekyll-folder-example

Jekyll example where we use a folder `Docs/` for hosting the website.

# Steps

1. refactoring
    - Rename `assets` folder to `static`
    - Put all markdown files in `Docs/content`

2. Generate Jekyll site
   ```shell
   cd Docs/
   jekyll new --skip-bundle .
   ```
3. Add dependencies to Gemfile
4. Install dependencies
   ```shell
   bundle install
   ```
5. Config Jekyll site `_config.yml` and `_config.development.yml`

6. Run
   ```shell
   jekyll serve --config _config.yml,_config.development.yml
   ```
7. Use Collections
