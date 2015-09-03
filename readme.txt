=== CIO Custom Field Groups for PODS  ===
Contributors: VisualData
Donate link: http://vipp.com.au/cio-custom-fields-importer/custom-field-groups-for-pods/
Tags: pods custom field groups, custom field groups, custom fields, pods group, custom field sections, custom field headers, custom field footers, group location rules, pods, ACF, advanced custom fields
License: GPLv2
License URI: http://www.gnu.org/licenses/gpl-2.0.html
Requires at least: 3.9.0
Tested up to: 4.3
Stable tag: 1.0.0

Copy, drag, drop, done. No PHP code required. This plugin extends PODS to group custom fields quickly and intuitively and support location rules and short codes.

== Description ==

Are you already using the awesome [PODS](https://wordpress.org/plugins/pods/) plugin to manage your custom content types and fields? 

Are you switching from Advanced Custom Fields to PODS but missing the location rules found in Advanced Custom Fields? 

Are you looking for a simple way to present your custom field data on your website in logical blocks? 

CIO Custom Field Groups for PODS may be the solution you are looking for. 

CIO Custom Field Groups for PODS extends PODS to organize your custom fields into groups quickly and intuitively. The group headers are pods custom fields named with a prefix "cio_section_". Groups are defined by the relevant position of custom fields in pods setting page, so grouping and re-grouping can be done quickly by dragging and dropping meta boxes.

The free version of CIO Custom Field Groups hooks into PODS form to generate a row with label and description only, without input cells. Output of group header fields in the front end is optional depending on your page template and pods template.

Custom fields used as group headers are field definition only without any data saved to these fields. If you use pods table storage, you may set up group header fields as relationship fields so that such fields will not be created in your data table.

PHP code is not required to use this plugin. However if you are comfortable with PHP code, you may instantiate the class in this plugin and use class methods to manipulate the custom fields and groups in your page template. 

= CIO Custom Field Groups Premium Version =

The premium version of CIO Custom Field Groups has the following additional features:

* dividing custom fields into groups (under headers) and sub-groups (above footers). 

* configuring the header and footer field prefix, if you need to name the fields in a certain way for the database to integrate with other plugins/programs.

* configuring the header and footer field background in the admin panel.

* configuring the header and footer field css for frontend display.

* setting up restriction access and display conditions similar to location rules of ACT

* supporting pods-form short code and two additional short codes cio-header and cio-footer for conditional display at the front end. 


* Displaying sections of custom fields according to user roles or capabilities. For example, you may collect and display different information is the users are wholesalers.  

* Display sections of custom fields on specified pages only. 

* Admin only custom fields.


CIO Custom Fields and Groups is an add-on to PODS but can be used to group custom fields created with other plugins. This is achieved by sharing the stored data between your plugin and PODS, thanks to the great work of PODS team.

Bothe the free and professional edition works in multisite environment.


PS: I am releasing the professional edition to the public to raise fund for a long time friend who runs a charity from Australia called [Captivating](http://captivating.org/). Captivating has a dedicated team to help victimised children in developing countries. CIO Custom Fields and Groups Professional Edition is bundled with extra features and is freely available to supporters of Captivating. If you are willing and able financially, please consider giving to Captivating. Any amount is appreciated. Tax deductible receipts are available if you are giving from Australia, US or Hong Kong. Please check with Captivating about receipts if you are giving from other countries.

[CIO Custom Fields and Groups Professional Edition](http://vipp.com.au/cio-custom-fields-importer/custom-field-groups-for-pods/) is also available for immediate download for a small once-off fee.

=How does it work=

We believe things should be as simple and easy as it could be. We embrace this philosophy in our code and business model.

CIO Custom Fields and Groups defines groups by the position of custom fields relevant to a group header, in the same way as groups are displayed in forms or on paper. Fields beneath a group header belongs to this group. Similarly, fields above the group footer belongs to the group.  You can use either headers or footers, or both to define groups.


CIO Custom Fields and Groups professional edition hooks into Pods core files so you can use PODS short code to display an edit form by specifying header or footer names.

`[pods-form name="mypod" id="321" headers="0, myheader1, myheader2" footers="myfooter1, myfooter2, 0" ]`

Grouping is optional with CIO Custom Fields and Groups. If some fields are grouped and some are not, you can access these ungrouped fields by using a dummy header or footer name "0" (zero), as shown in the example above.

Note headers and footers are used in the short code instead of groups. This is to avoid confusion with the "group" functionality under development and testing by pods team. 

CIO Custom Fields and Groups professional edition filters the parameters in the short code, identifies the fields in the group, and passes the field names to PODS to generate a form. 

Similarly, CIO Custom Fields and Groups professional edition hooks into Pods to display a header and footer label only without an input cell. 

CIO Custom Fields and Groups uses builtin table structures of WordPress and PODS to define groups. No extra taxonomy or data is created. The professional edition of CIO Custom Fields and Groups supports PODS shortcode and magic tags in shortcode template.

To display a group defined by the header field "my_header" from a custom post type called "product", you would use the following short code. 

`[pods name="product" id=123] {@my_header} [/cio-header]`

When CIO Custom Fields and Groups professional edition is activated, and preset display conditions are met, the custom fields belong to this group will be displayed. 

When CIO Custom Fields and Groups professional edition is deactivated, the above shortcode simply displays nothing, as no data is ever stored in the special relationship field "my_header". 

Please see screen shots for more examples. 

CIO Custom Fields and Groups Professional Edition comes with 

* unlimited site license. you can use it on as many websites as you like, either owned by you or your clients, or your neighbors, or your friends.

* life time free support, if you have paid an one-off fee to upgrade to professional edition

* life time free upgrade, if you have paid an one-off fee to upgrade to professional edition

* 30 day money back guarantee. no questions to ask.



== Installation ==


To install the CIO Custom Fields and Groups, unzip the downloaded zip file and upload the folder to /wp-content/plugins/, and then activate the plugin from the Plugins page in WordPress.

If you are using the free plugin and bought the professional edition, please remove the free plugin before installing the professional edition.


== Frequently Asked Questions ==

To update later.


== Changelog ==



= 1.0.0 =
* Initial release.


== Upgrade Notice == 

to update later.


== Screenshots == 

1. registration page with custom fields and groups. 

2. configuring individual custom fields (feature by PODS). When groups are enabled in CIO Custom Fields and Groups professional edition, you can set up conditions as group default, and set up extra conditions for individual fields.

3. color coded group headers ($head -> sky => blue) and footers ($foot -> grass => green). You can drag and drop custom fields, the headers or footers to update the custom field group quickly. (grouping of custom fields is available in professional edition only)

4. conditions to display or hide the groups. Pods relationship fields are used as headers and footers. You can set up these fields to relate to objects in WordPress, or even tables outside WordPress.

5. configuring display conditions of groups. This configuration set up here will be checked to decide whether to display a group.

6. when this plugin is activated, you can use extra parameters (headers, footers) in Pods short code. 

7. example of headers and footers in generated form. You may customise the display of headers and footers with CSS.   

8. extra custom fields in WooCommerce Checkout page, as an example. 

9. example of headers and footers in user profile. 




== Support ==


We do try to handle support at the following e-mail address:

E-mail: support@vipp.com.au


