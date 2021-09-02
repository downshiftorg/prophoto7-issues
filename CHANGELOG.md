# Changelog

### 7.7.19

enhancements (09/01/2021)

* **Enhancement** Updated ProPhoto for PHP 8 support, as well as dropping support for unsafe PHP versions under 7.3 (which are no longer supported by PHP)
* **Enhancement** After a change to Instagram's API, we now periodically refresh your connection, so you shouldn't have to re-authorize your account

### 7.7.18

bugfixes (08/11/2021)

* **NOTICE** - This release prevents future auto-updates for anyone running a PHP version under 7.3 on their site. Our September 1 release of ProPhoto 7.7.19 will only support PHP versions 7.3 and higher **including adding support for PHP 8**.
* Improved handling of fixed background images on iOS devices
* Fixed bug occasionally causing Instagram images to be missing from Instagram grids on slower servers

### 7.7.17

bugfixes (12/09/2020)

* Added the wp_body_open action which is used by some plugins
* Updated REST route paths which were causing PHP notices on sites that were in WP Debug mode
* Grouped loading of galleries in visual builder to prevent lots of galleries from overwhelming some slower servers
* Fixed bug causing the slideover menu to show incorrectly in some scenarios just in Safari browser
* Adding hook for a support plugin to fix WPML plugin issue that could cause a design regeneration loop in the admin
* Fixed some jQuery deprecations for the jQuery update in WordPress 5.6 release

### 7.7.16

bugfixes (07/19/2020)

* Fixed issue from Instagram enhancement that was preventing video thumbnails from displaying correctly
* ProPhoto galleries inserted as full sized images now correctly lazyload, include alt tags, and use srcset if available
* Fixed a regression that broke ProPhoto image watermarking
* Fixed bug preventing visual building of WooCommerce product category pages
* Page dropdown menu item is now sorted by page order values if set
* WordPress tiled galleries inserted into pages/posts now work as expected
* List item fonts selected in text modules now correctly override the default font setting
* Deleting copies of a designs original slideover block no longer cause a white screen error
* Fixed issue causing PHP warnings if WordPress debug mode was turned on

### 7.7.15

enhancement (06/23/2020)

* **Enhancement** Updated Instagram integration to work with Instagram API changes.  Instagram images are now uploaded to media library.

### 7.7.14

bugfixes (02/19/2020)

* Fixed error showing up at bottom of pages containing excerpt grids
* Should now work with php 7.4
* Cleaned up styling of gallery insertion form in classic editor after latest WordPress update
* The blog link in the layout manager now actually links to home page if home is set to show blog posts

### 7.7.13

bugfixes (01/31/2020)

* Slideover blocks were not scrolling all the way to the bottom
* Thumbnail galleries on a page no longer prevent scroll-to links from working
* Preventing fatal error when WPML plugin is enabled with ProPhoto 7 (NOTE: this is not providing any WPML support for ProPhoto 7, just preventing a fatal error).
* Additional guarding to prevent "View Context" fatal error
* Trying to prevent timeouts when importing designs
* Preventing failures when importing designs containing videos
* Improving compatability with PHP 7.4

### 7.7.12

bugfixes (11/20/19)

* **Enhancement** Fixed conflicts that were preventing NextGen Gallery compatibility
* A css change in WordPress 5.3 was resulting in content images getting a left and right margin
* Changes in the latest versions of Firefox were resulting in an error when saving in the visual builder
* Deleting the default grid or gallery style was throwing an error
* Making sure we don't cache SSL requests as non-SSL requests
* Removed some unnecessary CSS from front pages of site

### 7.7.11

bugfixes (10/15/19)

* (regression) Fixed error in the Post/Page editor when trying to insert a select posts grid
* Preventing scroll jumpiness after navigating to a page with a scroll-to link
* Gallery images now display in the correct order after inserting a Post or Page and saving

### 7.7.10

bugfixes (10/2/19)

