# Checklist for when putting a Wordpress site live

> A running list of things to check before deploying WordPress sites. How do people remember all this?

## Avoid putting a site live on a Friday.

## Development
+ Always use the last version of WordPress
+ Avoid excess of plugins
+ JavaScript compressed, minified and combined in one file
+ Add scripts always on footer
+ CSS compressed, minified and combined in one file
+ Callback image for all WordPress image requests
+ Use Git for version control
+ Use [Gulp](https://github.com/douglasanro/simple-wp-gulp)

### CSS
+ Don't use inline style!
+ Don't use tables for anything other than displaying data in an orderly way.
+ Remove Blank classes/IDs declaration i.e #header { } from your style.
+ Avoid the ‘! important’ in your style. Use the proper specificity.
+ If you are using position: absolute; then make sure its recent parent container ( Or the container to whom you want the absolute element to be relative with ) has position: relative;
+ Giving precise and clear class names to your elements is a key. This will seriously avoid confusion & let you understand your CSS better and faster.
+ Name of classes/IDs based on function, not appearance.
+ Use classes instead of ids whenever possible.
+ Separate class names by dashes. e.g ‘footer-copyright’
+ Note: Avoid names like ‘footerCopyright’, ‘FooterCopyRight’, or ‘footer_copyright’
+ No special characters in classes and ids.
+ For more information about naming see [this article](https://wiki.jasig.org/display/UPC/Markup+and+CSS+Naming+Conventions)
+ Mouse-hover effect should be present for all links.
+ Always specify a fallback generic font. i.e body { font-family: "Open Sans", sans-serif; }
+ Always user a web-safe font i.e [Google fonts](https://fonts.google.com)
+ Use numbers (Hex color), not names, for colors. i.e body { color : #FF0000; }
+ Always use pre-processor (SASS, LESS, Stylus)
+ Avoid coment inline. i.e // comment here



## Pre-launch
+ Check if favicon is there and apple-touch-icons as well and displaying correctly. (favicon 16x16, icon 180x180, ios-icon 192x192)
+ Style miscellaneous pages (404, search results, terms, etc)
+ Setup 301 redirects if needed
+ Review Print version
+ Setup Google Analytics, if not present
+ Setup Google Webmaster Tools, if not present
+ Install a [SEO Plugin](https://wordpress.org/plugins/wordpress-seo/)
+ Browser testing (be honest, was it thorough?)
+ Mobile testing
+ Image optimization [Compress JPEG & PNG images](https://wordpress.org/plugins/tiny-compress-images/)
+ CSS & JS optimization
+ Remove all Lorem Ipsum
+ Proofread entire site for grammar and spelling mistakes
+ Ensure that the client's contact information is entered (social links, admin email, etc)
+ Check all links, main navigation, sub navigation and mobile navigation.
+ Ensure that all required licenses are purchased for necessary plugins, fonts, etc
+ Check that all form submissions are working correctly
+ Check if structured data is working [Google testing tool](https://search.google.com/structured-data/testing-tool)

## Post-launch
+ Finish any remaining SEO configuration
+ Check all links, again.
+ Check all contact forms
+ Build first sitemap and ping search engines
+ Create a backup

## License
[MIT License](LICENSE) © Checklist for when putting a Wordpress site live
