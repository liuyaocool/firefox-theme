# firefox-thtme

# install

1. browser `about:support`
2. set `toolkit.legacyUserProfileCustomizations.stylesheets=true`




# about firefox

## config left

see `https://support.mozilla.org/zh-CN/kb/%E7%AE%A1%E7%90%86%E7%94%A8%E6%88%B7%E9%85%8D%E7%BD%AE%E6%96%87%E4%BB%B6#w_start-the-profile-manager-when-firefox-is-closed`

run `firefox -P` to re init

# guess window source code

## tab bar

```html
<div id="">


</div>
```

## url bar

```html
<div id="nav-bar">
    <div id="nav-bar-customization-target">
        <div id="urlbar-container">
            <div id="urlbar">
                <div id="urlbar-background">
                <div id="urlbar-input-container">
                    <div class="urlbar-input-box">
                        
                    </div>
                </div>
            </div>
        </div>
    </div>    
</div>
```


?? 
``` css
#urlbar[breakout][breakout-extend] > #urlbar-input-container,
.urlbar-page-action
#urlbar[breakout][breakout-extend][open]
#wrapper-urlbar-container
#urlbar-go-button
#urlbar .urlbarView-body-inner
#urlbar:not(.megabar):not([focused="true"]),
#urlbar:not(.megabar):not([focused="true"]):hover {
  border-bottom: transparent;
}
.urlbarView:not([noresults]) > .search-one-offs:not([hidden]) {
  border-top: none !important;
}
/* Megabar */
#urlbar[breakout] {
  height: auto !important;
}

```