* A grid including a post with an old ProPhoto 5 gallery, will now correctly show the first image in the grid
* Fixed tile bug causing layers respositioned on hover to be misaligned in some scenarios
* Repositioned the text module toolbar so it isn't cut off by edges of screen when in a narrow column
* Grids now use full sized images when ProPhoto image downsizing is disabled
* Re-worded some labels in the Layout settings area for more consistency/clarity
* Fixed incorrect spacing above and below some elements caused by changes in newer browser versions
* Prevent an Instagram error notification from causing a JavaScript error on site
* Grids now use high resolution images for high resolution (retina) devices

### 7.7.9

bugfixes (9/6/19)

* Fixed regression in 7.7.8 that could cause blocks with graphics and background galleries to render incorrectly

### 7.7.8

bugfixes (9/4/19)

* Fixed bug causing block control bars in the visual builder to display out of position
* Preventing a specific combination of grid settings from causing a white screen in the visual builder
* Using a scrollto link from within a grid item now works properly
* Fixed bug causing off-site images from being loaded properly
* Removed duplicate filter call that was causing some plugins to be displayed twice
* Fixed issue causing images and background galleries to not load properly after saving in certain browsers
* Fixed issue causing a custom font to go missing when importing from ProPhoto 6
* Password protected gallery pages now show the password form when loaded directly 
* Fixed some typos in the Settings area

### 7.7.7

bugfixes (7/24/19)

* **ENHANCEMENT** Added support for embedding video blocks responsively
* Fixed grid issue when a grid image was corrupted or missing image data in the media library
* Fixed form submission issue related to changing your site url
* Fixed issue resulting in images being pixelated (too small) in scenarios where srcsets couldn't be generated
* Fixed image rendering issue after switching site to https

### 7.7.6

bugfixes (6/20/19)

* Fixed mobile menu visibility issues
* Fixed issue causing multiple tiles in a graphic module to incorrectly display on multiple lines

### 7.7.5

bugfixes (6/18/19)

* (regression) Design generation error was causing incorrect menu fonts due to migration failure
* (regression) Modules that were being animated from the right were creating scrolling issues on mobile

### 7.7.4

Enhancements and bugfixes (6/17/19)

* **ENHANCEMENT** Gallery pages now render a gallery placeholder in the visual builder
* **ENHANCEMENT** Default to alphabetical ordering of all lists of pages/galleries
* **ENHANCEMENT** Adding responsive sizing to tile images for better performance
* Preventing duplicate recent posts dropdown menu
* Improved loading of galleries in the visual builder
* Locking the default layout from editing without confirmation
* Manage designs screen auto-scrolls to newly added designs
* Several performance optimizations to speed up the visual builder
* Some controls in the WordPress content module were being hidden incorrectly

### 7.7.3

Bugfixes and an enhancement (6/3/19)

* **ENHANCEMENT** Added importing of ProPhoto 4 & 5 galleries (under galleries > import)
* **ENHANCEMENT** Reorganized blocks by usage in current layout, to make them easier to find
* **ENHANCEMENT** Dropdown options at the top of the visual builder now close when you click anywhere outside of them
* Improved handling of sites using HTTPS, preventing browser errors due to left-over HTTP requests
* Prevent multiple spaces in text modules from collapsing to a single space
* Multiple WordPress content modules on a page could result in excerpt grid not displaying enough items
* Fixed encoding issue causing titles of posts/pages to show incorrectly in some areas of the visual builder 
* Assigning a layout to all WooCommerce pages was resulting in that layout appearing on all pages period 🤦‍
* Tooltip for deleting modules was showing text for blocks

### 7.7.2

Bugfixes (5/17/19)

* Fixed issue causing menu dropdowns to get the wrong font style applied
* Font selection wasn't working in WordPress Widget modules
* Dropping support for PHP 5.4 and 5.5 in keeping with WordPress' own requirements

### 7.7.1

Bugfixes (5/8/19)

* Removed old error reporting code that was causing a PHP warning
* Fixed edge case where special characters in custom font names could cause them to not display on the front of a site

### 7.7.0

Enhancements and bugfixes (5/6/19)

