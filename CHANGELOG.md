# angular-tag-cloud changelog

## v0.3.4 (19/12/2017)
 - Fix - not forcing to add click function
 - Add the ability to pass the weights into the component.
   (to make sure that words not overlapping because of custom css)   
 
## v0.3.3 (24/01/2017)
- Expose "afterCloudRender" function call to user (on-rendered attribute).
- Fix - run afterCloudRender.call() only after cloud render .(instead on before and after) . [yonatan20](https://github.com/yonatan20).

## v0.3.2 (22/01/2017)
- Expose the "delayed-mode" to user.
- Removed redundant Second call for drawing the words. [yonatan20](https://github.com/yonatan20).

## v0.3.1 (06/11/2016)
- Added the minified version. By [Ashok](https://github.com/ashokyadav006).

## v0.3.0 (25/04/2016)
- Added `href` support to tags. Use `link` property on tag object to specify link value.

## v0.2.5
- Added binding support. By [hazemhagrass](https://github.com/hazemhagrass).

## v0.2.0
- Added `overflow` option.
- Changed license to MIT
- npm installation guide

## v0.1.0
- Basic options: height, width.
- Custom `css` styling support
