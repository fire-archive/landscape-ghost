## Landscape theme for Ghost

Landscape for Ghost is based on our Landscape WordPress theme by BlankThemes.com: http://wordpress.org/themes/landscape

## Copyright & License

Designed and developed by BlankThemes.com.
Copyright (c) 2014 BlankThemes.com - Released under the GPL License.

Header image by Ansel Adams and is licensed under the Public Domain:
http://commons.wikimedia.org/wiki/File:Adams_The_Tetons_and_the_Snake_River.jpg


## How to install Landscape

Ghost themes live in `content/themes/`
After you have downloaded Landscape, extract it and place it in content/themes alongside the Casper default theme.

To switch to your newly added theme:

 * Restart Ghost. At the moment, Ghost won't notice that you've added a new folder to content/themes so you'll need to restart it

 * Login to your Ghost admin, and navigate to `/ghost/settings/general/`

 * Select your Theme name in the 'Theme' options dropdown

 * Click 'Save'

 * Visit the frontend of your blog and marvel at the new theme

If you are new to using Ghost, we recommend checking out the following:
 * Ghost Guide: http://docs.ghost.org/
 * Switching Themes: http://docs.ghost.org/themes/
 * Publishing with Ghost: http://docs.ghost.org/usage/writing/

## Editing the Main Menu

If you are using Landscape for your personal blog, the only file you need to edit is the default.hbs file. This is the file that contains code for your menu. You can edit the links to point to your pages or remove the menu entirely. The code to look for is the following:

`
<div id="menu">
<nav role="navigation" class="site-navigation main-navigation">
    <h1 class="assistive-text">Menu</h1>
    <div class="menu-main-container">
    <ul id="menu-main" class="menu">
    <li><a href="{{@blog.url}}">Home</a></li>
    <li><a href="#">Level 1</a>
        <ul class="sub-menu">
            <li><a href="#">Level 2b</a></li>
            <li><a href="#">Level 2a</a>
            <ul class="sub-menu">
                <li><a href="#">Uncategorized</a></li>
            </ul>
            </li>
        </ul>
    </li>
    <li><a href="#">About The Tests</a></li>
    <li><a href="#">Sample Page</a></li>
    </ul>
    </div>
</nav><!-- .site-navigation .main-navigation -->
</div><!-- #menu -->`
`

## Setting up Comments with Landscape and Ghost

You'll need to use a third party service like Discuss to have comments on your site. With that, you'll need to setup up an account with Discuss.com. Once you have done that, the following instructions will help you integrate Discuss with Landscape.

http://ghost.pellegrom.me/adding-disqus-comments-to-ghost/


## Credit Links

Landscape is GPL licensed. While we appreciate you keeping our credit links intact, this is not required. Simply find the following code in the default.hbs file and edit however.

`
<footer class="site-footer">
    <a class="subscribe icon-feed" href="{{@blog.url}}/rss/"><span class="tooltip">Subscribe!</span></a>
    <div class="inner">
         <section class="copyright">&copy; {{date format="YYYY"}} <a href="{{@blog.url}}/">{{@blog.title}}</a> &bull; Landscape Theme by <a href="http://blankthemes.com">Blank Themes</a></section>
         <section class="poweredby">Proudly published with <a class="icon-ghost" href="https://ghost.org">Ghost</a></section>
    </div>
</footer>
`

## Support

To report possible theme issues, you can contact us at BlankThemes.com.


