# Rails Blog: Using the Asset Pipeline

Our blog is basically fully functional, but looking a bit bland. Let's add a [free bootstrap theme](http://bootswatch.com/) to our app through the asset pipeline. Then, let's play around with Bootstrap's CSS classes and ids on our views to make it look nice.

## Steps

1. Copy a theme (either a bootstrap.min.css file or a bootstrap.css file) and include it in your `vendor/assets/stylesheets`. We put all stylesheets and javascripts (aka, assets) that we didn't write ourselves in the `vendor` folder.
2. In your `app/assets/stylesheets/application.css` manifest file, include the file(s) we added to our `vendor/assets`.
3. Play around with getting it to look nice! Check out the bootstrap [documentation](http://getbootstrap.com/css/).

## Bcrypt Segmentation Fault Issue

If you run into any Segmentation Fault issues (most likely caused by the `bcrypt` gem), run `gem uninstall bcrypt` (uninstall all versions), and then do `bundle install` again.

## Resources

* [What is the Asset Pipeline](http://edgeguides.rubyonrails.org/asset_pipeline.html#what-is-the-asset-pipeline-questionmark)
* [Asset Organization](http://edgeguides.rubyonrails.org/asset_pipeline.html#asset-organization)

<a href='https://learn.co/lessons/rails-blog-asset-pipeline' data-visibility='hidden'>View this lesson on Learn.co</a>
