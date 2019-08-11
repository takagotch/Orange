### orange
---
https://orange.biolab.si/

```py
// orangecontrib/example/tests/test_example.py
import unittest
from Orange.widgets.tests.base import WidgetTest

from orangecontrib.example.wudgets.mywidget import MyWidget

class ExampleTests(unittest.TestCase):
  def test_addition(self):
    self.assertEqual(1 + 1, 2)
    
class TestMyWidget(WidgetTest):
  def setUp(self):
    self.widget = self.create_widget(MyWidget)
    
  def test_addition(self):
    self.assertEqual(1 + 1, 2)

```

```sh
pip install .
pip install -e .
make html htmlhelp
python html htmlhelp
python -m Orange.canvas
```

```
```


