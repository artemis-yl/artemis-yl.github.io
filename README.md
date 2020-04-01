## Personal Notes on How to Do This

### Collapsible Section

# How to structure

YOU MUST ADD THE {} STUFF. kramdown doesn't read md for the insides of blocks, and sadly commommark doesn't image size.
```
# A collapsible section with markdown

{::options parse_block_html="true" /}

<details>
  <summary markdown="span">Click to expand!</summary>
  
  ## Heading
  1. A numbered
  2. list
     * With some
     * Sub bullets
</details>

{::options parse_block_html="false" /}

```

{::options parse_block_html="true" /}

<details>
  <summary>Click to expand!</summary>
  
  ## Heading
  1. A numbered
  2. list
     * With some
     * Sub bullets
</details>

{::options parse_block_html="false" /}

### Making a Table of Contents
```
1. [Introduction](#introduction)
2. [Some paragraph](#paragraph1)
    1. [Sub paragraph](#subparagraph1)
3. [Another paragraph](#paragraph2)

#### This is the introduction <a name="introduction"></a>
Some introduction text, formatted in heading 2 style

#### Some paragraph <a name="paragraph1"></a>
The first paragraph text

##### Sub paragraph <a name="subparagraph1"></a>
This is a sub paragraph, formatted in heading 3 style

#### Another paragraph <a name="paragraph2"></a>
The second paragraph text
```

1. [Introduction](#introduction)
2. [Some paragraph](#paragraph1)
    1. [Sub paragraph](#subparagraph1)
3. [Another paragraph](#paragraph2)

#### This is the introduction <a name="introduction"></a>
Some introduction text, formatted in heading 2 style

#### Some paragraph <a name="paragraph1"></a>
The first paragraph text

##### Sub paragraph <a name="subparagraph1"></a>
This is a sub paragraph, formatted in heading 3 style

#### Another paragraph <a name="paragraph2"></a>
The second paragraph text

### How to comment
Found this on Stackflow. but use this syntax:
```
(empty line)
[comment]: # (Type comment msg here)
```
Tested with the space below:


[comment]: # ( AAAAAAAAAAAAAAAAAAAAA PLS WORK)


There should be nothing.

### Side Bar
**Bottom Icons and their links**
Go to  ```_includes/custom-icon-links.html```

Copy code block 

Replace NAME with appropriate name for the link (ex. twitter)

Replace SITE_LINK with the start of the address (ex. https: //wwww.twitter.com/). 
    Rename NAME_NAME. This variable can be found in config.yml Note that {{<>}} can be removed and just have the whole link.

Replace ICON_MAGE_NAME with the name of the icon image file. Make sure the file is in the same folder. 
    If I get too many icons, I may make a new folder and need to readdress these to /svg/<>.svg
```
<a id="github-link"
    class="icon" title="NAME" aria-label="NAME"
    href="SITE_LINK/{{ site.NAME_NAME }}">
  {% include ICON_MAGE_NAME.svg %}
</a>
```
**Order of Navigation**
Got to ```_includes/sidebar-nav-links.html```

The last three lines determine if project pages or normal pages or icons go first.

The order of projects and pages themselves is determined by the ```sidebar_sort_order: <#>``` which is in the .md file itself. 
Basically, 1 goes first.

**Colour and Fonts and Others**
Go to ```assets/css/main.scss``` and name the variables. Check out the original repo for names of the variables and what they can do.

## Pages

**Categories vs Pages vs Posts**
Pages are just normal pages.

Categories group pages that are 'tagged' to belong within that category with 

Posts are pages that get sorted into categories.
  
  In order for posts to be collected, they MUST be:
  - named with YYYY-MM-DD-title.md format
  - tagged with this additional in the top
    ``` 
    categories:
    - NAME_OF-CATEGORY
     ```
### Posts
**Comments**
I removed comments from appearing on Post type pages by making the ```comments.html``` and leaving it blank.

## Welcome to GitHub Pages

You can use the [editor on GitHub](https://github.com/96yrlee/96yrlee.github.io/edit/master/README.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

Additional Lines
```
<p>&nbsp;</p> 
``` 
for all, specifically between elements such as bullet points
```&nbsp;``` for general. 
Repeat it for each additional line.

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/96yrlee/96yrlee.github.io/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://help.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.
