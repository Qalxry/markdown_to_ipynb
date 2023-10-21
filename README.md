# markdown_to_ipynb

A simple Python script that converts Markdown files to IPython Notebook (.ipynb) format. Code blocks are placed in code cells, while other text is placed in Markdown cells.

### Usage:

```text
    python markdown_to_ipynb.py <markdown_file_or_folder> [-o <ipynb_file>]

    <markdown_file_or_folder>       Input Markdown file or folder
    -o, --output                    Output IPython Notebook file or folder (default: <markdown_file_or_folder>)
    -y, --yes                       Do not ask for confirmation (default: False)
    -v, --version                   Show version
    -h, --help                      Show help
    -u, --usage                     Show usage

```
 
### Example:

```bash
    python markdown_to_ipynb.py test.md
    python markdown_to_ipynb.py test.md -o test.ipynb
    python markdown_to_ipynb.py test.md --output test.ipynb
    python markdown_to_ipynb.py ./markdown/
    python markdown_to_ipynb.py ./ -o ./ipynb/ -y
```

### Actual effect:

#### Input .md file: 

```markdown
## TEST

This is a test file.

这是一个测试文件。


```
a = 1
b = 2
c = a + b
print(c)
```

## TEST2

This is a test file.

```
import numpy as np

def main():
    return 0
```

> This is a test file.
```

#### Output .ipynb file:

![Output .ipynb file](https://github.com/Qalxry/markdown_to_ipynb/assets/70196852/b90e8756-dbb5-4404-97da-c3efa1afc25d)


