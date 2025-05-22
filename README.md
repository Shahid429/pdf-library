# pdf-library
A minimal GitHub Pages site hosting my collection of PDF books via an embedded in-browser viewer (Mozilla PDF.js), providing easy link-based, read-only access with download and print disabled.
# PDF Hub  
A minimal GitHub Pages site hosting my PDF book collection via an embedded in-browser viewer, providing link-based, read-only access with download and print disabled. :contentReference[oaicite:0]{index=0}

## Setup  
1. Create a repository named `yourusername.github.io` and push your PDFs into a folder called `books/`. :contentReference[oaicite:1]{index=1}  
2. For each PDF, add an HTML file (e.g., `book1.html`) embedding PDF.js from a CDN to display `books/book1.pdf`. :contentReference[oaicite:2]{index=2}  
3. In each HTML, include CSS to hide PDF.js toolbar download/print buttons:  
   ```css
   .toolbarButton.download,
   .toolbarButton.print { display: none !important; }
   ``` :contentReference[oaicite:3]{index=3}  
4. Enable GitHub Pages under **Settings → Pages → Source: main branch**. :contentReference[oaicite:4]{index=4}  

## Usage  
- View each book at `https://yourusername.github.io/book1.html`, `book2.html`, etc. :contentReference[oaicite:5]{index=5}  
- Readers can only pan, zoom, and browse pages—download and print are disabled by CSS. :contentReference[oaicite:6]{index=6}  

## Customization  
- To change the viewer scale, update the JavaScript render scale (e.g., `scale: 1.5`). :contentReference[oaicite:7]{index=7}  
- You can adjust page layout by editing the `<canvas>` styling or wrapping it in a responsive container. :contentReference[oaicite:8]{index=8}  

## Maintenance  
- To add a new book, upload `books/bookX.pdf` and create `bookX.html` following the same template. :contentReference[oaicite:9]{index=9}  
- Update this README to list any new book links so visitors can easily find them. :contentReference[oaicite:10]{index=10}  

## License  
All rights reserved for hosted PDF content.  
