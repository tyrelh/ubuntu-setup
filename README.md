# Details about my Ubuntu Setup
This document is more of a reference for myself to keep track of customizations I've made to my Ubuntu install. As I progress and learn more about linux customization I will continue to update this doc.

Feel free to use this as a reference or copy things I've done. Just remember I have no clue what I am doing and am learning some of this as I go.
![Desktop Screenshot](res/desktop.png?raw=true "Desktop Screenshot")
^ Sept 30, 2018

# VS Code

![VS Code Screenshot](res/vscode.png?raw=true "VS Code Screenshot")
^ Sept 30, 2018

Install the `One Dark Pro` theme from app. I am using the `Vivid` version.

Search filesystem for `OneDark-Pro.json`. Edit that or the vivid version (whichever you're using) so the title bar matches the other bars and charm(activity) bar to be darker rather than lighter (maybe could add this to `settings.json`?):
* `"activityBar.background": "#1E2127",`
* `"titleBar.activeBackground": "#21252B",`

In `settings.json` add this line to darken the editor background color:
```
"workbench.colorCustomizations": {
    "editor.background": "#191d22",
}
```
In the version I have as of writing this, `1.27.2`, add this line to `settings.json` to enable the new title bar on Linux:
```
"window.titleBarStyle": "custom",
```
* The new title bar will soon be default in an upcoming update.

I also have the `Material Icon Theme` extension installed for the nice file icons in the directory listing.

# Hyper
Install `hyper-snazzy` theme in the plugins section of `~/.hyper.js`.

I have just recently started using `Hyper` so I have yet to customize it's functionality apart from using `ZSH` and the above theme.

# ZSH
## OhMyZSH
* TODO
## Powerline
* TODO
* Powerline font

# Gnome
Install `Gnome Tweaks` from Software Center. 
## Themes
* `X-Arc-Shadow` (applications)
* `Capitaine-cursors` (cursor)
* `Arc-X-D` (icons)
* `X-Arc-Shadow` (shell)
    * In the theme css (`~/.themes/X-Arc-Shadow/gnome-shell/gnome-shell.css`), change the global `stage` font to be `Product Sans`, leaving the default backups.
* `Product Sans` (all fonts except mono)
    * https://befonts.com/product-sans-font.html
## Extensions
Install the Firefox extensions from https://extensions.gnome.org/ to easily install gnome extensions from there.
* User themes
    * May be installed by default. Allows for additional user themes.
* Dynamic Panel Transparency
    * Maximized color: `#1F2227`
    * Unmaximized color: full-transparent
* Frippery move clock
    * Move clock to right side of panel.
* Hide activities button
* Openweather
    * Add weather to panel.

# Future
One of the main things I haven't tried full-time yet is a tiling window manager to replace gnome. I've been looking into i3 but just haven't taken the plunge yet.