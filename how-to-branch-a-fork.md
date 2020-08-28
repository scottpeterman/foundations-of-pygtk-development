# git working with forked repo - using custom branch

### create branch from cloned master of repo
```git checkout -b learning1```
#### output
``Switched to a new branch 'learning1'```

### push new branch creation - will then appear in web ui
```
git push origin learning1
Total 0 (delta 0), reused 0 (delta 0)
remote: 
remote: Create a pull request for 'learning1' on GitHub by visiting:
remote:      https://github.com/scottpeterman/foundations-of-pygtk-development/pull/new/learning1
remote: 
To github.com:scottpeterman/foundations-of-pygtk-development.git
 * [new branch]      learning1 -> learning1
```
### first push requires setting upstream reference
``` git push --set-upstream origin learning1
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 299 bytes | 299.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To github.com:scottpeterman/foundations-of-pygtk-development.git
   5eabe85..ddebfc0  learning1 -> learning1
Branch 'learning1' set up to track remote branch 'learning1' from 'origin'.
```
### verify active branch in local repo
```
git branch
* learning1
  master
```

### Now Regular workflow works
````
git add -A
git commit -m "my message"
git push
````

