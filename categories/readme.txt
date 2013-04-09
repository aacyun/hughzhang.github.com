https://github.com/recurser/jekyll-plugins

generate_categories.rb
A generator that creates category pages for Jekyll sites (for example our plugin category).

Usage
To use it, simply drop the generate_categories.rb script into the _plugins directory of your Jekyll site.

You should also copy the category_index.html file to the _layouts directory of your own project. This file is provided as an example layout, and obviously you can change the HTML as you see fit.

You can also (optionally) generate an atom.xml feed for each category. To do this, copy the category_feed.xml file to the _includes/custom directory of your own project. You'll also need to copy the octopress_filters.rb file into the _plugins directory of your project, as the category_feed.xml requires a couple of extra filters.

How it works
When you compile your Jekyll site, this plugin will loop through the list of categories in your site, and use the layout above to generate a page for each one with a list of links to the individual posts.

Included filters
category_links : Outputs the list of categories as comma-separated links.
date_to_html_string : Outputs the post.date as formatted html, with hooks for CSS styling.
Available _config.yml settings
category_dir : The subfolder to build category pages in (default is 'categories').
category_title_prefix : The string used before the category name in the page title (default is 'Category: ').