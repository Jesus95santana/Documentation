### **Remove Files from Github**

Modify .gitignore File

```text-plain
git add .gitignore
git commit -m 'Modified .gitignore'
```

Remove git cache All (based on .gitignore & current Directory)

```text-plain
git rm --cached -r .
```

Remove git cache one folder

```text-plain
git rm --cached -r wp-content/plugins/sg-cachepress/
```

Commit and push

```text-plain
git commit -m "Remove ignored files from repository"
git push origin main
```

Add to a commit

```text-plain
git commit --amend 
```