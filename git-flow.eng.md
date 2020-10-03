# GIT FLOW

git flow init - init a repo using gitflow
git flow feature start <feature_name> - create a branch of feature with the chosen name
git flow feature publish - pushes features on git
git flow feature finish <feature_name> - merge the feature branch into the development branch
git flow release start <version_number> - create a new release based on the development branch
git flow release finish <version_number> - the launch branch will be merged into the main branch and the development branch, and then the launch branch will be deleted