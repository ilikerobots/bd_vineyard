# Black Dog Vineyard Website



## Black Dog Vineyard CMS
Basic page content can be edited via the CMS administration, located at 
https://bd-vineyard.netlify.com/admin/

### Collections
![Colletions](https://raw.githubusercontent.com/ilikerobots/bd_vineyard/master/readme_images/Screenshot_bd_collections.png)
There are three collections of site content:
 - **Mandatory Pages**: Pages that cannot be deleted.  Currently only the welcome page.
 - **Pages**:  Pages that may be added/deleted as desired
 - **Blogs**: Special category of pages, that are automatically included in the "News and Updates" section

### Editing a Page
After clicking the "Pages" collection, the current pages displayed on the site are listed.  Click one to open the editing interface.

The resulting page is divided into two panes.  On the left is the editing interface and on the right is the content preview.  The preview is not an exact representation of how content will look on the site.
![Editing](https://raw.githubusercontent.com/ilikerobots/bd_vineyard/master/readme_images/Screenshot_bd_edit_interface.png)

Each of the text fields can be edited on the left pane as desired.  Some fields, such as the **Body**, are "Rich Text" which allows the use of a text formatting editor with buttons for making bold/italic text, links, images, etc.
![Rich Text Editor](https://raw.githubusercontent.com/ilikerobots/bd_vineyard/master/readme_images/Screenshot_bd_markdown_editor.png)


#### Page field descriptions
Most fields are optional.  Required fields are in bold. If you're unsure of what field controls which text, open up a browser window of the site and compare.

 - **Title**: The document title used in search engines and browser tab names
 -  **Header**: The title displayed on the page itself
 - **Permanent Link**: the page name used in the URL, e.g. "mynewpage.html"
 - **Body**: The main content of the page
 - Pre-body intro: Intro teaser title before the main content of the page
 - **Layout**: Either no side columns, or a left- or right-side column
 - **Icon**: The shaded grey icon near the pre body intro.  Choose an icon name from https://faicons.com/
 - Sidebar: If the left- or right-hand column layouts are used, then this field control the content.  This field is itself a list of callout boxes items:
   -  Header: Callout box header
   - Description: Callout box description
   - CTA: The button text
   - Image: An image to show in the callout
   - Link: If a CTA is provided, then clicking will take to this page (should match to a "Permanant Link" of another page"
 - Row Sections:   Another set of optional callout items beneath the page content
   -  Header: Callout box header
   - Description: Callout box description
   - CTA: The button text
   - Link: If a CTA is provided, then clicking will take to this page (should match to a "Permanant Link" of another page"

#### Publishing
When page changes are complete, click the "Publish" button in the top right, then "Publish Now".  Changes will take ~30-60s to be visible on the site.
![Rich Text Editor](https://raw.githubusercontent.com/ilikerobots/bd_vineyard/master/readme_images/Screenshot_bd_publish_button.png)

### Editing a Blog Post
After clicking the "Blogs" collection, the current blog posts are listed.   From this page, editing a blog post is a similar process to editing a Page.  

#### Fields
 - **Title**: The document title used in search engines and browser tab names
 -  **Header**: The title displayed on the page itself
 - **Description**: Used as the "teaser" text in the list of Blogs
 - **Publish Date**: The date and time when this post should become visible.  Note you still need to publish via the top right button.  Set this date a few hours in the past to make it visible immediately. 
 - **Body**: The main content of the page 

### Adding a Blog Post
After clicking the "Blogs" collection, the current blog posts are listed.  Choose "New Blog" button.  Add content to each of the fields above.  Publish.

![New Blog](https://raw.githubusercontent.com/ilikerobots/bd_vineyard/master/readme_images/Screenshot_bd_new_blog.png)


### Editing the Welcome Page
The "Welcome" page cannot be deleted, and has a different set of fields than the other pages.   The best way to edit this page is to view the site, take note of the text you wish to edit, then open up the admin interface, choose the "Welcome" page, then scroll through the fields until you find the text you wish to edit.  Make your changes and Publish as with a normal page.


## Developer notes: 

### Generating static map
``` 
https://maps.googleapis.com/maps/api/staticmap?center=39.558789,-87.254057&size=1200x800&zoom=8&scale=2&markers=icon:https://www.likealocalguide.com/static/fraktal/images/map_point_red.png|39.558789,-87.254057&feature:administrative%7Csaturation:-100&style=feature:administrative.province%7Cvisibility:off&style=feature:landscape%7Csaturation:-100%7Clightness:65%7Cvisibility:on&style=feature:poi%7Csaturation:-100%7Clightness:50%7Cvisibility:simplified&style=feature:road%7Csaturation:-100&style=feature:road.arterial%7Clightness:30&style=feature:road.highway%7Cvisibility:simplified&style=feature:road.local%7Clightness:40&style=feature:transit%7Csaturation:-100%7Cvisibility:simplified&style=feature:water%7Celement:geometry%7Chue:0xffff00%7Csaturation:-97%7Clightness:-25&style=feature:water%7Celement:labels%7Csaturation:-100%7Clightness:-25
```
