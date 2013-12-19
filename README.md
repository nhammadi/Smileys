Smileys
=======

A more powerful and customizable emoticons plugin for TinyMCE 4

![](http://oi43.tinypic.com/jv1a48.jpg)

#### How it works

like every tinymce plugin, Smileys must be added in the plugins list then add the smileys button in the toolbar

```js
tinymce.init({
    plugins: "smileys",
    toolbar: "smileys"
});
```

You can disable the auto-conversion of smileys by setting the auto_convert_smileys configuration option to false 

```js
tinymce.init({
    auto_convert_smileys: false
});
```

You can even extend the default smileys list by your own by adding the extended_smileys configuration option to the init function of Tinymce

```js
 tinymce.init({
      extended_smileys:[
      [
          { shortcut: ':-)', url: 'http://www.fbsmileys.com/wp-content/emos/smile.png', title: 'smile' },
          { shortcut: 'O:)', url: 'http://www.fbsmileys.com/wp-content/emos/angel.png', title: 'angel' },
          { shortcut: 'o.O', url: 'http://www.fbsmileys.com/wp-content/emos/confused.png', title: 'confused' },
          { shortcut: '3:)', url: 'http://www.fbsmileys.com/wp-content/emos/devil.png', title: 'devil' },
          { shortcut: ':-O', url: 'http://www.fbsmileys.com/wp-content/emos/gasp.png', title: 'gasp' },
          { shortcut: '8-)', url: 'http://www.fbsmileys.com/wp-content/emos/glasses.png', title: 'glasses' },
          { shortcut: ':-D', url: 'http://www.fbsmileys.com/wp-content/emos/grin.png', title: 'grin' }
      ]
      ]
});
```

#### Features 
- The user can override the default smileys icons by his own in the tinyMCE init function
- Convert smileys shortcuts to the appropriate icons instantly

####Initialization Example

```js
<script type="text/javascript">
    tinymce.init({
      selector: "textarea",
      theme: "modern",
      plugins: ["smileys"],
      toolbar1: "smileys",
      smileys:[
      [
          { shortcut: ':-)', url: 'http://www.fbsmileys.com/wp-content/emos/smile.png', title: 'smile' },
          { shortcut: 'O:)', url: 'http://www.fbsmileys.com/wp-content/emos/angel.png', title: 'angel' },
          { shortcut: 'o.O', url: 'http://www.fbsmileys.com/wp-content/emos/confused.png', title: 'confused' },
          { shortcut: '3:)', url: 'http://www.fbsmileys.com/wp-content/emos/devil.png', title: 'devil' },
          { shortcut: ':-O', url: 'http://www.fbsmileys.com/wp-content/emos/gasp.png', title: 'gasp' },
          { shortcut: '8-)', url: 'http://www.fbsmileys.com/wp-content/emos/glasses.png', title: 'glasses' },
          { shortcut: ':-D', url: 'http://www.fbsmileys.com/wp-content/emos/grin.png', title: 'grin' }
      ]
      ]
    });
</script>
```
