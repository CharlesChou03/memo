# memo
* use a personal access token to push code
  1. go to https://github.com/settings/profile and click [Developer settings] in the bottom left
  2. in this page https://github.com/settings/apps and then click [Personal access tokens], and then click [Generate new token]
  3. copy the PAT token, and back to terminal
  
  ```
    git remote -v
    origin	https://github.com/{USER_NAME}/{REPO_NAME} (fetch)
    origin	https://github.com/{USER_NAME}/{REPO_NAME} (push)
  ```
  ```
    git remote set-url origin https://{USER_NAME}:{PAT_TOKEN}@github.com/{USER_NAME}/{REPO_NAME}
  ```
  ```
    git remote -v
    origin	https://{USER_NAME}:{PAT_TOKEN}@github.com/{USER_NAME}/{REPO_NAME} (fetch)
    origin	https://{USER_NAME}:{PAT_TOKEN}@github.com/{USER_NAME}/{REPO_NAME} (push)
  ```
