## Flow
1. Create a JSONT template (https://goessner.net/articles/jsont/):

<pre>
"link": {"uri":"http://company.com", "title":"company homepage" }}

which we want to transform into a HTML link element.

<a href="http://company.com">company homepage</a>

For doing this we can write a corresponding rule

{ "link": "<a href=\"{link.uri}\">{link.title}</a>" }
</pre>

1. Read comments using docco (https://www.npmjs.com/package/docco):

1. Loop through the file comments using Docco

1. Add values to the JSON data ( jsond.link.target = /link.target:(.+)/, $1)

1. Generate code using JSONT
