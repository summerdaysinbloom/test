# How to get started

This application is built with **grunt**, you may want to follow this :

1. Install project dependencies : `npm install`.
1. Run `grunt` 
1. Run `grunt watch for automatically compress `less/*.less` and `js/*.js` and update `assets.css` and `assets.js`


# gruntfile.js and package.json

For the security reason, I couldnt attach `gruntfile.js` and `package.json` directly. So I add a `gruntfile.md` and `package.md`. If you want to excute this file properly, please copy this :

1. `gruntfile.md` and create a file name as `gruntfile.js` then it will works.
2. `package.md` and create a file name as `package.json` then it will works.

# Editing content page 

I added a guideline page, you can easily get it to use just **copy** and **paste** since it includes specific html structure. Locally, you just visit `/guideline.html`

## Contents section

### structure of content page 

Each content section has same structure below: 

	<div class='span9'>
        <div class='wrapper'>
          <h1>Partners</h1>
          <div id='content' class='content mCustomScrollbar _mCS_1' >
          
          …
          
          </div>
        </div>
    </div>

`h1` is a page title, which is a static part of page. 

`div#content` or `div.content` is a real content section, which includes scroll bar : 

`mCustomScrollbar _mCS_1` is for the scroll bar. Do not change this part, otherwise it will not work properly.


Basically, it has `title` ,`category-frame`, `category-title` + `category`, `category-list`, `p`, `span` and `link`.

### Title. 

	<h2><i class='icon-comments-alt'></i>Title with h2 tag</h2>
    <!-- Title h2 without icon -->
    
    <h2>Title with h2 tag, w/o icon</h2>
    <!-- Title h3 without icon -->
    
    <h3>Title with h3 tag</h3>
    <!-- Title h4 without icon -->
    
    <h4>Title with h4 tag</h4>
    
It supports **h2**,**h3**,**h4** and with or w/o icon.
Add this line for adding icon : `<i class='icon-comments-alt'></i>`. You can also choose your icon from [here](http://fortawesome.github.io/Font-Awesome/icons/).

### category frame

It includes padding amd background. Every **H**, **P**, **span** and **a** tag are be part of category frame. 

### category list

 	 <div class='category-list'>
       <h3><i class='icon-reorder'></i>List title </h3>
       <div class='list-info'>Additional informaion or details only for list: </div>
       <ul>
         <li><i class='icon-ok'></i>list1</li>
         <li><i class='icon-ok'></i>list item with <a href='#' target='_blank'>links</a> , Etiam sed massa felis, aliquam   pellentesque est.</li>
         <li><i class='icon-ok'></i>list1</li>
       </ul>
     </div>