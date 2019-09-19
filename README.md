### markupsafe
---
https://github.com/pallets/markupsafe

```py
// tests/test_exception_custom_html.py
import pytest

from markupsafe import escape

class CustomHtmlThatRaises(object):
  def __html__(self):
    raise ValueError(123)
    
def test_exception_custom_html():
  obj = CustomHtmlThatRaises()
  with pytest.raises(ValueError):
    escape(obj)
```

```
```

```
```


