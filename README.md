![vgb_logo](https://i.ibb.co/99dkgjM/VGB-studio-black-1.png)

# VGB USER GUIDE

In this guide you will find the step-by-step instructions for customizing the storefront developed on the ScandiPWA theme for Magento.

## VGB ScandiPWA Cloud

FE - https://vgb.scandipwa.cloud

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
     ````<div class="HomePage-SlideContent"><h1 class="HomePage-SlideTitle"> CONSUME YOURSELF </h1> <p class="HomePage-SlideSubTitle"> There is no telling to people who they are or who they should be. Nor what they should feel.</p><a class="Button Button_isHollow HomePage-SlideButton" href="/category/women/collection">SEE MORE</a></div>````

>**NOTE!** After any change with the Scandiweb Slider Manager, go to **System** > **Tools** > **Cache Management**, and choose **Flush Cache Storage**.

## Menu

![menu](https://i.ibb.co/RjLzMBd/Screenshot-2020-04-01-at-12-44-24.png)

Similar to the homepage slider, the menu also gives you an ability to have different menus for men and women catalogs.

Menu overlay has a horizontal slider between men and women.

In both slides of the menu, the "More infos" is present. More infos section is integrated as an additional menu. This way it will allow easier content management inside the tab without requiring a change in the code.

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

On the mobile product description page, the vertical slider is implemented.

The user has an ability to go back to the previous category page by clicking on the "Back to X" button, where X is the category he was browsing.

To see the product description and choose available product options, the user needs to drag the bottom element up.

>The dragbar can be opened by sliding down after the last image of the product image slider.

To return back to the product image gallery, the user can drag the same element down or click the "X" button in the upper-right corner.

The product options will appear in the dropdown. No matter what attribute type is set for your attributes, they will be rendered as dropdowns as per design.

The product short description is rendered under the "Add to Cart" button.

The product description is rendered in the expandable tab.

### Desktop

On the desktop PDP, product images are rendered vertically one by one.

>You can download both horizontal and vertical images to the products, however the preferred option is vertical due to the mobile slider.

The position of the product information block on the right side is fixed, therefore when scrolling the page down, you will see only the image gallery scrolling.

The roduct short description is rendered under the product price.

The product description is rendered in the expandable tab.

## My Favorites

![my favorites](https://i.ibb.co/W53dWTP/Screenshot-2020-04-01-at-15-52-35.png)

On the desktop view of my favorites, the products are rendered by 4 in the line. On mobile, in turn, in one column.

In my favorites, the user can add products to cart one by one, go back to the product page by clicking on the "View Item" button, or remove products from the list.

**NOTE!** Only logged in users can add items to the wishlist.

## Contact Us

https://vgb.scandipwa.cloud/contact-us

There are 4 expandable tabs displayed on the contact us page:

1. CALL CENTER VAGABOND

On the first line, the store phone number is rendered.

It should be set in **Admin -> Stores -> Configuration -> General -> General -> Store Information -> Store Phone Number**

On the second line, the working hours are rendered.

They should be set in **Admin -> Stores -> Configuration -> General -> General -> Store Information -> Store Hours of Operation**

2. E-MAIL SUPPORT

The support email address can be managed in **Admin -> Stores -> Configuration -> General -> Store Email Addresses -> Customer Support -> Sender Email**

3. STAY SOCIAL

Under the "Find us here:" note, the CMS block is located.

To display the CMS block in the expandable tab, the block identifier should be "**contact-us-social**".

>When saving the block, make sure your content is not covered in the **p** tag.

4. FORM APPLICATION

The contact us form is located in under the form application tab.

On click on the "Send Your Message" button, the form applications are sent to the email address, set in **Admin -> Stores -> Configuration -> General -> Contacts -> Email Options -> Send Email To**

>**NOTE!** Make sure the contact us is enabled in **Admin -> Stores -> Configuration -> General -> Contacts -> Contact Us -> Enable Contact Us**

## Store Location

https://vgb.scandipwa.cloud/stores

On the stores page, the dropdown with all available cities is located.

By default, the dropdown title is Romania and can be changed only manually through the code.

Inside the dropdown, you will see all the available cities that are set to you stores in **Admin -> Scandiweb -> Store finder -> Stores -> Store detailed view -> City Name**.

>If there are multiple stores set for one city, the city name will not be dublicated in the dropdown.

**TO CREATE A NEW STORE**

1. On the admin sidebar, choose **Scandiweb**
2. Under **Store Finder**, choose **Stores**
3. Tap on **Create new store**
4. Fill in the **store name** (will appear on the storefront)
5. Fill in the **store ID** (will not appear, but is a required field)
6. Fill in the **city name** (will appear in the dropdown on the storefront)
7. Fill in the **city ID** (will not appear, but is a required field)
8. Fill in the **store address** (will appear on the storefront)
9. Fill in the **phone number** (will appear on the storefront)
10. Add the store **image**
11. Under the **More Info**, fill in the **Store Working Hours** (will appear on the storefront)
12. Under the **More Info**, add the **Extra image 1**
13.  Under the **More Info**, add the **Extra image 2**
14.  When complete, tap **Save Store**

**NOTE!** For the changes to appear on the storefront, go to the Magento Cache Management, and choose **Flush Cache Storage**.

## Cookie Notice

Cookie notice can be enabled on the storefront by following the guide [here](https://scandiweb.atlassian.net/wiki/spaces/SUG/pages/1693286407/Cookie+Law+Compliance).

The Cookie Popup Read more Link text was changed to the "Click here for more information on our Cookies policy"

## Social Login

### Facebook

>**Note:** *Verify Your Business on Facebook. You can connect your app to a Facebook Business Manager account, if applicable, and get started on the business verification process. You'll just need to upload a document showing your business or organization's name and physical address. After successfully completing business verification, you'll also need to sign either 1 or 2 contracts. [Learn more](https://developers.facebook.com/docs/apps/review/#business-verification)*

>**Note:** *Individual Verification Paused.
Due to coronavirus (COVID-19), we have temporarily paused Individual Verification to focus our reviewers on efforts that help keep people informed and safe. We know this review step is important and will resume it as soon as we can. [Learn More](https://developers.facebook.com/blog/post/2020/03/24/pausing-individual-verification/)*

TO SET UP FACEBOOK SOCIAL LOGIN:

1. Visit https://developers.facebook.com/
2. LogIn
3. Go to **MyApps**
4. Choose **Create App**
5. Fill in the necessary fields
6. Click **Set up**
7. At the App dashboard Click **Settings -> Basic**
8. Fill in the necessary fields
9. Also there You will be able to find **App ID** and **App Secret**
10. Go to **Products -> Facebook Login -> Settings**
 Fill field Valid OAuth Redirect URIs like: https://base_url/sociallogin/endpoint/?hauth.done=Facebook https://base_url/sociallogin/endpoint/?hauth_done=Facebook & 
(https://vgb.scandipwa.cloud/sociallogin/endpoint/?hauth.done=Facebook &
https://vgb.scandipwa.cloud/sociallogin/endpoint/?hauth_done=Facebook)
11. Save changes

### Google

TO SET UP GOOGLE SOCIAL LOGIN:

1. Visit [console.cloud.google.com/](console.cloud.google.com/)
2. LogIn
3. In Header (Right After Google Cloud Platform), select **My Projects** 
4. Choose **New Project**
5. Fill in the necessary fields
6. At left Menu Bar click On **APIs & Services**
7. At left Menu Bar click On **OAuth consent screen** 
8. Choose User Type **Internal** for testing  or **External** for public
9. Fill in the necessary fields. If Publick - wait for verification
10. Go to **Credentials** and click **+CREATE CREDENTIALS** 
11. Choose **OAuth client ID**
12. **Application type** : Web Application 
13. Fill in the necessary fields 
    1.  Authorized redirect URIs = https://vgb.scandipwa.cloud/sociallogin/endpoint/?hauth.done=Google
14. Press **Create** 
15. In PopUp window you will find You Credentials
