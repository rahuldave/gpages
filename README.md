# gpages

- http://jmcglone.com/guides/github-pages/

```
jupyter nbconvert --to markdown --template ./_support/markdown.tpl  --output-dir . notebooks/olives-model.ipynb
[NbConvertApp] Converting notebook notebooks/olives-model.ipynb to markdown
[NbConvertApp] Support files will be in olives-model_files/
[NbConvertApp] Making directory ./olives-model_files
[NbConvertApp] Making directory ./olives-model_files
[NbConvertApp] Making directory ./olives-model_files
[NbConvertApp] Writing 12014 bytes to ./olives-model.md
(py3l) ➜  gpages git:(master) ✗ ls
README.md          _support           olives-eda.md      olives-model_files
_config.yml        index.md           olives-eda_files
_site              notebooks          olives-model.md
(py3l) ➜  gpages git:(master) ✗ python _support/nbmd.py olives-eda.md
```
