# twShowdown
Live Preview your TinyMCE Markdown in Showdown.js with full MathJax support
Works with *twExoticMarkdownEditor.js*

If you are using another library to Parse your published Markdown, say PHP Parsedown Extra, note that Markdown Parsers have syntax flavours, therefore using Showdown (Javascript) might show little differences from your final official output.

##Usage:

```
  tinymce.init({
    external_plugins: {
      twShowdown: "[[++assets_url]]components/tinymcewrapper/tinymceplugins/twShowdown.js", //plugin location
    },
    twShowdownSettings: { 
      (coming soon)... pass in any Showdown official setting you like to overwrite default behaviour
      ... below are proprietary settings
      twShowdownCDNbase: "",
      //twMathJaxDisable: , // use 1 to disable
      twMathJaxURL: "", //defauls to CDN
      twPoppedTitle: "",
      twPopped: 0, // popped (default) or inline
      twPoppedWidth: "",
      twPoppedHeight: "",
      twViewInlineButtonText: "View Inline",
      twCloseButtonText: "Close",
      twInlineHeight: 250
    },
    toolbar: "preview",
    contextmenu: "preview"
});
```
