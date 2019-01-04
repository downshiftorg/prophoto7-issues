# Changelog

### 7.4.3

Bugfixes (1/3/19)

* Woff uploading works again after the WordPress 5.0.1 and 4.9.9 security updates broke it
* Slideover block positioning wasn't correctly taking the layout top margin into account
* Fixes issue causing special characters in post title/content to break grid display
* Fixes fatal DOM document error related to comments

### 7.4.2

Bugfixes (12/20/18)

* Recent posts dropdown menu item now only shows published posts
* (Regression) Our patch to fix the embedded gallery error broke the visual builder 😬

### 7.4.1

Bugfixes (12/19/18)

* Images added to post as a WordPress image block weren't getting the ProPhoto image spacing/alignment settings
* In some scenarios, ProPhoto page caching wasn't clearing properly after saving in the visual builder
* Embedded galleries were causing a fatal error when viewed in the WordPress 5 block editor

### 7.4.0

Features, enhancements, and bugfixes (12/10/18)

* **FEATURE** Module animations - Add animations to modules that are triggered as they are scrolled into view
* **FEATURE** ProPhoto caching - Page and CSS caching functionality that can greatly improve page load speeds
* **ENHANCEMENT** In layout area, assignments for posts and pages are now clickable to quickly visually build those pages
* **ENHANCEMENT** Added more tooltips to the visual builder for improved usability
* In the visual builder in Firefox, the slideover block was displaying outside of the preview area
* In IE11, the thumbstrip of a gallery with many images was displaying the images super tiny :open_mouth:
* In some cases, stuck customizations for rows/columns in a sticky block weren't applying
* Fixes image alignment issues related to WordPress 5.0 image block

### 7.3.1

bugfixes (11/21/18)

* Scroll-to links weren't scrolling to the correct position when there was a grid on the page
* Tiles with scaled images were doing not good things in IE11
* Radio inputs in a ProPhoto form were submitting the wrong selected value
* Saving changes to font style with custom font while using Safari caused problems when viewing site in Chrome
* Scroll to link validation was failing in Firefox
* (regression) Fixes fatal error on pages using an Instagram grid

### 7.3.0

Features and bugfixes (11/8/18)

* **FEATURE** WooCommerce support - Integrate e-commerce into your site with the WooCommerce plugin. ProPhoto allows assignmnent of layouts to all the major WooCommerce pages and product pages
* **FEATURE** You can now add checkbox elements to ProPhoto forms
* **FEATURE** Enter a custom slug for your ProPhoto gallery pages (in Settings > Misc)
* **ENHANCEMENT** Added a horizontal alignment setting for ProPhoto grids
* Fixes a caching issue with Instagram causing Instagram grids to not load in some scenarios
* Tiles inside of graphic modules were incorrectly utilizing the image size constraint setting
* Archive dropdown menu items were all jacked up if WordPress installation had a non-standard directory structure
* Image watermarking was breaking for users with ImageMagick

### 7.2.3

Enhancement & Bugfixes (10/18/18)

* **ENHANCEMENT** (GDPR compliance) Go to Settings > Site Settings > Social Media to entirely disable social media network support on site
* Fixes pixel rounding issue in masonry grids that could result in 1 pixel spaces between images
* Comment customizations are now available in WordPress content module regardless of what page type you're currently on
* A background image on the layout with attachment set to scroll now displays properly in the visual-builder
* Sorted issue with h1 vs. h2 tags for article titles on single and multipost pages
* Titles of slide-up style grids weren't vertically aligning properly if font style had a non-100% line height

### 7.2.2

Bugfixes (10/5/18)

* Enhanced ProPhoto's detection of file structure to accommodate unusual WordPress setups on some webhosts
* Fixes post-auto-update issue that was resetting a subset of customizations for some layouts
* Fixes scrollto positioning errors when there is a sticky block
* (regression) Our approach with horizontal menu dropdown spacing wasn't compatible with menu item background hover color

### 7.2.1

Bugfixes (10/1/18)

* Fixed bug causing a white screen of death on SEO settings page when using an SEO plugin
* Fixed Instagram grid issue causing distortion of images at smaller sizes
* Updated Instagram authentication process due to changes in Instagram API
* Added work around for importing ProPhoto 6 attachments on slower servers
* Added vertical spacing options for dropdowns in horizontal menus
* Fixed bug preventing registration form from submitting

### 7.2.0

Major release with new features and enhancements, as well as some bug fixes

* **FEATURE** Quickly jump to visual editor mode from any post/page editor screen via a button in the WordPress toolbar
* **FEATURE** Insert/Edit grids in a post or page using the ProPhoto button
* **FEATURE** Hide post titles on a layout by layout basis
* **FEATURE** Added 2 brand new included designs, and did some refining of our existing designs
* **ENHANCEMENT** Including 'getting started' link and video to the end of the registration process
* **ENHANCEMENT** Added number of posts setting to the recent posts from category grid
* **ENHANCEMENT** Added default text to WordPress content module for 404 pages
* Refactored CSS generation resulting in significant performance improvements for layouts that include a WP content module
* Fixes vertical centering within full-height blocks in Internet Explorer 11
* Prevent catastrophic jumbling of live design when auto-updating site with live and customizing designs
* Fixes vertical alignment issues within slide-up style grid overlays

### 7.1.7

Bugfixes (9/17/18)

* Fixed comment bug resulting in fatal error after saving layout on a page with comments disabled
* Removed extra space showing under galleries on phones when showing the control bar outside of the gallery

### 7.1.6

Bugfixes (9/14/18)

* Reworked comment rendering to allow 3rd party commenting plugins to display (Disqus support)
* Fixed SEO settings problem incorrectly showing a SEO plugin enabled (contact us if your site is still in this state)
* Fixed issue causing an empty graphics module to be un-editable after saving
* Added tutorial links to all of our included designs on the manage designs screen
* Fixed error in ImageMagick downsizing causing grid/gallery images to not show the first time they were loaded
* Updates image sizing calculation in grids that was resulting in undersized images in some scenarios
* Fixes duplication of submenu items in pages and categories dropdowns
* Fixes sticky blocks not always sticking on the front

### 7.1.5

Performance improvements and bugfixes (9/5/18)

* **FEATURE** Lazyloading of images (Settings > Site Settings > Misc) can improve page load times
* **ENHANCEMENT** Added image downsizing support for grids to prevent loading of full-sized images
* **ENHANCEMENT** Added more control for quality/sharpening of downsized images (Settings > Site Settings > Misc)
* Fixed bug that was resulting in always using the inferior GD library for image downsizing, even when ImageMagick was available
* Added validation for scroll-to links in menu items, preventing invalid scroll-to links from resulting in invalid links
* Fixed bug causing embedded video backgrounds to be sized incorrectly
* Fixed bug in search menu item preventing the search results from displaying correctly

### 7.1.4

Bugfix (8/21/18)

* Fixed bug causing creation of empty, unattached modules that were causing errors in multiple places
* Custom Statcounter code wasn't being rendered on the front
* Fixed errors preventing additional gallery images from loading when image missing meta data
* Fixed incorrect layout assignments for the default "Creative" design
* Adds "customize" button to live design, to switch back to editing mode for that design

### 7.1.3

Bugfix (8/17/18)

* (regression) Fixes horizontal menu dropdowns not showing when hovered. Broken by 7.1.2 update

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
