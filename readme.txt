=== Plugin Name ===
Contributors: halgatewood
Tags: food, nutrition, nutrition label, nutrition facts
Tested up to: 3.4
Requires at least: 3.0
Stable tag: 1

== Description ==

This plugin creates a 'nutrition-label' custom post type which can be assigned to any page or post. 

You can also include a label with the shortcode 'nutrition-label' which generates a FDA-style nutrition label.

See http://en.wikipedia.org/wiki/Nutrition_facts_label for more information on nutrition labels.

Reference daily intake values come from http://en.wikipedia.org/wiki/Reference_Daily_Intake

This plugin is forked from the wp-nutrition-label plugin found at http://romkey.com/code/wp-nutrition-label

== Installation ==

1. Upload /nutrition-facts-label to the /wp-content/plugins directory

2. Activate the plugin through the Plugins menu in WordPress

3. Create a label in the new 'Labels' section of the admin.

4. Include the shortcode [nutrition-label id=100] where you want a specific label to be displayed. 

5. DEVELOPERS: When creating the label you can also specify the Page or Post you want the label to appear and include echo do_shortcode("[nutrition-label]"); in the template where you want the label.

== Frequently Asked Questions ==

= What units does the label use? =

* Grams: totalfat, satfat, transfat, carbohydrates, fiber, sugars, protein
* Milligrams (mg): cholesterol and sodium
* Unitless: servings and calories (units are implicit for calories)
* You should include the unit in the serving size attribute (ie: "4 oz")

= What about **Calories from Fat**? =

The **Calories from Fat** number is computed from the totalfat attribute.

= What about vitamins? =

Thinking about it.

= How do I style the nutrition label? =

You can control the width with the "width" attribute. The width attribute uses **ems** as its unit. It is styled to scale but it's likely that the "Nutrition Label" text won't scale well as the default font is Helvetica, which isn't fixed-width.

Each label as an id attribute of wp-nutrition-label-{ID} which allows you to change the label as you see fit.

= How about calculating the nutrition values based on a recipe? =

This is **really** hard to do. To do it at all reliably requires human intervention to match ingredients names against their entries in a nutrition database. That's a level of difficulty I don't wan to try to tackle with this plugin. You may find the USDA's free online nutrition database useful for looking up nutrition information:

http://www.nal.usda.gov/fnic/foodcomp/search/


== Screenshots ==

1. New Labels Section

2. List view in the admin, custom columns for shortcode and the page it is assigned to.

3. Add/Edit Label Form

4. Include 'do_shortcode' in your template.  It will search for the first label associated to that page.

5. Include labels on a per-page basis.

6. Example output

== Upgrade Notice ==

= 1 =
* Initial Release, forked and updated from wp-nutrition-label plugin

== Changelog ==

= 1 =
* Initial release
