# LH Archived Post Status
Allows posts and pages to be archived so you can remove content from the main loop and feed without having to trash it.

<br>

## Development Info

### Contributors
shawfactor (original contributor), [Marco Di Bella ](https://github.com/mdibella-dev) (this fork)

### Tags
admin, posts, pages, status, workflow

### Requires at least

- WordPress 5.0

### Tested up to

- WordPress 6.3

<br>

## Description

This plugin allows you to archive your WordPress content similar to the way you archive your e-mail. Unlike other archiving solutions though this actually does it all and does it properly

- Makes a new post status available in the drop down called Archived
- Hides or removes your content without having to trash the content
- Content can either be hidden entirely from public view  or simply from the main loop and feed and pages, with other solutions you can only hide it from public view.
- Allows you to add a label to the title of those posts/pages etc that are archived
- Allows you to add a message to the top of the post/page etc that the content is no longer up too date
- Allows you to set an archiving date after which content is automatically changed to having an archived status
- Compatible with posts, pages and custom post types

This plugin is ideal for sites where certain kinds of content is not meant to be evergreen

<br>

## Frequently Asked Questions

**Isn't this the same as using the Draft or Private statuses?**

Actually, no, they are not the same thing.

The Draft status is a "pre-published" status that is reserved for content that is still being worked on. You can still make changes to content marked as Draft, and you can preview your changes.

The Private status is a special kind of published status. It means the content is only available to certain logged in users.

The Archived post status, on the other hand, is meant to be a "post-published" status. Once a post has been set to Archived the content is either hidden entirely from non logged in viewers or removed from the front page and feed (but still available on singular pages). This behaviour is controlled in the settings screen.

<br>

**Doesn't this do the same thing as the other archiving plugin in the repository?**

Actually it does more! Unlike the other plugin content archived with this plugin can still be available to non logged in visitors (depends on plugin settings) and just  removed from the front page and xml feeds (with a custom message can also be added to flag to visitors that the content is no longer up too date). Alternately it can be hidden entirely (to non logged in viewers).

<br>

**Can't I just trash old content I don't want anymore?**

Yes, there is nothing wrong with trashing old content. However it will be hidden from non logged in viewers.

However, WordPress automatically purges trashed posts every 7 days (by default), so it will be gone.

This is what makes the Archived post status handy. You can unpublish content without having to delete it forever.

<br>

**How can I view a listing of my archived content on its own archive pagelisting all archived posts, pages etc?**

This not not part of my plugin per se but it is easily done.

The easiest way would be to install a plugin that allows you to query by post_status e.g.: https://wordpress.org/plugins/display-posts-shortcode/ and input the shortcode with the post_status of archive:, e.g. `[display-posts post_status=”archive”]`

If you want to customise the display that shortcode has plenty of arguments. There are also other shortcodes tha can do this (just search the repository).

<br>

**My archived posts have disappeared when I deactivate the plugin, why is this?**

The reason is that WordPress no longer recognises them, but they are still in the database. If you no longer need the plugin, just reactivate it, switch all the archived posts/pages/cpts to a native post status and THEN deactivate the plugin.

<br>

**What if something does not work?**

LH Archived Post Status, and all [LocalHero](https://lhero.org) plugins are made to WordPress standards. Therefore they should work with all well coded plugins and themes. However not all plugins and themes are well coded (and this includes many popular ones).

If something does not work properly, firstly deactivate ALL other plugins and switch to one of the themes that come with core, e.g. twentyfifeen, twentysixteen etc.

If the problem persists please leave a post in the [support forum](https://wordpress.org/support/plugin/lh-archived-post-status/). I look there regularly and resolve most queries.

<br>

**What if I need a feature that is not in the plugin?**

Please contact me for custom work and enhancements here: [https://shawfactor.com/contact/](https://shawfactor.com/contact/)

<br>

**Is there a template function to including archiving functionality appropriately on the front end?**

Yes the plugin defines the function archive_post_link which acts almost identically to the WordPress native function edit_post_link. That is clicking it will archive the relevant post is the current user has the edit_post capability. You can add it to you theme.

<br>

## Installation

1. Upload the entire `lh-archived-post-status` folder to the `/wp-content/plugins/` directory.
2. Activate the plugin through the 'Plugins' menu in WordPress.
3. Navigate to Settings->Reading and set the visibility and archiving message

<br>

## License

This package ist released under **GPLv2 or later**. License URI: http://www.gnu.org/licenses/gpl-2.0.html
