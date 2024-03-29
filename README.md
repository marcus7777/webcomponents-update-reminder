# Webcomponents-update-reminder
Remind your user to update your components just by adding one line

## Get start
To use this element in your components:
```
<!-- import this element just like you do to other web components -->
<!-- you can add async tag to this as it won't effect the render of the page -->
<link rel="import" href="../webcomponents-update-reminder/webcomponents-update-reminder.html" async>

<!-- adding this inside your web component -->
<webcomponents-update-reminder
    repo="YOUR ELEMENT'S GITHUB REPO, FOR EXAMPLE: PolymerElements/paper-toolbar">
</webcomponents-update-reminder>
```
That's all! When your component have a new version, the user will recieve a info like this:

![a info in console](https://raw.githubusercontent.com/markhuang1212/webcomponents-update-reminder/master/info.JPG)

The element will read your repo's `release tag` and compare it with the local `bower.json` to detect if there is a new version, **only minor and major version update will remind user to update (unless your element's major version is 0)**. Your user will recieve a message in console when developing on `localhost` or `127.0.0.1`.

You need to mention that the `version` tag in your `bower.json` should be look like `X.Y.Z`,  the `release tag` in your github repo should be look like `vX.Y.X` or `X.Y.Z`. We recommend naming tags that fit within [semantic versioning](http://semver.org/).

## Let's build together!
This element is still building. If you're interested in it, you can help building it together!
