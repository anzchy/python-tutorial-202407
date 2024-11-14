This repo contains different versions of the official python tutorial, only for noncommercial use.

# source files    
> https://github.com/python/cpython       

# tool for converting ipynb format:   
converted by rst2ipynb: 
https://pypi.org/project/rst2ipynb/

how to use:
```rst2ipynb xxx.rst -o xxx.ipynb```

# tool for converting to html format:  
html/epub converted by Sphinx: 
http://www.sphinx-doc.org  

how to use:      
> add conf.py
```

import sphinx_rtd_theme

html_theme = 'sphinx_rtd_theme'
html_theme_path = [sphinx_rtd_theme.get_html_theme_path()]


# 项目基本信息
project = 'Python Doc'
copyright = '2024, Jack Cheng'
author = 'Jack Cheng'
version = '1.0'
release = '1.0'

# 输出格式
extensions = [
    'sphinx.ext.autodoc',
    'sphinx.ext.intersphinx',
    'sphinx.ext.todo',
    'sphinx.ext.coverage',
    'sphinx.ext.mathjax',
    'sphinx.ext.ifconfig',
    'sphinx.ext.viewcode',
    'sphinx.ext.githubpages',
]

source_suffix = '.rst'
master_doc = 'index'

# HTML 输出设置
html_theme = 'sphinx_rtd_theme'
html_static_path = ['_static']

# 其他设置
language = 'en_US'
exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']

```

> converting command  
```
sphinx-build /Users/xxx/Desktop/python-rst /Users/xxx/Desktop/python_tutorial_202407
```





