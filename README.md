# CVAS Github Page

This is the repository that contains source code for the all of the CVAS papers

## Runing locally

Run `bundle install`
Run `run.sh`

## Running locally on Ubuntu 20 and before

```bash
curl -fsSL https://github.com/rbenv/rbenv-installer/raw/HEAD/bin/rbenv-installer | bash

echo 'export PATH="$HOME/.rbenv/bin:$PATH"' >> ~/.zshrc
echo 'eval "$(rbenv init -)"' >> ~/.zshrc
source ~/.zshrc

rbenv install 3.2.5

rbenv global 3.2.5

gem install jekyll bundler
```

## Creating a new Paper

- Create a copy of `new_paper.html` at the root of the repo.
- Update the information in the front matter (Only the youtube id is needed. Not the full URL)
- Create folders using the permalink name of the page in `static/images` to store paper related files
- Add the information concerning the paper in `_data/authors.yaml` and `_data/papers.yaml`
- Create a `thumbnail.png` images in the paper folder
- Copy the layout from a previous paper and update accordingly
