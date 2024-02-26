# FixMAUpopup
A munki nopkg to try to stop Microsoft AutoUpdate bouncing in the doc and confusing users who have munki to patch/update their Microsoft apps.

The script does a check to see if the Microsoft AutoUpdate app is living in /Application Support and exits if it has already been removed.

The post install part of the nopkg had to also be added to each of the Micosoft 365 recipes I have since Word, Excel, etc, reinstall Microsoft AutoUpdate every time - even replacing the locked folders of this fix.

The fix itself was suggested at: https://apple.stackexchange.com/questions/428234/how-to-remove-microsoft-autoupdate-from-macos

Place the plist into your munki repo's pkginfo folder and don't forget to run /usr/local/munki/makecatalogs

Read more about nopkg items at: https://github.com/munki/munki/wiki/nopkgs

## Contributors
* Alex Narvey

—
Alex Narvey
precursor.ca
