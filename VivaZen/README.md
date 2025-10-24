# VivaZen THEME

## A Zen-like Experience for Vivaldi

- Auto-hide **tab bar**, **address bar** and **bookmark bar** with any position
- Works with **tab bar** positioned anywhere (left, right, top, or bottom)
- Works with **address bar** and **bookmark bar** positioned on top or bottom
- You can choose what you want auto hide

## ⚠️ IMPORTANT ⚠️

**Window dragging does not work** - This CSS mod disables the ability to drag the browser window by the toolbar or tab bar due to the required `-webkit-app-region: none` property. You can only drag the window using the window title bar.

You can remove `-webkit-app-region: none`, but auto hide can not work property.

## Video/Screenshots

![Video of VivaZen](./screenshots/address-hide.webm)
![Video of VivaZen](./screenshots/bookmark-hide.webm)
![Video of VivaZen](./screenshots/address-bookmark-hide.webm)

## How to use it?

1. Go to **vivaldi://experiments** and enable **Allow CSS modification**
2. Download _VivaZen.css_ and put it in a new folder
3. In settings, go to **Appearance**, find **Custom UI Modifications**, and select the folder with _VivaZen.css_
4. You can use color or image or gif as background
5. Reboot the browser

## Your Settings

### Auto Hide Options

You can set what has auto hide and what hasn't

```CSS
--auto-hide-tab_bar: true;
--auto-hide-address_bar: true;
--auto-hide-bookmark_bar: true;
```

### STYLING FOR ELEMENTS (Default Disabled)

You can set **true** or **false**

```css
--use-theme: false;
```

### Change colors of background

You can change colors here

```css
/* Background Configuration */
--background: linear-gradient(45deg, #000000, #032e17, #06938c, #000000);
--background-size: 100vw 100vh;
--color: #ffffff;
--address-input-shadow: #ffffff21;
```

### Image From Vivaldi Theme Store as Background

1. Find picture in **vivaldi/Default/VivaldiThumbnails/**
2. In **`VivaZen.css`**:

- Change

```css
--background: linear-gradient(45deg, #000000, #032e17, #06938c, #000000);
```

to

```css
--background: url("chrome://vivaldi-data/thumbnail/IconName");
```

### Your Image as Background

1. Paste you image to folder with my mod
2. In **`VivaZen.css`**:

- Change

```css
--background: linear-gradient(45deg, #000000, #032e17, #06938c, #000000);
```

to

```css
--background: url("./YourIconName");
```
