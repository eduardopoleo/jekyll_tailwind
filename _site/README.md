# Notes:

Objects {{ }} -> just to output variables
tags {% %} -> to write logic into the partials
filters {{ "hi" | capitalize }} -> pipes the object into a function

Folder Structure:
- _layout: render {{ content }} and must be specified in the page front matter
- _site: where the site static assets get generated and dump into
- _includes: we put partials that get repeated into different layouts or other places
  {% include navigation.html %} navigation.html is in the includes files
- _data: use to store data in the file system that you can use to iterate over
- _sass: Sass comes bundles up with jekyll and the sass file will live in the top folder
- _posts are also first class citizens from the beginning. I think they are a baked in collection!
  post entries have the following form: date-title.html. `page.date` and `page.title` get parsed from it
  automagically