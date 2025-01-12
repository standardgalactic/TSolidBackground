
# **TSolidBackground**  

TSolidBackground allows you to immerse in a window completely by creating a solid overlay over the window borders and around the window.  
In a different saying, it tries to mimic fullscreen for any window without resizing it.  

At first, I made TSolidBackground to prevent myself from getting distracted while playing VNs and later added more features that were useful for me.  

**Default Hotkeys:** *(All hotkeys and many more options can be changed in the .ini)*  

    TSolidBackground hotkey: !T (! represents the Alt key on your keyboard. Read the hotkey guide below.)
    Always On Top: !Y
    Center window: !G
    Show/Hide taskbar: !F
    Advanced Options: !U
    Suspend all other hotkeys: !F8
    Default Color: 250000 (hex value without the #)

**✅ If you are planning to use TSolidBackground, you should also read 'Things to Know' below.**  

### [Webm Preview](https://raw.githubusercontent.com/Onurtag/TSolidBackground/gh-pages/Preview/TSolidBackground%20Preview.webm)  
### [Get latest relese*](https://github.com/Onurtag/TSolidBackground/releases)  

*Compiled using the latest Ahk2Exe. The file is not compressed so you can check the source code easily.  

--------------------  
## 🌟 Things To Know  

* If no hotkeys work on the active/selected window, run TSolidBackground as admin.  
If they still don't work try enabling Keyboard Hook on the Advanced Options menu.  

* TSolidBackground.ini file will be created when you create a .ini using the Advanced Options (default **Alt+U** key).  
After creating the .ini file you can edit it using a text editor to change the hotkeys and many more options.  
You can also quickly edit the .ini by using the "Edit TSolidBackground.ini" button in the tray menu.  
**[QUICK HOTKEY EDITING GUIDE.png](https://github.com/Onurtag/TSolidBackground/raw/gh-pages/images/Hotkey%20Guide.png)**  
[Advanced hotkey Guide 1](https://autohotkey.com/docs/Hotkeys.htm), [Guide 2](https://www.autohotkey.com/docs/KeyList.htm)

* If you want to disable a hotkey you can do it by leaving the related variable empty in the TSolidBackground.ini.  

* You have to select the window (make it active) before using most hotkeys.  

* You can change the background color using the Advanced Options menu in the Advanced Features menu (default hotkey: Alt+U).  
You can press the **[R]** button to switch between red and blue.  

* When you are on the Move/Resize Window menu, you can use the Advanced Features (default: Alt+U) hotkey to get a new window to move/resize.  

* If your window doesn't show up on the Move/Resize dropdown menu, you can try editing the excluded windows list using the **Edit** button in the Advanced Options menu.  
When this option is enabled, the TSolidBackground Move/Resize menu dropdown will not list all the windows that don't have a title in addition to all the windows that are listed in the above menu.  

* Always on top mode can be used for multiple windows at the same time.  
Exiting or reloading in any way like using the notification icon menu (right click - exit) will fix your windows if you left them in the always on top mode.  

* Using the TSolidBackground function will disable always on top if the selected window is always on top.  
You can use the always on top hotkey afterwards if you really want the window on top.  

* Experimental window hooking currently works like this:  
After Hooking Main Window(or browser tab) to the Hooked window, the hooked window will stay always on top when that tab/window is currently active. When you change tabs/go to a different window it will minimize and when you go back it will be on top again. You can also stop the window hooker using the tray icon menu.  

* You can use [this script](https://pastebin.com/DdTkfjdM) to make a window transparent or clickthrough.  

--------------------  
**Known Issues:**  

* Hiding taskbar sometimes might not work right away on slow computers, try it again.  
* Explorer.exe might crash and restart if you spam the hotkeys too much (Especially Show Hide taskbar key).  
It might also crash if you try to resize a window smaller than allowed etc.  

If you have any other problems, [open an issue](https://github.com/Onurtag/TSolidBackground/issues). I'll try to fix it.  


--------------------  
## Changelog

>**Legend:**  
>🔁 Change  
>✅ Fix/Improvement  
>➕ Addition  
>❌ Removal  

* **Version 2.9.16**  

🔁 Change the default "Suspend All Hotkeys" key from F8 to Alt+F8 (!F8)  
✅ Fix a bug where it was not possible to modify the "Suspend All Hotkeys" hotkey.  
✅ Fix a bug where the location of TSolidBackground.ini was not consistent.  
➕ Refactor Window Hooker (Alpha) logic and add some minor features (these do not show up on the GUI yet)  

* **Version 2.9.15**  

✅ Update notification popups library

* **Version 2.9.14**  

✅ Switch notification popups with a better looking library  

* **Version 2.9.13**  

➕ Added Ctrl/Shift speed modifiers to MouseMover  
✅ Updated the Exit code  

* **Version 2.9.11**  

➕ Added three hotkeys to Move/Resize a specific window quickly. You will have to choose and enable the hotkeys manually in the .ini. 

* **Version 2.9.10**  

➕ Added an option to disable partial window title hooking on the Window Hooker menu.  

* **Version 2.9.9**  

➕ Added an option to enable Keyboard Hook for when the hotkeys don't work on a window.  

* **Version 2.9.8**  

➕ Added a "TSB this window" button into the Move/Resize menu.  
❌ Disabled the "Got a new window to move/resize" and "Got a new window for tsolidbackground" popups  

* **Version 2.9.7**  

✅ Small window hooker improvements.  

* **Version 2.9.6**  

✅ Small gui fixes.  
✅ Fixed the encoding problem of the updater.  

* **Version 2.9.4**  

✅ Fix for higher dpi scaling settings.  
✅ Bug fix for file encoding problems.  
✅ Fixed a 1 pixel border which was visible on the top while using TSolidBackground.  

* **Version 2.9.3**  

✅ Gui optimizations.

* **Version 2.9.2**  

Fixed all client size calculations.

* **Version 2.9.1**  

Handled some exceptions and fixed some tooltips.

* **Version 2.9.0**  

Changed default modifier to alt (! instead of +), changed default color to red (250000 instead of 051523).
Fixed mouse mover bugs.

* **Version 2.8.7**  

Added a menu to customize excluded titles.  
Added a C (Copy Window Title) button to move/resize menu to help with above.  
Added middle click to mouse mover.  

* **Version 2.8.6**  

Added more Numeric UpDowns so we can all use our scroll wheels.  
Added Minimize/Restore Window, Maximize Window and Close Window buttons to the Move/Resize menu.  
Added various tooltips using the AddToolTip library.  
Better VNR (Kagami) protection.

* **Version 2.8.5**  

Corrected a mistake.

* **Version 2.8.4**  

Can now exclude system windows & untitled windows from the move/resize dropdown menu. Enabled by default.  
Tiny bug fix.  

* **Version 2.8.3**  

Added clicks to mouse mover.  
Bug fixes.  

* **Version 2.8.2**  

Added mouse mover using keyboard.

* **Version 2.8.1**  

Various bug fixes. (Centering, Multimonitor stuff)

* **Version 2.8.0**  

Full Automatic updater added.  
Ini versions added for easier ini version control. Inis will now last longer.  

* **Version 2.7.2**  

Fixes for the new resize/move selector.  
Esc now goes back to the main menu.  
Named the 4 TSB hidden windows so you can move/resize them using the new resize/move selector.   
Better cheating capabilities.  

* **Version 2.7.1**  

Experimental speed improvements.  
Added a dropdown window selector to resizer menu as an alternative way to select windows. (Thanking xThorpyx for the inspiration)


* **Version 2.7.0**  

Added a way to check for updates in the advanced options menu.  
Added a way to auto check for updates. Make a new .ini and you will see the dialog.  
Added a way to disable a hotkey by leaving the variable empty in the .ini.  
Fixed overlapping checkboxes.  
There are **TSolidBackground.ini changes** in this update. You should delete yours and make a new one.  


* **Version 2.6.4**  

Edit TSolidBackground.ini tray menu button.  
Back button in advanced menus.

* **Version 2.6.3**  

New 3 Permanent custom TSolidBackground size settings.


* **Version 2.6.2**  

Added Debug variable to ini. Setting it to 1 will activate F11 Debug variables hotkey.  
Put some more work into the window hooker (currently Beta).  


* **Version 2.6.0**  

Moving buttons added to advanced move menu.  
"Make a Dummy Window for TSolidBackground" added. Use this to get a custom sized TSolidBackground.  
Ver. 2.6.1: Save dummy to .ini.


* **Version 2.5.1**  

Some cleanup.
Added a different icon for the "Suspended" state (Compiled .exe only). 


* **Version 2.5.0**  

Changed UI fonts to Segoe UI.  
Revamp of Advanced Features (default Alt+U hotkey)  
Added Experimental Window hooking to advanced features (!U).  
*Window hooking currently works like this: After Hooking Main Window(or browser tab) to the Hooked window, the hooked window will stay always on top. When you change tabs/go to a different window it will minimize and when you go back it will be on top again. You can also stop the window hooker using the tray icon menu.* 

* **Version 2.4.4**  

Protect VNR checkbox
	
	
* **Version 2.4.3**  

Fix custom hotkey not changing.
Cleanup useless code

* **Version 2.4.1:**  

Can now save size + position in !U options menu.  
Added reset button for custom TSb.  


* **Version 2.4.0:**  

Finally got my hands on a second monitor and now everything works in multiple monitors.  
Added an [O] button to !U for moving to original position.  
Added U,D,L,R buttons to easily move windows.  

* **Version 2.3.0:**  

Removed old options, moved to (!U)  
Added .ini option to disable startup window.  
Seperated custom width and height, made new temprorary options in (!U).  

* **Version 2.2.2:**  

Added custom sizing option to the .ini and did some other stuff too.

* **Version 2.2.1:**  

Removed useless stuff and added useful stuff.


* **Version 2.2.0:**  

Added features to Move/Resize (Alt+U)


* **Version 2.1.4:**  

Added window client area to resizer


* **Version 2.1.3:**  

Removed useless info.  
Now less casual.  


* **Version 2.1.2:**  

Added resize window function.


* **Version 2.1.1:**  

Fixed bug when using with VNR.


* **Version 2.1:**  

Taskbar hide revamp.  
Added notes to start popup  
Fixed huge bugs.  
New dark color scheme.  


* **Version 2.0:**  

TSolidBackground revamp, now the window borders are gone too! (Thanking biggest_decision for the heads up.)  
Added show/hide taskbar key, removed the command that was included in TSolidBackground key.  
This is probably the final version unless I go bug hunting or get a new feature request.  


* **Version 1.1:**  

Fixed timing issues with slower PC.  
Fixed the bug where the window sometimes went background when using TSolidBackground  
Added tray menu: Reload, About  
Added opening popup with hotkey information.  
Added Suspend hotkeys and Center window functions


--------------------  
## 📦 Included Functions/Libraries

AddTooltip by Various authors  
From https://autohotkey.com/boards/viewtopic.php?&t=30079  

GetMonitorIndexFromWindow() by Shinywong.  
From https://autohotkey.com/board/topic/69464-how-to-determine-a-window-is-in-which-monitor/?p=440355  

GetWindowInfo by "just me"  
From https://autohotkey.com/board/topic/69254-func-api-getwindowinfo-ahk-l/  

StackingPleasantNotify by Onurtag  
A mod of the original PleasantNotify by Soft which was later modded by evilC   
From https://www.autohotkey.com/boards/viewtopic.php?f=6&t=6056#p35696  
