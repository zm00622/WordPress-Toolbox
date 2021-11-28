# WordPress-Toolbox

## Add Custom Page

https://www.quora.com/How-do-you-create-a-custom-PHP-page-in-WordPress

A custom page allows you to have different layout, look and feel from regular pages in WordPress. You can even have it work as full fledged PHP page which is what you want right?

Here is what you should do:

Create a page call it my-custom-page.php and save it under your theme directory.
Now, edit this php file and write the following line at the top of the page
<?php /* Template Name: My Custom Page */ ?>
Write your PHP code under the custom page definition line, you can call your other WP template, functions inside this file.
Start like
<?php require_once("header.php");?> or whatever way you are integrating your header and footer to keep the layout consistent.
Since this is a custom page, you NEED TO CREATE A PAGE from WordPress admin panel.
Go to Admin => Pages => Add New
Add a page title, depending upon how you have coded the custom page, you might add page body (description) as well. You can fully skip the description if it’s written in the custom php page.
At right hand side, select Template.
Choose My Custom Page from the dropdown.
You are all set! Go to the slug (permalink) created by wordpress and see the page.
