SEO Jekyll tool
===============

[![endorse](http://api.coderwall.com/bretthardin/endorsecount.png)](http://coderwall.com/bretthardin)

One problem that [I have with Jekyll](http://bretthard.in/2012/06/jekyll-and-seo-optimization/), and I missed from wordpress, was a way to analyze posts for SEO optimization. I borrowed a lot of the work from Wordpress SEO by YOAST.

Usage
-----
Download the jekyll-seo.rb file and run it against the output of jekyll. This is important. You cannot run this on the markdown file, because it does not contain the HTML that is required for SEO analysis.

	jekyll-seo -k "optimize jekyll for seo" _site/2012/06/open-source-attribution/index.html

Output
------

```
Analyzing Post: _site/2012/06/open-source-attribution/index.html...

Article Heading: true (2)
Page title: true (1)
Content: true (12)
Meta description: true (1)
```

TODO
----
* turn this into a gem that just adds rake tasks to your Jekyll site
* Identify SEO terms in the URL
* You have not used your keyword / keyphrase in any subheading (such as an H2) in your copy.
* No images appear in this page, consider adding some as appropriate.
* The meta description is under 120 characters, however up to 156 characters are available. The available space is shorter than the usual 155 characters because Google will also include the publication date in the snippet.
* The page title contains keyword / phrase, but it does not appear at the beginning; try and move it to the beginning.
* The keyword / phrase does not appear in the URL for this page. If you decide to rename the URL be sure to check the old URL 301 redirects to the new one!
* The copy scores 68.9 in the Flesch Reading Ease test, which is considered OK to read.
* This page has 14 outbound link(s).
* The keyword density is 1.74%, which is great, the keyword was found 15 times.
* The meta description contains the primary keyword / phrase.
* There are 890 words contained in the body copy, this is greater than the 300 word recommended minimum.
* The page title is more than 40 characters and less than the recommended 70 character limit.
#The keyword appears in the first paragraph of the copy.
