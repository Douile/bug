# Bug report
[Bugzilla report](https://bugzilla.mozilla.org/show_bug.cgi?id=1598500)
## Steps to reproduce
1pre. Delete canvas permission rules for the domain you are using
1. Open two (or more) tabs (in the same domain) both of which will request permission to extract canvas data (e.g.  https://douile.github.io/bug/firefox.70.0.1/canvasPermission/)
2. Open the canvas prompt in both tabs without accepting or denying (press X button)
3. In one of the tabs decline the permission request by pressing the canvas permission icon
4. Switch to the other tab and observe the canvas permission icons
## What happened
In the second tab there are two canvas permission prompt icons, one where the permission is denied (line through) and another where the permission has not been accepted yet.
(Clicking the icons will remove the additional one)
## What should have happened
The URL bar of the second tab should've updated removing the old permission icon
