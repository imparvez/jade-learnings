# jade-learnings

What is Jade?
Jade is designed primarily for server side templating in node.js, however it can be used in many other environments.

It is only intented to produce XML like documents(HTML, RSS etc).

To Install Jade in your project:
npm install -g jade

To check whether it has been installed correctly:
jade --help

You will be provided with the list of help/options related to jade

Once done with successful installation of jade in your project folder.
Go to the project directory
Create one file name "index.jade"
Write basic tags in it(Which will be taught to you in this tutorials)
Then type: jade index.jade
Voila!!!!You will get a new HTML rendered document.

###Tags:
First word in JADE is always a Tag such as,
p
div
h1 etc

After the first word, whatever content is gets wrapped inside that same tag.
Jade knows about self closing tags such as,
img
input

Try this in your terminal to see the results for self closing tags
$echo img | jade

###Text:
Everything after the first word in jade is text

p hello world
Text gets wrapped around tags in jade

Note: For multiple line use PIPE |
Jade understands PIPE as a placeholder such as

p
	| Hello world
	| <h1>This is an heading</h1>
	| Hope you enjoy this

###Nesting
Nesting in JADE is same as what we prefer while writing HTML document
Hit tab to have proper indentation in our text editor. Same goes with Jade such as

div
	p
		h1 This is header
	p
		strong I'm strong
	div
		small Say HIII!!!!

While nesting, add a new line and hit a tab to have a proper indentation

###Comments
- Single Line Comments
	//Your Comments goes here
	p your text
	div
		h1 header

-Unbuffered Commnets
	//- Your Comments here won't show up in HTML document
	p Your text

-Block Comments
	// This is multi line comments
		You just have to hit enter
		and write your new comment

###Classes
Class in jade can be define using . and className after that for eg:

p.paragraph
p element with "paragraph" as its class name

###IDs
IDs in ajde can be define using # and IDname after that for eg:

#container
div element with "container" as its IDs name


































