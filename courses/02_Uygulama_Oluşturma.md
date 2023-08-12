# İlk Uygulamamızı Oluşturalım

![111](https://github.com/fuatsezer/PyQt5/assets/63423939/1b7e5124-a1b5-4e0a-9ea0-485d086dd3ff)



```python
import sys
from PyQt5 import QtWidgets
from PyQt5.QtWidgets import QApplication, QMainWindow, QToolTip
from PyQt5.QtGui import QIcon

def window():
    app = QApplication(sys.argv) # uygulama yaratma (gerekli)
    win = QMainWindow() # Pencere yaratma (gerekli)
    win.setWindowTitle("First Application") # Uygulama başlığı 
    win.setGeometry(200,200,700,700) # Pencerenin pozisyonunu ve boyutunu belirleme 
    # (pos_x,pos_y,size_x,size_y) 
    win.setWindowIcon(QIcon("img.png")) # Uygulamanın iconunu belirleme
    win.setToolTip("my tool tip")
    win.show() # Pencereyi gösterme (gerekli)
    sys.exit(app.exec_()) # X tuşuna basınca pencereyi kapatma (gerekli)

window() # window fonksiyonunu çağırma (gerekli)
```
