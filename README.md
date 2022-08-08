# jekyll-folder-example

Jekyll example where we use a folder `docs/` for hosting the website.

# Steps

1. refactoring
    - add `assets/` folder into `docs/`
    - Put all markdown files in `docs/_docs/`

2. Generate Jekyll site
   ```shell
   cd docs/
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

> Folder should be named `docs` all lowercase.

## Data Generation

```shell
brew install yq
curl https://api.github.com/repos/m4rs-mt/ILGPU/releases | yq -P > Desktop/jekyll-folder-example/docs/_data/releases.yml
curl https://api.github.com/repos/m4rs-mt/ILGPU/milestones | yq -P > Desktop/jekyll-folder-example/docs/_data/milestones.yml
```
