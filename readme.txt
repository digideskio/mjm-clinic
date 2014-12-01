=== MJM Clinic ===
Contributors: damanic
Donate link: http://mjman.net
Tags: clinic, therapy, services, listings, health, conditions
Requires at least: 4.0
Tested up to: 4.1
Stable tag: 1.0.1
License: GPLv3
License URI: http://www.gnu.org/licenses/gpl-3.0.html

A tool for hosting clinic and health care related websites. Enables presentation of services with relations
to common health conditions, health indications/symptoms and related products. Fully integrated booking forms.

== Description ==
Built to add functionality to any theme, the MJM Clinic plugin makes use of widgets and shortcodes for quick integration.

The MJM Clinic plugin allows you to

* Create numerous Clinic/Service locations, with contact details/forms, address, maps.
* Create hierarchical health service categories
* Create Service/Therapy listings, assign them to one or more locations, one or more categories and one or more indication/symptom tags.
* Create Patient feedback entries and assign them to a service and/or health condition.
* Create Case Studies and assign them to a health condition and/or service.
* Create Indication and Contraindication tags to link services, conditions, patient feedback, case studies, products etc.
* Set up a service/advice disclaimer.
* Enable/Disable combinations of the above features.
* Enable/Disable comments on your service listings.

= In the pipeline =

* Create related products that can be displayed on various pages through tags or direct relation. These products can be set up to link to an online shop.


= Widgets =

Numerous sidebar widgets have been included to help show off your services, health conditions info, clinic locations etc.
* Assigned Case Studies - can be assigned to feature on a specific service or a health condition page
* Assigned Condition - Health conditions can be assigned to feature on any number of specified service listings
* Assigned Patient Feedback - can be assigned to feature on a specific service or a health condition page
* Assigned Services - Displays a list of services that were specifically assigned to a health condition, patient feedback or case study
* Clinic Locations - Displays clinic locations where a service/therapy is available
* Indication Tags - Displays a list of indication tags for service, condition, feedback and case study single posts
* Location Map - Displays a map on a location taxonomy page
* Related Casestudy - Displays casestudy on single tax and post pages that share indications
* Related Feedback - Displays feedback on single tax and post pages that share indications
* Related Health Conditions - Displays conditions on single tax and post pages that share indications
* Related Services - Displays services on single tax and post pages that share indications
* Service Categories - A list or dropdown menu of clinic service categories.
* Service Session Info - Displays a services session info, price
* Shared Symptoms - Displays other conditions that share symptoms (indication tags)


= Shortcodes =

`[mjm-clinic-booking-form]`
Output an ajax form, can have more than one per page without conflicts.
Optional attributes = ['service', 'location', 'no_service_select', 'no_location_select']

Example Usage:
[mjm-clinic-booking-form service='cold-flu' location='my-clinic' no_service_select=1 no_location_select=1]
The above will generate a form for the given service and location (slugs), and hide/disable the options for the user to select/change the service or location.

Without any attributes the form will show drop downs for location and services, and detects the most relevent
form state for the page.


= Helper Functions =
There are a number of helper functions that can be used in your theme, which are found in `inc/func.php`.


= Theme Integration =
All plugin generated output includes an abundance of css classes and id's all of which use mjm-clinic prefixes to prevent conflicts with any other plugins or themes.
MJM Clinic works out of the box, but theme developers can easily over-ride the default presentation styles and templates.


TO OVERIDE THE DEFAULT CSS
Copy the following files from {MJM-CLINIC-PLUGIN-DIR}/views/css/ to {YOUR-THEME-DIR}/mjm-clinic/ . Customise away.
* `public.css`

TO OVERIDE THE BOOKING FORM JS
Copy the following files from {MJM-CLINIC-PLUGIN-DIR}/views/css/ to {YOUR-THEME-DIR}/mjm-clinic/ . Customise away.
* `booking_form.js`

TO CUSTOMIZE THE CATEGORY PAGES
Copy the following files from {MJM-CLINIC-PLUGIN-DIR}/views/templates/ and place them in the root of your theme folder. Customise away.
* `taxonomy-mjm_clinic_service_category.php`
* `taxonomy-mjm_clinic_service_location.php`
* `taxonomy-mjm_clinic_indication.php`

TO CREATE YOUR OWN SERVICE, CONDITION, FEEDBACK AND CASE STUDY TEMPLATES
Create the following files in your themes root directory. Use your themes single.php as reference for setting up a single post template.
* `single-mjm_clinic_service.php`
* `single-mjm_clinic_condition.php`
* `single-mjm_clinic_feedback.php`
* `single-mjm_clinic_casestudy.php`



= About this plugin =
This plugin was created for clinics to promote services and products in a way that inter-relates with information on health conditions and symptoms.



== Installation ==

1. Upload `mjm-clinic.zip` to the `/wp-content/plugins/` directory or use the built-in plugin installer on the WordPress Plugin Dashboard page.
3. Activate the plugin through the 'Plugins' menu in WordPress
3. Have a look at the plugin settings, thats it!
4. Optional: Install the taxonomy-images plugin if you would like images for any of your categories/taxonomies.

== Frequently Asked Questions ==

[Ask some]

== Screenshots ==

1. Description


== Upgrade Notice ==
None

== Changelog ==

= 1.0.1 =
* initial release