=== Featured Image Admin Thumb ===
Contributors: seanchayes
Donate link: https://www.seanhayes.biz/
Tags: post-thumbnail, thumbnail, admin, image, featured, featured image, featured thumbnail, featured admin thumbnail
Requires at least: 5.3
Requires PHP: 7.0
Tested up to: 6.1
Stable tag: 2.0
License: GPLv2 or later
License URI: http://www.gnu.org/licenses/gpl-2.0.html

Adds inline thumbnail image to admin columns on Post/post types view (where supported). Click to easily set/change the featured image.

== Description ==

When active this plugin adds a column to the All Posts/All Pages and where supported the All Custom Post Type admin views. This column, "Featured Image", will display a thumbnail of the featured image or post thumbnail so you can easily determine the content that is missing an image.

You can also make inline edits that allow you to change the featured image from the All Posts/All Pages/All Custom Post Type view without having to edit the post.

The plugin is now translatable using the wp.org translation tools.

== Installation ==

= Using The WordPress Dashboard =

1. Navigate to the 'Add New' in the plugins dashboard
2. Search for 'featured-image-admin-thumb'
3. Click 'Install Now'
4. Activate the plugin on the Plugin dashboard

= Uploading in WordPress Dashboard =

1. Navigate to the 'Add New' in the plugins dashboard
2. Navigate to the 'Upload' area
3. Select `featured-image-admin-thumb.zip` from your computer
4. Click 'Install Now'
5. Activate the plugin in the Plugin dashboard
6. Consider using a thumbnail re-generator to create specific thumbnails for the All Posts/Pages admin views

= Using FTP =

1. Download `featured-image-admin-thumb.zip`
2. Extract the `featured-image-admin-thumb` directory to your computer
3. Upload the `featured-image-admin-thumb` directory to the `/wp-content/plugins/` directory
4. Activate the plugin in the Plugin dashboard

== Frequently Asked Questions ==

= You don't see the thumb column and the thumbnails in that column =

After checking that the plugin is enabled, be sure to click Screen Options if you don't immediately see the column and ensure "Featured Image" has a checkmark next to it

= My thumbnail column shows posts with blank areas in the thumb column =

During testing I found that if a post has a featured image assigned but does not show a thumbnail it was because the image file is missing it will show up blank within the sorted posts that do show thumbnails

== Screenshots ==

1. The Featured Image column in the All Pages/Posts admin view when no featured image is set.
2. The Featured Image column in the All Pages/Posts admin view when a featured image is set.
3. The Featured Image column in the All Pages/Posts admin view when a featured image is set and the click action is set to edit post.
4. The screen options pull down menu in the Post/Pages screen.

== Changelog ==

2.0 (TBD)
* Allow different thumbnail sizes to be used.
* Allow user to set what action is taken when clicking the thumbnail (edit post or set featured image), if set to edit post, the "Set featured image" link will appear below the thumbnail.
* Add settings page for above options.
* Renamed "Thumb" column to "Featured Image".
* Added function to generate the required thumbnail size if it does not yet exist.

1.6 (2021-03-30)
* Addresses plugin conflict when using Gutenberg editor and ACF [Conflict with ACF](https://wordpress.org/support/topic/conflict-with-acf-11/)

1.5.3 (2019-07-01)
* Addresses thumb column dislay issue with EDD Frontend Submissions [Plugin not working with EDD](https://wordpress.org/support/topic/plugin-not-working-with-edd/)

1.5.2 (2018-09-26)
* Addresses an issue where in Excerpt view where the displayed thumbnail did not represent the thumbnail in the post. Switching to List view, however, the thumbnail showed correctly.
* Fix for support request [odd thumb behavior in excerpt view:](https://wordpress.org/support/topic/odd-thumb-behavior-in-excerpt-view/)

1.5.1 (2018-08-31)
* Add thumb column to EDD Downloads. Use filter (documented in 1.4.2 release) if you want to exclude thumb column in EDD Downloads. Code linting.

1.5.0 (2018-06-21)
* Ability to sort featured image thumbnail column. You can easily see the content that has a featured image, displays no featured image or has no featured image assigned to it.
* Posts that have not had a featured image assigned will show up as Set featured image

1.4.4 (2017-11-22)
* Restoring an accidental PHP specific array definition to be compatible with earlier PHP versions

1.4.3 (2017-11-8)
* A general tidy up release
* Code tidy up, removal of unneeded definitions and legacy unused functions
* Correcting return variables
* Adjust `fiat_thumb` image size to be square and have a centered crop
**you might** need to regenerate thumbnails if there are visual inconsistencies with thumbnails.
* Escaping in markup has been improved

1.4.2 (2017-5-15)
* Updated list of default excluded post types
* Page post type is now included by default hopefully fixing [this support query:](https://wordpress.org/support/topic/4-7-changed-the-flow-odd-use/)
* Added filter "fiat/restrict_post_types"
* Example filter usage `add_filter( 'fiat/restrict_post_types', 'your_theme_name_restrict_post_types' );` then create a function `your_theme_name_restrict_post_types` to modify and return and array of post_types to exclude

1.4.1 (2016-6-9)
* Bug fix when checking sizes and removal of pencil based on support feedback

1.4 (2015-11-16)
* Language translation functionality added

1.3.6 (2015-10-29)
* Removed post check inadvertently included from another branch and was restricting display of thumbnail column

1.3.5 (2015-10-28)
* Check if WooCommerce is installed and if so adjust column output on WooCommerce product post type page [reported here thank you:](https://wordpress.org/support/topic/conflict-with-woocommerce-25)

1.3.4 (2015-08-14)
* Check if sizes is an array before looping over it as [reported here:](https://wordpress.org/support/topic/how-to-cure-sql-corruption) to prevent PHP error display
* Updated stable tag

1.3.3 (2015-02-04)
* Additional excluded post type
* Markup and JS to support showing the selected thumbnail in the media uploader

1.3.2 (2015-02-04)
* Minor improvement to code that attaches FIAT column handler to Posts, Pages and other taxonomy screens
* Inclusion of fix from [here:](https://wordpress.org/support/topic/would-like-to-see-media-category-sort) that allows filters from other plugins to work

1.3.1 (2014-07-24)
* Adding in missing Genericons.

1.3 (2014-07-15)
* Added highlighting on images in All Post/All Pages/All Custom Post Type screens - displaying an edit icon that when clicked can change the featured image inline without having to edit the relevant content item

1.2
* Add custom media uploader (css and js) support for all registered and active custom post types

1.1
* Improved sizing logic when displaying existing thumbnails

1.0.2
* Updated logic to detect best thumbnail size to use

1.0.1
* Added thumbnail size check to use default "thumbnail" if bundled "fiat_thumb" is not available for some images

1.0
* First version

== Upgrade Notice ==
You might upgrade to the latest version to take advantage of thumbnail column sorting - see which of your content has a thumbnail assigned or not.

== Updates ==
