# WordPress-Menu-HTML

Here is the output HTML from WordPress default `wp_nav_menu` function


```
<nav id="site-navigation" class="main-navigation" role="navigation">
    <button class="menu-toggle">Menu</button>
    <a class="assistive-text" href="#content" title="Skip to content">Skip to content</a>
    <div class="menu-container"> <!-- Do not  use this class for styling -->
        <ul id="menu-short" class="nav-menu"> <!-- Use this class for styling -->
            <li id="menu-item-9468" class="nav-item menu-item menu-item-type-custom menu-item-object-custom menu-item-9468"><a href="http://wpthemetestdata.wordpress.com/">Home</a></li>
            <li id="menu-item-9667" class="nav-item menu-item menu-item-type-post_type menu-item-object-page menu-item-9667"><a href="http://192.168.0.90/themes-dev/about/">About</a></li>

            <li id="menu-item-9668" class="nav-item menu-item menu-item-type-post_type menu-item-object-page menu-item-has-children menu-item-9668"><a href="http://192.168.0.90/themes-dev/parent-page/">Parent Page</a>
                <ul class="sub-menu">
                    <li id="menu-item-9843" class="menu-item menu-item-type-post_type menu-item-object-page menu-item-9843"><a href="http://192.168.0.90/themes-dev/parent-page/child-page-01/">Child Page 01</a></li>
                    <li id="menu-item-9844" class="menu-item menu-item-type-post_type menu-item-object-page menu-item-9844"><a href="http://192.168.0.90/themes-dev/parent-page/child-page-02/">Child Page 02</a></li>
                    <li id="menu-item-9845" class="menu-item menu-item-type-post_type menu-item-object-page menu-item-9845"><a href="http://192.168.0.90/themes-dev/parent-page/child-page-03/">Child Page 03</a></li>
                    <li id="menu-item-9672" class="nav-item menu-item menu-item-type-post_type menu-item-object-page menu-item-9672"><a href="http://192.168.0.90/themes-dev/parent-page/child-page-04/">Child Page 04</a></li>
                    <li id="menu-item-9671" class="nav-item menu-item menu-item-type-post_type menu-item-object-page menu-item-has-children menu-item-9671"><a href="http://192.168.0.90/themes-dev/parent-page/child-page-05/">Child Page 05</a>
                        <ul class="sub-menu">
                            <li id="menu-item-9673" class="nav-item menu-item menu-item-type-post_type menu-item-object-page menu-item-9673"><a href="http://192.168.0.90/themes-dev/parent-page/child-page-03/grandchild-page/">Grandchild Page</a></li>
                            <li id="menu-item-9842" class="menu-item menu-item-type-post_type menu-item-object-page menu-item-9842"><a href="http://192.168.0.90/themes-dev/parent-page/child-page-03/grandchild-page/">Grandchild Page</a></li>
                        </ul>
                    </li>
                </ul>
            </li>
        </ul>
    </div>
</nav>
```


## Menu Item CSS Classes #Menu Item CSS Classes

The following classes are applied to menu items, i.e. to the HTML <li> tags, generated by wp_nav_menu():
#### All Menu Items #All Menu Items



```css
.menu-item
```
This class is added to every menu item.

```css
.menu-item-has-children
```
This class is added to menu item which has sub-items .

```css
.menu-item-object-{object}
```
This class is added to every menu item, where {object} is either a post type or a taxonomy.

```css
.menu-item-object-category
```
This class is added to menu items that correspond to a category.

```css
.menu-item-object-tag
```
This class is added to menu items that correspond to a tag.

```css
.menu-item-object-page
```
This class is added to menu items that correspond to static pages.

```css
.menu-item-object-{custom}
```
This class is added to menu items that correspond to a custom post type or a custom taxonomy.

```css
.menu-item-type-{type}
```
This class is added to every menu item, where {type} is either “post_type” or “taxonomy”.

```css
.menu-item-type-post_type
```
This class is added to menu items that correspond to post types: i.e. static pages or custom post types.

```css
.menu-item-type-taxonomy{}
```
This class is added to menu items that correspond to taxonomies: i.e. categories, tags, or custom taxonomies.






## Current-Page Menu Items #Current-Page Menu Items

```css
.current-menu-item{}
```
    This class is added to menu items that correspond to the currently rendered page.


## Current-Page Parent Menu Items #Current-Page Parent Menu Items


```css
.current-menu-parent{}
```
This class is added to menu items that correspond to the hierarchical parent of the currently rendered page.
    
```css
.current-{object}-parent
```
This class is added to menu items that correspond to the hierachical parent of the currently rendered object, where {object} corresponds to the the value used for .menu-item-object-{object}.

```css
.current-{type}-parent
```
This class is added to menu items that correspond to the hierachical parent of the currently rendered type, where {type} corresponds to the the value used for .menu-item-type-{type}.



## Current-Page Ancestor Menu Items #Current-Page Ancestor Menu Items


```css
.current-menu-ancestor
```
This class is added to menu items that correspond to a hierarchical ancestor of the currently rendered page.

```css
.current-{object}-ancestor
```
This class is added to menu items that correspond to a hierachical ancestor of the currently rendered object, where {object} corresponds to the the value used for .menu-item-object-{object}.

```css
.current-{type}-ancestor
```
This class is added to menu items that correspond to a hierachical ancestor of the currently rendered type, where {type} corresponds to the the value used for .menu-item-type-{type}.



## Site Front Page Menu Items #Site Front Page Menu Items


```css
.menu-item-home
```
This class is added to menu items that correspond to the site front page.


Top ↑
## Backward Compatibility with wp_page_menu() #Backward Compatibility with wp_page_menu()

The following classes are added to maintain backward compatibility with the [[Function Reference/wp_page_menu|wp_page_menu()]] function output:


```css
.page_item
```
This class is added to menu items that correspond to a static page.
    
```css
.page_item_has_children
```
This class is added to menu items that have sub pages to it.

```css
.page-item-$ID
```
This class is added to menu items that correspond to a static page, where $ID is the static page ID.

```css
.current_page_item
```
This class is added to menu items that correspond to the currently rendered static page.

```css
.current_page_parent
```
This class is added to menu items that correspond to the hierarchical parent of the currently rendered static page.

```css
.current_page_ancestor
```
This class is added to menu items that correspond to a hierarchical ancestor of the currently rendered static page.







