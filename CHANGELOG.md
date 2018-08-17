# Changelog

### 7.1.3

Bugfix

* Fixes horizontal menu dropdowns not showing when hovered after 7.1.2 update

### 7.1.2

Bugfixes and enhancement (8/15/18)

* **ENHANCEMENT** Revised our design initialization process to be much, much, much faster :)
* Added gallery placeholder in visual builder for galleries that are embedded in post/page content
* Fixed 'disable facebook meta' checkbox in the ProPhoto Settings so it works
* Fixed bug causing background galleries to disappear on front after an auto-update
* Fixed layout custom CSS so it works when viewing the site
* Fixed collapsible vertical menus so they display collapsed by default as intended
* Fixed regression in delete modified image button which resulted in deletion of p6 gallery images in some scenarios
* Fixed bug with initial background gallery sizing in the visual builder
* Fixed onboarding bug causing design home page to redirect to incorrect page 

### 7.1.1

Bugfixes (8/7/18)

* Updated and optimized the 6 included designs and improved their onboarding experience
* Working around bug in Safari to get text layers center aligning correctly in Tiles
* The remote email sending option in the ProPhoto settings area now reliably sends emails
* Background videos from YouTube and Vimeo should now autoplay
* Our Google Tag Manager code will now only run on the front when you are logged in, for GDPR compliance
* Fixed thumbnail gallery displaying wrong thumbnail when clicked and never-ending spinner
* Fixed issue with category dropdown menu item excluding extra categories
* Prevents attachments from overloading the server when importing a large ProPhoto6 design

### 7.1.0

Features, enhancements and a bugfix (8/2/18)

* **FEATURE** Activating an included or purchased design now sets up all assigned pages and posts for you automatically.
* **FEATURE** Page navigator dropdown added to Visual Builder.  Quickly jump between editing different pages of your site.
* **ENHANCEMENT** Visual Builder controls UI was restructured for better usability
* **ENHANCEMENT** Blocks in the block library now show what layouts they are used in when hovering the green "usage" circle
* The 'delete modified images' button in the settings area now actually deletes modified images ¯\_(ツ)_/¯

### 7.0.11

Bugfixes and an enhancement (7/27/18)

* **ENHANCEMENT** You can now delete entries from your form submission log
* Tiles used in grid read-more links now get their fonts sized correctly
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
