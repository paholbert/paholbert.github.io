
# Minimum Configuration to Display a Website on GitHub

Here's the very minimum you have to do to get your site on GitHub.

## System encompases 
- GitHub and
- local

It excludes:

- No Bootstrap
- No Jekyll
- No frills at all

### Create a new repo on GitHub called &lt;username&gt;.github.io,

where &lt;username&gt; is your id on GitHub, of course.
	
<code class="error">BTW, what is your id on GitHub?</code>

### Clone this empty repo locally.

'cd' to the stub for the area where you do your work. I call mine 'work' (creative, huh?).
'clone' the empty repo.
git clone https://github.com/&lt;username&gt;/&lt;username&gt;.github.io
This gives you 
a definition for 'origin',
an initialized local repo, and
a workspace (with nothing in it).

### Create a web page

'cd' into the workspace
echo "You could have used atom!" &gt; index.html

### Commit to master on local repo

git add .
git commit -m '
Brief description (&lt;50 chars), no period, \n

More detailed description wrapped at 72 chars
'

### Push local repo to GitHub

git push origin master

### View your New Awesome Web Site

Browse to http://github/&lt;username&gt;.github.io

