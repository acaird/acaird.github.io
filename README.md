# Jekyll-Bootstrap

The quickest way to start and publish your Jekyll powered blog. 100% compatible with GitHub pages

## Usage

 - write your blog post in org-mode
   - make sure to include a header like:
     ```
	 #+BEGIN_EXPORT HTML
	 ---
	 layout: post
	 title: title goes here
	 tagline: tagline goes here
	 categories: computers
	 tags: list of space-seperated tags goes here
	 ---
	 #+END_EXPORT

	 ```
 - export your blog post to an HTML file, but select "body only" during the export
 - copy the HTML file to your `_posts` directory in your blog
   - make sure the top of the HTML file has only the YAML block above and that it is first in the file
   - make sure any image references or other references and links all work
 - `git commit` and `git push` the HTML file
 - wait a few minutes, and it should show up in GitHub pages

 If you want to see things locally, install `jekyll`:
  1. `gem install bundler`, `gem install jekyll`
  2. in my case, this put it in `/opt/homebrew/lib/ruby/gems/3.2.0/bin/jekyll`
  3. now you can run `/opt/homebrew/lib/ruby/gems/3.2.0/bin/jekyll serve` or `/opt/homebrew/lib/ruby/gems/3.2.0/bin/jekyll build` to see what information it gives you

If you aren't lazy, you can set up an org-mode publish workflow for this. Or whatever.
