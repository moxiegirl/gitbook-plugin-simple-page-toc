# Gitbook Simple Page TOC Plugin [![npm version](https://badge.fury.io/js/gitbook-plugin-simple-page-toc.svg)](https://badge.fury.io/js/gitbook-plugin-simple-page-toc)

This plugin inserts a table of content (TOC) section into your GitBook page. It is powered by the  [markdown-toc](https://github.com/jonschlinkert/markdown-toc) library.

## Usage

### Installation

Add the plugin to your `book.json`:

```
{
	"plugins" : [ "simple-page-toc" ]
}		
```

### Create TOC

Place a `<!-- toc -->` code comment somewhere into your text. Generating your GitBook inserts a table of contents immediately after this comment.

### Optional configuration

You can add the following configuration params to your `book.json`:

```
{
	"plugins" : [ 
		"simple-page-toc" 
	],
	"pluginsConfig": {
		"simple-page-toc": {
			"maxDepth": 3,
			"skipFirstH1": true
   }
}		
```

Name        | Type    | Default | Description 
----------- | ------- | ------- | ------------
maxDepth    | Number  |       3 | Use headings whose depth is at most maxdepth.
skipFirstH1 | Boolean |    true | Exclude the first h1-level heading in a file.

## Changelog

* 0.1.0 Releases:
  * 0.1.0 First release
