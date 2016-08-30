
<style>
body {
	background-color: Linen;
}
.error {
    color: red;
}
code.prompt {
	color: CornflowerBlue; /* dark blue */
}
code.prompt-user {
	color: Black; /*  */
	background-color: LightGoldenRodYellow;
}
code.prompt-root {
	color: GreenYellow; /*  */
	background-color: Black;
}
code.input {
	color: Maroon; /*  */
}
code.output {
	color: Black; /* LightSkyBlue light blue */
}
pre.input {
	color: Maroon;  /* maroon (same as code.input) */
}
pre.output {
	color: LightSkyBlue;  /* light blue (same as code.output) */
}
</style>

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

<!--
<code class="error">BTW, what is your id on GitHub?</code>
-->

### Clone this empty repo locally.

- 'cd' to the stub for the area where you do your work. I call mine 'work' (creative, huh?).
- 'clone' the empty repo.

<code>git clone https://github.com/&lt;username&gt;/&lt;username&gt;.github.io</code>

This gives you:

- a definition for 'origin',

- an initialized local repo, and

- a workspace (with nothing in it).

### Create a web page

- 'cd' into the workspace

<code>echo "You could have used atom!" &gt; index.html</code>

### Commit to master on local repo

<code>git add .</code>

<code>git commit -m '
Brief description (&lt;50 chars), no period, \n<br/>
This is a blank line followed by<br/>
More detailed description wrapped at 72 chars
'</code>

### Push local repo to GitHub

<code>git push origin master</code>

### View your New Awesome Web Site

Browse to http://github/&lt;username&gt;.github.io

