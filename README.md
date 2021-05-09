# www.lindsaymoynihan.com

## initial setup

- create a new public repository named `www.lindsaymoynihan.com`
- go to https://github.com/lindsaymoynihan/www.lindsaymoynihan.com/settings and configure the new repo
- `mkdir www.lindsaymoynihan.com`
- `cd www.lindsaymoynihan.com`
- `git init`
- `git config user.name lindsaymoynihan`
- `git config user.email 'lindsaymoynihan@users.noreply.github.com'`
- `git config pull.ff only`
- `git add -A`
- `git commit -m 'first commit'`
- `git branch -M main`
- `git remote add origin https://github.com/lindsaymoynihan/www.lindsaymoynihan.com.git`
- `git switch --orphan gh-pages`
- `git commit --allow-empty --allow-empty-message`
- `git push -u origin gh-pages`
- `git switch main`
- `git push -u origin main`
- go to https://github.com/lindsaymoynihan/www.lindsaymoynihan.com/settings/branches and set main as the default branch

## dev notes

bundle install;

cd www;

JEKYLL_ENV=development bundle exec jekyll serve --host 0.0.0.0;

or

JEKYLL_ENV=production bundle exec jekyll build;

for example:

cd /path-to/lindsaymoynihan.com/www/ && git pull && bundle install && JEKYLL_ENV=production bundle exec jekyll build
