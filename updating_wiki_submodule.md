# Project Wiki as Git Submodule

SEE: [Including a github wiki in a repository as a submodule](https://brendancleary.com/2013/03/08/including-a-github-wiki-in-a-repository-as-a-submodule/)

```
cd docs
# Make your changes and commit as normal (note you are now committing to the submodule repo)
git add deliverables.md
git commit -m "Added deliverables page."

# Now push submodule commits to the remote.
git push

# Now got back to the partent project and do another commit that basically says,
#    "Here is a pointer to the new version of the submodule which is in you."
cd ../
git commit -m "updated wiki."

# Push the changes to the remote
git push
```
