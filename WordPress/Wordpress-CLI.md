### Quick Notes:
Checks WP Version & Plugin Titles that need update:
```
wp cron event run --due-now

wp core version

wp plugin list --update=available --fields=title --format=csv | awk 'NR>1 {gsub(/"/, ""); print}'
```
Updates WP Version & All Plugins
```
wp core update

wp plugin update --all

wp cache flush
```
### Site Management

1. `wp core download` - Download WordPress core files.
2. `wp core install` - Install WordPress with basic configuration.
3. `wp core version` - Check Wordpress Version
4. `wp core update` - Update WordPress to a newer version.
5. `wp core verify-checksums` - Verify WordPress files against checksums.
6. `wp db export` - Export the database.
7. `wp db import` - Import a database file.
8. `wp db optimize` - Optimize the database.
9. `wp db repair` - Repair the database.
10. `wp db reset` - Reset the entire database.
11. `wp site empty` - Empty a site of its content.

### Plugin Management

1. `wp plugin activate` - Activate a plugin.
2. `wp plugin deactivate` - Deactivate a plugin.
3. `wp plugin delete` - Delete a plugin.
4. `wp plugin install` - Install a plugin.
5. `wp plugin list` - List all plugins.
6. `wp plugin update` - Update one or more plugins.
7. `wp plugin status` - Check the status of plugins.
8. `wp plugin list --update=available` - Checks all plugins that need update
12. `wp sg purge` - Clears Siteground Purge  
     

### Theme Management

1. `wp theme activate` - Activate a theme.
2. `wp theme delete` - Delete a theme.
3. `wp theme disable` - Disable a theme.
4. `wp theme enable` - Enable a theme for network.
5. `wp theme install` - Install a theme.
6. `wp theme list` - List themes.
7. `wp theme update` - Update a theme.

### User Management

1. `wp user create` - Create a new user.
2. `wp user delete` - Delete a user.
3. `wp user list` - List users.
4. `wp user update` - Update a user.
5. `wp user generate` - Generate dummy users.
6. `wp user set-role` - Set the role of a user.

### Post Management

1. `wp post create` - Create a post.
2. `wp post delete` - Delete a post.
3. `wp post edit` - Edit a post.
4. `wp post generate` - Generate dummy posts.
5. `wp post list` - List posts.
6. `wp post update` - Update a post.
7. `wp post meta` - Manage post meta.

### Media Management

1. `wp media import` - Import media files.
2. `wp media regenerate` - Regenerate thumbnails.
3. `wp media list` - List media items.

### Comment Management

1. `wp comment create` - Create a comment.
2. `wp comment delete` - Delete a comment.
3. `wp comment list` - List comments.
4. `wp comment approve` - Approve a comment.
5. `wp comment unapprove` - Unapprove a comment.
6. `wp comment spam` - Mark a comment as spam.
7. `wp comment unspam` - Unmark a comment as spam.

### Taxonomy Management

1. `wp term create` - Create a term.
2. `wp term update` - Update a term.
3. `wp term delete` - Delete a term.
4. `wp taxonomy list` - List taxonomies.

### Maintenance and Debugging

1. `wp cron event run` - Run a cron event.
2. `wp cron event list` - List cron events.
3. `wp eval` - Execute arbitrary PHP code.
4. `wp eval-file` - Execute a PHP file.
5. `wp export` - Export content to a WXR file.
6. `wp import` - Import content from a WXR file.
7. `wp cache flush` - Flush the cache.

### Database Management

1. `wp db cli` - Open a MySQL command-line interface.
2. `wp db query` - Execute a SQL query.
3. `wp db search` - Search through the database.

### Multisite Commands

1. `wp site create` - Create a site in a multisite network.
2. `wp site delete` - Delete a site from a multisite network.
3. `wp site list` - List sites in a multisite network.
4. `wp network meta` - Manage metadata of a network.

### Development and Maintenance

1. `wp scaffold child-theme` - Generate child theme.
2. `wp scaffold plugin` - Generate starter code for a plugin.
3. `wp scaffold post-type` - Generate post type code.
4. `wp scaffold taxonomy` - Generate taxonomy code.
5. `wp shell` - Interactive WP-CLI shell.

### Security

1. `wp security check` - Perform security checks.
2. `wp security update` - Update security features.

### Localization

1. `wp language core install` - Install a core language.
2. `wp language core activate` - Activate a core language.
3. `wp language plugin install` - Install a language for a plugin.
4. `wp language theme install` - Install a language for a theme.

### Miscellanea

1. `wp transient delete` - Delete transients.
2. `wp transient set` - Set a transient.
3. `wp transient get` - Get a transient value.
4. `wp option get` - Get an option value.
5. `wp option update` - Update an option value.
6. `wp option delete` - Delete an option.
7. `wp option list` - List all options.

### Advanced Commands

1. `wp rewrite list` - List rewrite rules.
2. `wp rewrite flush` - Flush rewrite rules.
3. `wp rewrite structure` - Set the permalink structure.
4. `wp capability list` - List all capabilities.
5. `wp capability add` - Add a capability.
6. `wp capability remove` - Remove a capability.

### Hosting and Server

1. `wp server` - Launch PHP's built-in web server.
2. `wp package install` - Install a WP-CLI package.
3. `wp package uninstall` - Uninstall a WP-CLI package.

### Package and Version Management

1. `wp cli update` - Update WP-CLI itself.
2. `wp cli info` - Print WP-CLI information.
3. `wp cli check-update` - Check for update of WP-CLI.
4. `wp cli alias` - List and add WP-CLI aliases.

### Testing and Environment

1. `wp doctor check` - Run checks to identify problems.
2. `wp doctor list` - List all available checks.
3. `wp config create` - Create a `wp-config.php` file.
4. `wp config list` - List the configurations.