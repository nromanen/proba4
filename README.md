1. Add user `softservedata` to this repository.

2. Create branch `develop` as default branch.


3. Protect branches main and develop with these rules:
- user can't merge to both branches without pull request,
- allowed to merge to develop branch only if we have 2 approvals
- merge to main branch allowed if only owner or user online-marathon approved PR
4. Add template (pull_request_template.md) to .github directory for creating issue in format:

## Describe your changes

## Issue ticket number and link

## Checklist before requesting a review
- [ ] I have performed a self-review of my code
- [ ] If it is a core feature, I have added thorough tests.
- [ ] Do we need to implement analytics?
- [ ] Will this be part of a product update? If yes, please write one phrase about this update.

5. Create project for this repository.

6. Add deploy keys to your repository.

7. Create discord server and add notification when PR was created.

8. For github actions: 
- create PAT (Personal Access Token) with Full control of private repositories and Full control of orgs and teams, read and write org projects
- add repository secret with key (name) URL and the value in format USERNAME/REPOSITORY_NAME 
- add repository secret key key TOKEN and the value of PAT
