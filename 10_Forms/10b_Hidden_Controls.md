# 10b Hidden controls

## Video

* [Short Video for this page](https://mwsu.hosted.panopto.com/Panopto/Pages/Viewer.aspx?id=6ff3ad85-2dd7-4f0a-8041-ab8c00150880)

## Hidden

The input type "hidden" may seem odd at first.  It is considered a control, but the user does not see it.

It is very useful for passing arguments that an api may require, but which do not need to be specified in this situation.

The value in hidden fields is not shown to the user, but it is not exactly secret.  The user can see the value when they view the source.

```html
        <label>Height:</label> <input type="text" name="feet">ft. <input type="text" name="inches">in.
        <input type="hidden" name="units" value="english"
```
