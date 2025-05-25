# 🧠 Top 50 Git Commands & Interview Questions for DevOps Engineers

## 🔍 Git Basics

1. **What is Git?**  
   Git is a distributed version control system used to track changes in source code during software development.

2. **What is the difference between Git and GitHub?**  
   Git is a version control tool; GitHub is a platform for hosting Git repositories.

3. **How do you initialize a Git repository?**  
   ```bash
   git init
   ```

4. **How do you clone a repository?**  
   ```bash
   git clone https://github.com/user/repo.git
   ```

5. **What command stages changes for a commit?**  
   ```bash
   git add <file>
   ```

6. **How do you commit staged changes?**  
   ```bash
   git commit -m "Message"
   ```

7. **How do you check the status of your working directory?**  
   ```bash
   git status
   ```

8. **How do you view the commit history?**  
   ```bash
   git log
   ```

9. **How do you see a summarized commit history?**  
   ```bash
   git log --oneline
   ```

10. **How do you check the differences between commits or working tree?**  
    ```bash
    git diff
    ```

## 🔄 Branching & Merging

11. **How do you create a new branch?**  
    ```bash
    git branch new-feature
    ```

12. **How do you switch to another branch?**  
    ```bash
    git checkout new-feature
    ```

13. **How do you create and switch in one step?**  
    ```bash
    git checkout -b new-feature
    ```

14. **How do you list all branches?**  
    ```bash
    git branch
    ```

15. **How do you delete a local branch?**  
    ```bash
    git branch -d branch-name
    ```

16. **How do you merge a branch into current branch?**  
    ```bash
    git merge branch-name
    ```

17. **How do you resolve merge conflicts?**  
    Manually edit files, then:
    ```bash
    git add .
    git commit
    ```

18. **How do you rebase a branch?**  
    ```bash
    git rebase main
    ```

19. **What is the difference between merge and rebase?**  
    Merge preserves history, rebase creates a linear history.

20. **How do you abort a merge or rebase?**  
    ```bash
    git merge --abort
    git rebase --abort
    ```

## 🚀 Remote Repositories

21. **How do you add a remote repository?**  
    ```bash
    git remote add origin URL
    ```

22. **How do you push code to a remote repository?**  
    ```bash
    git push origin branch
    ```

23. **How do you pull latest changes from remote?**  
    ```bash
    git pull
    ```

24. **How do you fetch changes without merging?**  
    ```bash
    git fetch
    ```

25. **How do you view remote URLs?**  
    ```bash
    git remote -v
    ```

26. **How do you remove a remote?**  
    ```bash
    git remote remove origin
    ```

27. **How do you rename a remote?**  
    ```bash
    git remote rename origin upstream
    ```

28. **How do you push all branches?**  
    ```bash
    git push --all
    ```

29. **How do you set a branch to track a remote branch?**  
    ```bash
    git branch -u origin/main
    ```

30. **How do you clone only a specific branch?**  
    ```bash
    git clone -b branch-name --single-branch repo-url
    ```

## 🛠️ Advanced Git Usage

31. **How do you stash changes?**  
    ```bash
    git stash
    ```

32. **How do you list stashes?**  
    ```bash
    git stash list
    ```

33. **How do you apply a stash?**  
    ```bash
    git stash apply
    ```

34. **How do you drop a stash?**  
    ```bash
    git stash drop
    ```

35. **How do you rename the last commit message?**  
    ```bash
    git commit --amend -m "New message"
    ```

36. **How do you revert a commit?**  
    ```bash
    git revert <commit>
    ```

37. **How do you reset to a previous commit?**  
    ```bash
    git reset --hard <commit>
    ```

38. **What’s the difference between `reset`, `revert`, and `checkout`?**  
    - `reset`: move HEAD & change history  
    - `revert`: create a new commit that undoes a commit  
    - `checkout`: switch to a commit or branch

39. **How do you clean untracked files?**  
    ```bash
    git clean -f
    ```

40. **How do you list ignored files?**  
    ```bash
    git status --ignored
    ```

## 🧪 Git Best Practices and DevOps Scenarios

41. **How do you handle secrets in Git repos?**  
    Use `.gitignore`, secret managers, or tools like Git-Secrets.

42. **How do you write an effective `.gitignore`?**  
    List paths, directories, or file patterns to exclude from Git.

43. **What is Git submodule and how is it used?**  
    Used to include one Git repo in another.  
    ```bash
    git submodule add <repo>
    ```

44. **How do you resolve a detached HEAD state?**  
    Create a new branch from current commit and check it out:
    ```bash
    git checkout -b temp-branch
    ```

45. **How do you squash multiple commits into one?**  
    ```bash
    git rebase -i HEAD~n
    ```

46. **How do you sign commits?**  
    Configure GPG key and use `git commit -S`.

47. **What is `git bisect`?**  
    Used to find a commit that introduced a bug via binary search.

48. **What is Git workflow used in CI/CD pipelines?**  
    Common ones: Git Flow, GitHub Flow, Trunk-based Development.

49. **What are hooks in Git?**  
    Scripts that run on events like commit, push, merge.

50. **How do you tag a version and push it?**  
    ```bash
    git tag v1.0
    git push origin v1.0
    ```
