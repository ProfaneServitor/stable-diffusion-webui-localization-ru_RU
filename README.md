Russian localization of Stable Diffusion webui

# Скрипт для добавки отсутствующих ключей

```python
import json
files=['localization.json', 'ru_RU.json']

with open('merged_file_name.json', "w") as outfile:
    res = dict()
    for f in files:
        dct = dict(json.load(open(f, "r").read()))
        res.update(dct)
    outfile.write(res)

```
