# Static Site Generator (Project is in progress)

A simple static site generator written in Python. It converts Markdown files in the `content/` directory into styled HTML pages using a template, and copies static assets to the output directory.

## Technologies Used

- **Python 3**: Core language for all scripts.
- **Standard Library**: Uses only Python's built-in modules (`os`, `shutil`, etc.).
- **HTML/CSS**: For templates and styling.
- **Markdown**: Content source format.

## Installation & Local Usage

1. **Clone the repository:**
   ```sh
   git clone https://github.com/Soumava-221B/Static_Site_Genrator-Python-.git
   cd Static_Site_Genrator-Python-
   ```

2. **Ensure Python 3 is installed:**
   ```sh
   python3 --version
   ```

3. **Run the site generator and start the local server:**
   ```sh
   ./main.sh
   ```
   This will:
   - Delete and recreate the `public/` directory.
   - Copy static assets from `static/` to `public/`.
   - Convert Markdown files from `content/` to HTML in `public/`.
   - Start a local server at [http://localhost:8888](http://localhost:8888).

4. **Run tests:**
   ```sh
   ./test.sh
   ```

## File Structure

```
.
├── content/           
│   ├── blog/
│   │   ├── glorfindel/
│   │   │   └── index.md
│   │   ├── tom/
│   │   │   └── index.md
│   │   ├── majesty/
│   │   │   └── index.md
│   ├── contact/
│   │   └── index.md
│   └── index.md
├── public/           
│   ├── blog/
│   │   ├── glorfindel/
│   │   │   └── index.md
│   │   ├── tom/
│   │   │   └── index.md
│   │   ├── majesty/
│   │   │   └── index.md
│   ├── contact/
│   │   └── index.md
│   ├── images/
│   │   ├── glorfindel.png
│   │   ├── rivendell.png
│   │   ├── tolkien.png
│   │   ├── tom.png
│   ├── index.css
│   └── index.html
├── src/               
│   ├── copystatic.py      
│   ├── gencontent.py      
│   ├── htmlnode.py        
│   ├── inline_markdown.py 
│   ├── main.py            
│   ├── markdown_blocks.py 
│   └── textnode.py        
├── static/            
│   ├── index.css
│   └── images/
│       ├── glorfindel.png
│       ├── tom.png
│       ├── rivendell.png
│       ├── tolkien.png
.
```
