# Nairobi Eats

If you see this error:

Error: error building site: "/Users/brianmarete/Documents/projects/hugo-projects/nairobi-eats/content/reviews/zen-garden/index.md:28:1": failed to render shortcode "image-gallery": failed to process shortcode: "/Users/brianmarete/Documents/projects/hugo-projects/nairobi-eats/layouts/shortcodes/image-gallery.html:47:27": execute of template failed: template: shortcodes/image-gallery.html:47:27: executing "shortcodes/image-gallery.html" at <$image.Fit>: nil pointer evaluating resource.Resource.Fit

Do the following:

1. Make sure image path names and titles in gallery.json match asset names in cloudflare
2. Delete /resources/images folder
3. Run hugo server --gc
