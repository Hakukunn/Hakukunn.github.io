## Welcome to GitHub Pages

<!DOCTYPE html>
<meta name="viewport" content="initial-scale=1.0, user-scalable=no" />  
<style type="text/css">  
    html{height:100%}    
    body{height:100%;margin:0px;padding:0px}    
    #container{height:100%}    
</style> 
<script type="text/javascript" src="https://api.map.baidu.com/api?v=2.0&ak=LXpXl6bnXk8EPypPqxwu1CL1s2j0jLU9"></script>
<div id="container"></div> 
var map = new BMap.Map("container"); 
var point = new BMap.Point(116.404, 39.915); 
map.centerAndZoom(point, 15);  
var map = new BMap.Map("container");    
var point = new BMap.Point(116.404, 39.915);    
map.centerAndZoom(point, 15);    
window.setTimeout(function(){  
    map.panTo(new BMap.Point(116.409, 39.918));    
}, 2000);









You can use the [editor on GitHub](https://github.com/Hakukunn/Hakukunn.github.io/edit/main/index.md) to maintain and preview the content for your website in Markdown files.

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

For more details see [Basic writing and formatting syntax](https://docs.github.com/en/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/Hakukunn/Hakukunn.github.io/settings/pages). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://support.github.com/contact) and we’ll help you sort it out.
