# Instructions
==============

## Repo setup and Git hub actions setup
--------------
1. Create GH repo
2. Setup `GH_TOKEN` secret for actions to push artifacts to repo
3. Setup github pages as follows and click on save
   1. Source - Deploy from a branch
   2. Branch - main
   3. Folder - /docs 
![gh pages setup](gh_pages.png)
4. Take note of the live site url - usually `https://<repo-owner>.github.io/<gh_repo_name>`
5. Add live site url as environment variable in github action e.g. repo_url

## Adding Helm repo
---------------
1. Add Helm repository - `helm repo add <gh_repo_name> https://<repo-owner>.github.io/<repo_name>`
2. View list of charts in repo - `helm search repo <gh_repo_name>`


# References
==============
1. Helm official site - https://helm.sh/docs/topics/chart_repository/#github-pages-example
2. Example repo - https://github.com/technosophos/tscharts 