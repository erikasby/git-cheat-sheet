## Sync forked repository

#### Add the remote, call it "upstream":
1. `git remote add upstream https://github.com/whoever/whatever.git`

#### Fetch all the branches of that remote into remote-tracking branches
2. `git fetch upstream`

#### Make sure that you're on your master branch:
3. `git checkout main`

#### Rewrite your master branch so that any commits of yours that aren't already in upstream/master are replayed on top of that other branch:
4. `git rebase upstream/main`

## Merge development branch with main

#### On branch development
1. `git merge main`

#### Resolve any merge conflicts if there are any
2. `git checkout main`

#### There won't be any conflicts now
3. `git merge development`