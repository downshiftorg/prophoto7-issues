# Changelog

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
