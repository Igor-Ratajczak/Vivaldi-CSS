# Vivaldi-CSS

## New UI for Vivaldi

* Tab bar with auto-hide
* Search on center
* More animations
* Remove Reader View from address bar

## Problems

### Bookmarks & Status Bar

When both the **Bookmark Bar** and **Status Bar** are enabled, they overlap in the same space.  
As a result, the **Status Bar becomes unclickable** because is under of **Bookmark Bar**.

## Screenshots

### Startpage

![Screenshot of a startpage](/screenshots/startpage.png)

### Address Bar

![Screenshot of a address bar](/screenshots/tab_bar.png)

### Search

![Screenshot of a search](/screenshots/search.png)

### History

![Screenshot of a history](/screenshots/history.png)

### Floating panel on

![Screenshot of a floating panel on](/screenshots/floating_panel_on.png)

### Floating panel off

![Screenshot of a floating panel off.](/screenshots/floating_panel_off.png)

## How to use it?

1. Go to **vivaldi://experiments** enable **Allow CSS modification**
2. Download *style.css* and put in new folder e.g. vivaldi
3. In settings go to **Appearance** find **Custom UI Modifications** and select folder with *style.css*
4. The screenshots use the theme Purple Haze by resdek. You can download it from Vivaldi themes.
5. Reboot browser

## Your changes

### Change background

1. Paste your picture in **vivaldi/Default/VivaldiThumbnails/**
2. In **`style.css`**  
   * Locate the following line of code:  

     ```css
     chrome://vivaldi-data/thumbnail/O3CNZC67HXCG6MMASH7YCHCIJUNBQMLE.jpg
     ```

   * Replace it with:  

     ```css
     chrome://vivaldi-data/thumbnail/YourIconName
     ```

3. Save, reboot browser and have fun!

### Reader View

If you want reader view on address bar. Remove this code from *style.css*

```css
/*  Remove reader view */
div.button-toolbar:has(button.ToolbarButton-Button[aria-label='Reader View']) {
    display: none;
}
```
