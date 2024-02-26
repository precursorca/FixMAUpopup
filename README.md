# FixMAUpopup
A munki nopkg to stop Microsoft AutoUpdate bouncing in the doc and confusing users who have munki to patch/update their Microsoft apps.

The post install part of the script had to be added to each of the Micosoft 365 recipes I have since Word, Excel, etc reinstall Microsoft AutoUpdate every time - even replacing the locked folders of this fix.

The fix itself was suggested at: https://apple.stackexchange.com/questions/428234/how-to-remove-microsoft-autoupdate-from-macos