* **ENHANCEMENT** Added a "full size images" style to the prophoto gallery block for use in the gutenberg editor
* **ENHANCEMENT** Font styles have been re-worked, making them much more powerful, flexible, and easier to use
* **ENHANCEMENT** Bold, italic, list, and blockquote formatting options added to the text module
* Added work-around for Instagram authorization error for non-native english users
* Fixed timing issue that could cause the media button to not work when using the classic editor
* Fixed post author links not getting encoded correctly
* Fixed issue where customization settings couldn't be overridden in "stuck" mode for sticky blocks

### 7.6.4

Bugfixes (4/4/19)

* Added several fixes for broken/stuck instagram grids, included a notice when Instagram account authorization has expired
* Ensuring we display all categories in grid form when selecting a category related grid type
* Fixed an issue where contact form submissions containing HTML would break the form submission log
* Users who imported footer link removal from ProPhoto 6 will now be asked to re-submit their license
* Setting in the form for inserting a grid in a post/page weren't working properly in the classic editor

### 7.6.3

Bugfixes (3/14/19)

* Preventing occasional issue causing Slideover blocks and mobile menu icons to disappear after updates
* regression - Fix for rare issue with extraneous media images in 7.6.2 was caused an error

### 7.6.2

Bugfixes (3/12/19)

* regression - Fixed issue resulting on fatal error on blog page when using excerpt grid
* Updated code causing a PHP warning on PHP 7.3

### 7.6.1

Bugfixes (3/6/19)

* Fixes conflict that was preventing creation of a post/page from the BlogStomp app
* Fixes conversion to block of ProPhoto galleries that were inserted using the classic editor
* Grid placeholders were incorrectly showing up on pages that shouldn't be showing grid excerpts
* Premium designs weren't displaying their thumbnail image corretly on the manage designs screen
* Some fixes to font styles in excerpt grids when in the visual builder
* Prevents thumbnail style galleries from breaking if gallery images are deleted from the media library
* Images aligned left or right at the end of content were resulting in incorrectly positioned comments area
* Fixes issues with grid images on a few webhosts with non-standard WordPress installations
* Adds support for plugin fix in rare cases where ProPhoto was creating extraneous empty images in the media library 

### 7.6.0

Features, enhancements, and bugfixes (2/19/19)

* **FEATURE** Introducing ProPhoto Gallery and Grid blocks for WordPress 5. Using WordPress 5's block editor, you can now visually add and edit ProPhoto Galleries and Grids from within your post/page editor.
* **FEATURE** You can now select a default gallery style and grid style to use any time they are embedded in a post or page
* **ENHANCEMENT** Grids without any content now show a placeholder for easier management
* **ENHANCEMENT** Added an opt-in error/message logging tool to aid us in debugging your sites
* Improved handling of custom fonts during design generation to ensure they save correctly
* Making a slideover block unique no longer blows up your layout
* The correct font style is now being applied to validation text in ProPhoto forms
* Cleaned up design generation to avoid rare instances of elements dissapearing on front of site

### 7.5.0

Features, enhancements, and bugfixes (1/23/19)

* **FEATURE** Added a guided tour through the visual builder to help new users get their bearings
* **ENHANCEMENT** Controls for blocks and modules in the visual builder no longer scroll off the screen
* **ENHANCEMENT** ProPhoto now warns you when attempting to delete your WordPress content module in layouts that should have one
* Regenerating site HTML/CSS if the WordPress site or home urls change
* Modules that are sliding over from the right no longer cause weird scroll bar issues
* Fixes issue causing galleries to not render in posts/pages when using the classic editor plugin
* Added pagination to ProPhoto's form log, avoiding errors for users with hundreds of form submissions
* Hosts using a centralized location for WordPress core files no longer breaks ProPhoto generated images
* Fixes issue where hidden grids were breaking scrollto links
* Space above and below image settings now correctly apply to images inserted with the old "ProPhoto insert all" method
* Custom CSS applied to a row at a specific breakpoint now applies correctly
* Fixes carousel gallery image alignment when used as a background gallery

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
