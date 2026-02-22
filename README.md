# PyDeepLX Remastered

A Python package for unlimited DeepL translation with some correctives to work from Russia

## Description

This is a Python package for DeepL translation, I didn't limit the number of translations in the code, if there is a `429` error, it means your IP has been blocked by DeepL temporarily or proxy didn't work, please don't request it frequently in a short time and use trusted proxies.

## Usage

### Install Package

```bash
pip install -i https://github.com/Alberto-Kali/PyDeepLXR.git
```

### Use in code

```python
from PyDeepLX import PyDeepLX
# By default, the source language is automatically recognized and translated into English without providing any alternative results.
PyDeepLX.translate("你好世界") # Return String

# Specify the source and target languages
PyDeepLX.translate("你好世界", "ZH", "EN") # Return String

# Need alternative results
PyDeepLX.translate("毫无疑问的", "ZH", "EN", 3) # Return List: ['Without a doubt', 'No doubt']

# Print the results
PyDeepLX.translate("毫无疑问的", "ZH", "EN", 3, True)

# Using proxy
PyDeepLX.translate(text="毫无疑问的", sourceLang="ZH", targetLang="EN", numberAlternative=0, printResult=False, proxies="socks5://127.0.0.1:7890")
```

## Authors

**PyDeepLX** © [Vincent Young](https://github.com/missuo), Released under the [MIT](./LICENSE) License.<br>
**PyDeepLX Remaster** © [Alberto Genuardy](https://github.com/Alberto-Kali), Released under the [MIT](./LICENSE) License.<br>
