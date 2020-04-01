![vgb_logo](https://i.ibb.co/99dkgjM/VGB-studio-black-1.png)

# VGB USER GUIDE

In this guide you will find the step-by-step instructions for customizing the storefront developed on the ScandiPWA theme for Magento.

## VGB BaboonCloud credentials

FE - https://vgb.babooncloud.com/

BE - https://vgb.babooncloud.com/admin

*Login*: admin

*Password*: 931865b85d

## Useful Links

[ScandiPWA User Guide](https://scandiweb.atlassian.net/wiki/spaces/SUG/overview)

[Magento 2 User Guide](https://docs.magento.com/m2/ce/user_guide/getting-started.html)

## Homepage Slider

![slider](https://i.ibb.co/5TkKDGQ/Screenshot-2020-04-01-at-12-23-04.png)

On the homepage, you are able to switch between women and men slider that allows you to have different content.

> **NOTE!** The horizontal slider including "men" and "women" buttons cannot be changed manually.

For the sliders to appear on the homepage, you should use the following **slider identifiers:**

1. WOMEN - slider ID 5 
2. MEN - slider ID 6

**TO ADD THE HOMEPAGE VERTICAL SLIDERS:**

Follow the guide [here](https://scandiweb.atlassian.net/wiki/spaces/SUG/pages/1758855269/Slider+Management).

**TO ADD THE CONTENT ON SLIDES:**

1. Open your slide in edit.
2. Under **Block 1** section, find the **Block Text** editor.
3. Switch to the HTML editor (tap on **Show/Hide editor**)
4. Use the following template for the block text:
    1. When using paragraph text: 
       1. ````<div class="HomePage-SlideContent"><h1 class="HomePage-SlideTitle"> CONSUME YOURSELF </h1> <p class="HomePage-SlideSubTitle"> There is no telling to people who they are or who they should be. Nor what they should feel.</p><a class="Button Button_isHollow HomePage-SlideButton" href="/category/women/collection">SEE MORE</a></div>````
    2. When not using paragraph text: 
       1. ````<div class="HomePage-SlideContent"><h1 class="HomePage-SlideTitle"> CONSUME YOURSELF </h1><br><a class="Button Button_isHollow HomePage-SlideButton" href="/category/women/collection">SEE MORE</a></div>````

>**NOTE!** After any change with the Scandiweb Slider Manager, go to **System** > **Tools** > **Cache Management**, and choose **Flush Cache Storage**.

## Menu

![menu](https://i.ibb.co/RjLzMBd/Screenshot-2020-04-01-at-12-44-24.png)

Similar to the homepage slider, menu also gives you an ability to have different menus for men and women catalogs.

Menu overlay has a horizontal slider bettween men and women.

In both slides of the menu, the "More infos" is present. More infos section is integrated as additional menu. This way it will allow easier content management inside the tab without requiring a change in the code.

For the menus to appear on the menu overlay, you should use the following **menu identifiers:**

1. WOMEN - women-menu
2. MEN - men-menu
3. MORE INFOS - moreinfo-menu

**TO CREATE THE MENUS:**

Follow the guide [here](https://scandiweb.atlassian.net/wiki/spaces/SUG/pages/1691418673/Menu+Manager).

## Product Listing Page

![PLP](https://i.ibb.co/1vPLXZw/Screenshot-2020-04-01-at-13-05-38.png)

On the product listing page, each 5th product (starting from the first one) is a hero product that gets displayed in full-screen.

The attribute (in our example - "New") will appear on the hero products only.

**TO SET AN ATTRIBUTE TO BE VISIBLE ON PLP:**

Follow the guide [here](https://scandiweb.atlassian.net/wiki/spaces/SUG/pages/1695711539/Color+and+Content+Customization).

Scroll down until the **content customization** section and see the **Product List** in the table.

***

Category description and category title are displayed under the header and are centralized.

Filters are opened in the overlay. No matter what attribute type is set for your filterable attributes, they will be rendered vertically as per design.

If there are more than 3 attribute values for the attribute, the "Show more +" button will appear. On click, it changes to "Show less -" and the additional attribute values appear visible.

## Product Description Page

### Mobile

![PDP mobile](https://i.ibb.co/NSnYKgN/Screenshot-2020-04-01-at-15-02-16.png)

On the mobile product description page, the vertical slider is implemented.

The user has an ability to go back to the previous category page by clicking on the "Back to X" button, where X is the category he was browsing.

To see the product descirption and choose available product options, the user needs to drag bottom element up.

To return back to the product image gallery, the user can drag the same element down or click the "X" button in the upper-right corner.

The product options will appear in the dropdown. No matter what attribute type is set for your attributes, they will be rendered as dropdowns as per design.

### Desktop 

TBD

## My Favorites

![my favorites](https://i.ibb.co/W53dWTP/Screenshot-2020-04-01-at-15-52-35.png)

On the desktop view of my favorites, the products are rendered by 4 in the line. On mobile, in turn, in one column.

In my favorites, the user can add products to cart one by one, go back to the product page by clicking on the "View Item" button, or remove products from the list.

## Contact Us
