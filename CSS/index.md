# CSS Styleguide

## File structure

In the end, there should be only one css file, compressed for production mode or extended for development purposes.
This file is typically named `main.css` or `app.css`,

`main.scss` has the following contents:
```

// Project's custom settings 
@import "settings";

// Framework's settings
@import "<extra-framework>/<settings-file>":

// for bootstrap framework
// @import "bootstrap/variables";
// or for foundation framework
// @import "foundation/settings";

// Import framework's main sass file

@import "<extra-framework>";

// Project's sass file
@import "global";

```

`_global.scss` imports all the projects partial sass files 
like `_footer.scss` or `_navigation.scss`. These files should  be imported in alphabetical order.

Example of `_global.scss` file:
```
@import "footer";
@import "modals";
@import "tables";
```

