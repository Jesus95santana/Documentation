### Ignore everything
```
*
```
### Exclude .gitignore from being ignored
```
!.gitignore
```

### Exclude Theme & Plugin directories
```
!public
!public/wp-content/
!public/wp-content/themes/
!public/wp-content/plugins/
!public/wp-content/mu-plugins/
!public/wp-content/mu-plugins/**
```

### Ignore All themes Except
```
public/wp-content/themes/*
!public/wp-content/themes/fictional-block-theme/
!public/wp-content/themes/fictional-university-theme/
!public/wp-content/themes/full-site-theme/
```

### Ignore All plugins Except
```
public/wp-content/plugins/*
!public/wp-content/plugins/are-you-paying-attention/
!public/wp-content/plugins/manual-image-crop
!public/wp-content/plugins/our-first-unique-plugin/
!public/wp-content/plugins/our-word-filter-plugin/
!public/wp-content/plugins/regenerate-thumbnails/
```


### ReIgnore Igore Files
```
.DS_Store
._*
node_modules
```

### Only Ignore Twenty themes
```
#/wp-content/themes/twenty*/
```

### Common plugins to be ignored
```
#/wp-content/plugins/siteground-migrator
#/wp-content/plugins/worker
#/wp-content/plugins/wp-migration-duplicator
#/wp-content/plugins/wordpress-importer
#/wp-content/plugins/sg-security
#/wp-content/plugins/sg-cachepress
#/wp-content/plugins/all-in-one-wp-migration
#/wp-content/plugins/jetpack
#/wp-content/plugins/wordfence
#/wp-content/plugins/wpe-site-migration
```