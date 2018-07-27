# Changelog

### 7.0.11

Bugfixes and an enhancement (7/27/18)

* **ENHANCEMENT** You can now delete entries from your form submission log
* Icons now show correctly when submitting a contact form
* Fixed issue preventing all design assets from downloading on some servers
* Prevents warning in Twitter menu item when there are no tweets
* Fixed menu item border that was being applied to the collapse icon in vertical menus
* Fixed max-width setting for form elements
* Links in text modules now correctly respect the "open in new window" checkbox
* Ensuring embedded grid galleries display images in correct order

### 7.0.10

Bugfixes (7/13/18)

* Preventing design initialization modal from rendering on every page if initialization fails to complete

### 7.0.9

Bugfixes (7/6/18)

* Major refactor of saving process to prevent layouts/blocks from intermittently disappearing on the front
* Fixed incorrect corner radius calculations in Tiles causing wrong radiuses in some scenarios
* Fall back to first grid style if a grid's assigned style has been deleted
* Prevent deletion of all of your grid styles
* Fixed scrolling issues mobile menu icon when visual building
* Repairing some designs imported from P6 that couldn't modify module visibility
* You can now select which email field in a contact form is the reply-to address
* Prevent grid galleries from being duplicated on pages with multiple galleries
* In Layouts area, layouts now correctly show single page assignments
* In Layouts area, single gallery (and other custom post type) pages are now assignable

### 7.0.8

Bugfixes (6/21/18)

* Grid title was incorrectly getting classname for the read more link
* (regression) "$" fix in 7.0.7 caused a multitude of other encoding issues, so using more comprehensive approach

### 7.0.7

Bugfixes (6/20/18)

* Fixed issue in Safari causing changes to mobile menu to not display correctly
* Ensuring layouts are initialized immediately after auto-update, instead of on next page load
* Tiles now show hover state on touch devices when touched
* Grid items now correctly respect setting to open in a new window
* Preventing "$" character from getting stripped out of site content

### 7.0.6

An new feature and some bugfixes (6/15/18)

* **ENHANCEMENT:** X-ray mode (in the view mode menu) allows you to view hidden/small items in visual builder for easier editing
* CSS was't getting browser cache broken on the front end, occasionally resulting in customization changes not displaying
* (regression) Save change in 7.0.5 wasn't saving a new layout if it wasn't currently being edited

### 7.0.5

Bugfixes (6/13/18)

* Added progress bar for design initialization pop-up
* Switched save technique to deal with blocks/layouts sporadically not dislpaying on the front
* Fixed grids so that the entire grid item can be clicked to follow it's link
* Fixed tiles which have image layers so they can be dragged into a layout
* Fixed white screen of death bug related to vertical menus in designs imported from ProPhoto 6
* Fixed multiple choice field types in forms so they can be edited
* Fixed grid read-more link customizations that were applying incorrectly to grid titles
* Fixed WordPress Content Moudle image customizations that were not applying correctly

### 7.0.4

Bugfixes (6/6/18)

* ProPhoto version text at bottom of admin pages now links to this changelog
* A conflict with WP Engine hosting was causing the visual builder to not display at all
* Embedded thumbnail galleries weren't displaying on the front
* "$" character in WordPress content was being encoded incorrectly
* Embedded gallery images were incorrectly getting WordPress content module image settings
* Custom CSS from Settings > Advanced > Custom Code wasn't being applied
* Block height settings weren't displaying correctly at breakpoint settings
* Gallery builder is now compatible with yoast seo plugin
* Were incorrectly trying to fetch p6 import data from p5 users
* Creating/importing a design will now not duplicate WordPress media library items
* Grid read more links were always underlined

### 7.0.3

An enhancement and some bugfixes (5/25/18)

* **Enhancement:** Comments now have an optional user consent checkbox for GDPR compliance
* Galleries would not display on the front for some designs imported from ProPhoto 6
* Imported designs were initializing with an empty front page, resulting in 404 message
* In designs imported from ProPhoto 6, modules hidden at different breakpoints weren't being hidden on the front
* Clicking to collapse a vertical menu while visual building was causing a white screen of death
* The mobile menu wasn't properly hiding/showing based on breakpoint settings
* SEO meta title now correctly displays your site/article title
* Modules weren't draggable in some scenarios
