
  

https://0x7x.github.io/markdowngeneration/Readme

  
  

<center><span style="font-size: 24px;">Helpful Things to Paste in Obsidian</span></center>

  

<hr>

  
  

> New Page Page Break

  
  

```
<div style="page-break-after: always;"></div>
```

  
  

<hr>

  

> Long Straight Line

  

```
<hr>
```

  

<hr>

  

> Center Text

  

```

<center>Text Here</center>

```

  

<hr>

  

> Bold and Change Size of Text

  

```

<span style="font-size: 24px; font-weight: bold;">Text Here</span>

```

  

<hr>

  

> Paragraph Indent

  

```

$\quad$

```

  
  
  

```

---

```

  

<hr>

  

> Check Box

  

```

- [ ] Task

```

  

---

  

> Check Box

  

```html

<!DOCTYPE html>

<html>

<head>

<title>Markdown Viewer</title>

<script src="https://cdn.jsdelivr.net/npm/marked@2.0.0/marked.min.js"></script>

<link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Inter&display=swap">

<link rel="stylesheet" type="text/css" href="index.css">

<script>

// Extract the file name from the URL

var path = window.location.pathname;

var pageName = path.split('/').pop().replace('.md', '');

  

// Set the page title

document.title = pageName;

</script>

</head>

<body>

<div id="markdown-content" class="markdown-content">

<!-- Markdown content will be loaded here -->

</div>

  

<script>

// Extract the file name from the URL

var path = window.location.pathname;

var pageName = path.split('/').pop().replace('.html', ''); // Assuming the file extension is ".md"

var pageNameClean = decodeURI(path.split('/').pop().replace('.html', '')); // Assuming the file extension is ".md"

// Set the page title and display the title within the content

document.title = pageNameClean;

document.getElementById('markdown-content').innerHTML = '<h1 class="x1">' + pageNameClean + '</x1>';

  

// Now, fetch and render the Markdown content

fetch(pageName + '.md') // Use the pageName to fetch the .md file

.then(response => response.text())

.then(markdown => {

// Replace image references with the correct paths and sizes

markdown = markdown.replace(/!\[\[([^\]|\n]+?)(?:\s*\|\s*(\d*))?\s*]]/g, function(match, p1, p2) {

const imagePath = 'attachments/' + p1;

const width = p2 ? ` width="${p2}"` : '';

return `<img src="${imagePath}" alt="Image"${width}>`;

});

  

// Parse and render the modified Markdown content

document.getElementById('markdown-content').innerHTML += marked(markdown);

})

.catch(error => {

console.error('Error loading Markdown file:', error);

});

</script>

</body>

</html>

  

```

  

---