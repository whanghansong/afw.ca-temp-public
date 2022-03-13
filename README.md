# afw.ca

## v4 (i think i got this)
Steps: 
- 1. Save the files (NOTE: Control + Save)
- 2. CODE: " Git Status " (NOTE: optional: check for status of file changes) 
- -     Example: PS C:\Users\Hansong\projects\afw.ca> git status
        On branch TempV2
        Your branch is up to date with 'origin/TempV2'.
        Changes not staged for commit:
            (use "git add <file>..." to update what will be committed)
            (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md
        no changes added to commit (NOTE: use "git add" and/or "git commit -a") 
- 3. CODE: " git checkout -b tempV3 " (NOTE: this creates a branch "-b" with the name "TempV3")
- -     PS C:\Users\Hansong\projects\afw.ca> git checkout -b tempV3
        Switched to a new branch 'tempV3'
- 4. CODE: " git add . " (add all files to the pool for upload) " git add README.md " (or whatever the file names are)
- 5. CODE: " git statu" (NOTE: just to be sure)
- -     On branch tempV3
        Changes to be committed:
        (use "git restore --staged <file>..." to unstage)
        modified:   README.md
- 6. CODE: " git commit -m  "version 3" " (NOTE: commit changes (this is a required step) and add a description of the changes made)
- -     PS C:\Users\Hansong\projects\afw.ca> git commit -m "Version 3 of practice readme.md file"
        [tempV3 e31bcbc] Version 3 of practice readme.md file
        1 file changed, 13 insertions(+)
- 7. CODE: " git push -u origin tempV3 " (NOTE: "tempV3" is name of the branch. I guess we can use different things if we don't have branches...meh)(when pushing, parameters are not needed if branch already exists)
- -     Enumerating objects: 8, done.
        Counting objects: 100% (8/8), done.
        Delta compression using up to 8 threads
        Compressing objects: 100% (6/6), done.
        Writing objects: 100% (6/6), 1.36 KiB | 696.00 KiB/s, done.
        Total 6 (delta 1), reused 0 (delta 0), pack-reused 0
        remote: Resolving deltas: 100% (1/1), done.
        remote: 
        remote: Create a pull request for 'tempV3' on GitHub by visiting:
        remote:      https://github.com/Sparkx120/afw.ca/pull/new/tempV3
        remote:
        To github.com:Sparkx120/afw.ca.git
         * [new branch]      tempV3 -> tempV3
        branch 'tempV3' set up to track 'origin/tempV3'.
- 8. Now Control + left click the github link and we can see a new git added under the branch tempV3. 
- 9. In github it's now possible to use "Create pull request" to get started to merge a branch to the main. Then eventually "Confirm Merge"
- 10. once that is done it's also okay to delete the branch. (or create a new branch...whatever)
- 11. let's say we merge the branch to main. and .. if we deleted the branch we can now choose to download the New, Merged main files and replace our local copies with the latest. 
- 12. CODE: " git checkout main " (NOTE: switch to main branch) 
- 13. CODE: " git pull " (since we are in main branch now pull will sync main branch with github)
- 14. CODE: " git status " (NOTE: when in doubt, check git status)

- 15. IMPORTANT!! (see below)
- 16. VIM: (VIM opens when have to deal with commit message and things turn ugly. ALWAYS use insert message) "i" to enter insert mode (type text), hit "escape" to switch to normal mode. type ":wq" (stands for: write quit) to exit VIM.
