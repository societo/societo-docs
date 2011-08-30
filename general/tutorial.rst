=====================
Tutorial (Imcomplete)
=====================

Getting started
===============

Societo concepts
----------------

Societo aims to realize any social site -- but, what is "social"?

Facebook, Google+ or Twitter? No, they are just one implementations of social community.

Networking? No, if you share aims with others who don't have real connection with you, it is sufficient to build a format of "social".

Many social sites implements that their own distinct "socal" world. The mission of Societo is to realize any type of social sites so Societo can't set own "social" definition.

Well, Societo doesn't define any "social". But instead, it provides useful tools you to realize your own "social".

Have you play with the blocks when you was a child? Or playing house? Simply stated it is similar to what Societo is trying to realize.

Do you want to create your image of small social land or big social world by using Societo?

So, what should I do first?
---------------------------

Access to root of your site (means index.php with no parameters) to feel about above concept.

You will see the following blank page which is created by the Societo Installer.

.. image:: /images/tutorial_blank_page.*
    :width: 320px
    :target: ../_images/tutorial_blank_page.png

Do you understand about our concept? You need to put the pieces for building your social site.

Every page is built by using "Page" feature
-------------------------------------------

You can do "putting the pieces" is from "Page" feature in backend.

You may be already in backend. If not, click "Admin" link in page footer.

.. image:: /images/tutorial_point_to_admin_link.*
    :width: 320px
    :target: ../_images/tutorial_point_to_admin_link.png

Click "All Pages" of the side banner in backend and you can see a page list which shows two pages.

.. image:: /images/tutorial_point_to_page_link.*
    :width: 320px
    :target: ../_images/tutorial_point_to_page_link.png

There are "insecure_default" and "secure_default". A blank page which you access in the previous section is "secure_default".

insecure_default? Actually, it is a login page. Yes, installer creates login page for you automatically.

.. note::
    Currently, Societo is incomplete, so you are able to rename and delete insecure_default and secure_default.
    But, these pages are depended by system. So deleting these pages may damage normal working of Societo.
    The problem must be solved in the feature. But, for now, please operate carefully while wating the solution.

Well, look into insecure_default. Click "insecure_default" of the menu and display the following page.

.. image:: /images/tutorial_insecure_default.*
    :width: 320px
    :target: ../_images/tutorial_insecure_default.png

There are two areas; the one has a "Username Login Form" (plot area) and another one has many boxes e.g. "Edit Profile Form", "Member Search Form", ...

Societo calls these box "Page Gadget".

Next, look into secure_default...

.. image:: /images/tutorial_secure_default.*
    :width: 320px
    :target: ../_images/tutorial_secure_default.png

You can see the plot area doesn't have any gadget. This means a blank page.

Do you notice plot area has gray-colored few sub area. Drag-and-drop a gadget from list of gadgets to the sub area, you can get gadget configuration dialog. For example, in case of free area gadget (which is provided by SocietoFreeAreaPlugin), a form to input any HTML like the following:

.. image:: /images/tutorial_gadget_config.*
    :width: 320px
    :target: ../_images/tutorial_gadget_config.png

Input mandatory item, enter, and the gadget is put to the plot area.

.. image:: /images/tutorial_ploted_gadget.*
    :width: 320px
    :target: ../_images/tutorial_ploted_gadget.png

OK, access the user page and confirm results.

.. image:: /images/tutorial_confirm_ploted_page.*
    :width: 320px
    :target: ../_images/tutorial_confirm_ploted_page.png

You can see the gadget and is has the inputted values correctly.

Don't worry, "Recipe" feature helps you
---------------------------------------

But -- yes, but, even if it is flexible, repeating that creating page, ploting gadget and confugure it, is laborious. If so, you will give up building your own social site.

Don't worry. Societo provides a way to skip this trouble. It is "Recipe" feature. Let's try it.

First, click "Recipe" from the side menu.

.. image:: /images/tutorial_point_to_recipe_link.*
    :width: 320px
    :target: ../_images/tutorial_point_to_recipe_link.png

There are forms and two button. I think this interface is not good so I will fix this to friendly one in the stable release.

Well, input "http://recipe.societo.org/example.xml" to "Input recipe URL" field and submit.

.. image:: /images/tutorial_recipe_results.*
    :width: 320px
    :target: ../_images/tutorial_recipe_results.png

Your inputted is URL to a recipe which is prepared by Societo. Societo read this recipe and show the like above. A list of plugins, pages, and menus are displayed.

Please read a content of this recipe and click button. Then ...

.. image:: /images/tutorial_recipe_eat_up.*
    :width: 320px
    :target: ../_images/tutorial_recipe_eat_up.png

This page is appeared. Don't you know what's happend? OK, please display a list of pages once again.

.. image:: /images/tutorial_cooked_page.*
    :width: 320px
    :target: ../_images/tutorial_cooked_page.png

Something was increased! Yes, these are pages which Societo "cooked" automatically by that "Recipe" feature.

Look into secure_default page.

.. image:: /images/tutorial_cooked_secure_default.*
    :width: 320px
    :target: ../_images/tutorial_cooked_secure_default.png

Some gadgets are added. Look into other pages if you want.

Are you satisfied now? This is a power of "Recipe" feature. So, with a recipe what are compiled basic page structures if you need, Societo creates sites by following it.

After the requesting founation work in Societo, all it takes to do build your own social site is to do an interior design. Of course you can start your site with no changes.

Currently, Societo prepares the http://recipe.societo.org/example.xml recipe only. But, for example, if there are "Recipe for Twitter-like social site", "Recipe for compony", "Recipe for couple", "Recipe for disposable social site", and etc -- is fine, isn't it? We realize the recipe contributing site in the near futer. If you already have an idea of the recipe? Well, please send DM to @co3k in Twitter. I'll introduce it in our blog.
