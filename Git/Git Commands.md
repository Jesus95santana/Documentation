### **Remove Files from Github**

Modify .gitignore File

```
git add .gitignore
git commit -m 'Modified .gitignore
```

Remove git cache All (based on .gitignore & current Directory)

```
git rm --cached -r .
```

Remove git cache one folder

```
git rm --cached -r wp-content/plugins/sg-cachepress/
```

Commit and push

```
git commit -m "Remove ignored files from repository"
git push origin main
```

Add to a commit

```
git commit --amend 
```