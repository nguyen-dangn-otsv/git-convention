# Git workflow

## Rule

## Main workflow

1.Rule
1.1 Only accept merge request from release and hotfix
2."Traditional" Gitflow workflow
2.1 Create main (create new repository)

## Feature workflow

1. Rule
   1.1 Each new feature branch only contain one feature.
   1.2 Branch feature/branch only checkout from develop.
   1.3 Resolve conflict before create new pull request into develop.
   1.4 Only accept create new Pull Request into develop.
2. "Traditional" Gitflow workflow
   2.1 Create branch feature/branch from develop.
   2.2 Commit to feature/branch.
   2.3 Create new pull request feature/branch into develop

## Bugfix workflow

1. Rule

   1.1 Each new bugfix branch only fix one feature.

   1.2 Branch bugfix/branch only checkout from develop.

   1.3 Resolve conflict before create new pull request into develop.

   1.4 Only accept create new Pull Request into developer.

2. Gitflow Workflow

   2.1 Create branch bugfix/branch from develop.

   2.2 Commit to bugfix/branch.

   2.3 Create new pull request bugfix/branch into develop

## Release Workflow

1. Rule
   1.1 Archive history of official releases. On the release branch we will add tags for each version release like v0.1 , v0.2 .
   1.2 Release branch only checkout from develop
   1.3 The release branch represents a complete feature set

2. “Traditional" Gitflow workflow
   2.1 Create release branch from develop branch  
   2.2 Commit to release branch
   2.3 Create a pull request from release branch to main

## Hotfix Workflow

1. Rule
   1.1 hotfix branch only checkout from main
   1.2 Once complete changes will be merged into main and develop (or current release branch if applicable) and tag version mark on main
2. "Traditional" Gitflow workflow
   2.1 Create branch hotfix/branch-name from main
   2.2 Commit into hotfix/branch-name
   2.3 Create new pull request hotfix/branch-name into main and develop (or current release branch if applicable)
   2.4 Tag version mark on main

# Git conventions

## 1) Git commit convention

Git commit convention follow structures here:

_<type>[optional scope]: <description>_

<type>:
\_build: Build related changes (eg: npm related/ adding external dependencies)
\_chore: A code change that external user won't see (eg: change to .gitignore file or .prettierrc file)
\_feat: A new feature
\_fix: A bug fix
\_docs: Documentation related changes
\_refactor: A code that neither fix bug nor adds a feature. (eg: You can use this when there is semantic changes like renaming a variable/ function name)
\_perf: A code that improves performance
\_style: A code that is related to styling
\_test: Adding new test or making changes to existing test

## 2) Git branch naming convention

### Branch

- Main
- Develop
- Release
- Hotfix
- Bugfix

### Convention

*branch/taskid-branch-name
*use hyphen as a separator.
Ex: feature/Intern-123-add-new-student
