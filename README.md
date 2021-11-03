# Git workflow

## Rule

## Main workflow

1. Rule

   1.1 Only accept merge request from <code>release</code> and <code>hotfix</code>
   
2. "Traditional" Gitflow workflow

   2.1 Create <code>main</code> (create new repository)

## Feature workflow

1. Rule

   1.1 Each new feature branch only contain one feature.


   1.2 Branch <code>feature/branch</code> only checkout from <code>develop</code>.


   1.3 Resolve conflict before create new pull request into <code>develop</code>.


   1.4 Only accept create new Pull Request into <code>develop</code>.
2. "Traditional" Gitflow workflow


   2.1 Create branch <code>feature/branch</code> from <code>develop</code>.


   2.2 Commit to <code>feature/branch</code>.


   2.3 Create new pull request <code>feature/branch</code> into <code>develop</code>.

## Bugfix workflow

1. Rule

   1.1 Each new bugfix branch only fix one feature.

   1.2 Branch <code>bugfix/branch</code> only checkout from <code>develop</code>.

   1.3 Resolve conflict before create new pull request into <code>develop</code>.

   1.4 Only accept create new Pull Request into <code>develop</code>.

2. Gitflow Workflow

   2.1 Create branch <code>bugfix/branch</code> from <code>develop</code>.

   2.2 Commit to <code>bugfix/branch</code>.

   2.3 Create new pull request <code>bugfix/branch</code> into <code>develop</code>.

## Release Workflow

1. Rule


   1.1 Archive history of official releases. On the release branch we will add tags for each version release like v0.1 , v0.2 .


   1.2 Release branch only checkout from <code>develop</code>.


   1.3 The release branch represents a complete feature set.

2. “Traditional" Gitflow workflow


   2.1 Create <code>release</code> branch from <code>develop</code> branch.


   2.2 Commit to <code>release</code> branch.


   2.3 Create a pull request from <code>release</code> branch to <code>main</code>.



## Hotfix Workflow

1. Rule


   1.1 <code>hotfix</code> branch only checkout from <code>main</code>.


   1.2 Once complete changes will be merged into <code>main</code> and <code>develop</code> (or current release branch if applicable) and tag version mark on <code>main</code>.


2. "Traditional" Gitflow workflow


   2.1 Create branch <code>hotfix/branch-name</code> from <code>main</code>.


   2.2 Commit into <code>hotfix/branch-name</code>.


   2.3 Create new pull request <code>hotfix/branch-name</code> into <code>main</code> and <code>develop</code> (or current release branch if applicable).


   2.4 Tag version mark on <code>main</code>.

# Git conventions

## 1) Git commit convention


Git commit convention follow structures here:


_<< type >>[optional scope]: <description>_


   
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

- <code>main</code>
   
   
- <code>develop</code>
   
   
- <code>release</code>
   
   
- <code>hotfix</code>
   
   
- <code>bugfix</code>

### Convention

*branch/taskid-branch-name
   
*use hyphen as a separator.
Ex: feature/Intern-123-add-new-student
