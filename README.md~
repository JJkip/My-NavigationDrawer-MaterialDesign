# My-NavigationDrawer-MaterialDesign
This is a sample app which implements Material Drawer based on [Navigation drawer (library)](https://github.com/rudsonlive/NavigationDrawer-MaterialDesign) by [rudsonlive](https://github.com/rudsonlive).

I have however improved it to run on as low as API level 8. In my case there were two places that were making the library not to run on API lower than 14. So I made the following changes:

### 1. NavigationLiveoAdapter

On the setAlpha function, I replaced
```
        v.setAlpha(alpha); and v.setAlpha(1f);
```

with

```
        ViewHelper.setAlpha(v, alpha); and ViewHelper.setAlpha(v, 1f);
```


I replaced v.setAlpha() method with ViewHelper.setAlpha() in [NineOldAndroids](http://nineoldandroids.com/)


### 2. FragmentMain

On the onCreateOptionsMenu method I replaced 

```
        final MenuItem menuItem = menu.findItem(R.id.menu_search);
        menuItem.setVisible(true);

        SearchView searchView = (SearchView) menuItem.getActionView();
        searchView.setQueryHint(this.getString(R.string.search));
```

with

```
        SearchView searchView = (SearchView) MenuItemCompat.getActionView(menu.findItem(R.id.menu_search));
        searchView.setQueryHint(this.getString(R.string.search));
```

**For acknowledgement and respect of his work, the license still remain**
