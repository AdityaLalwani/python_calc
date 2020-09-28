# Details of test.py 
    import sys
    from PyQt5.QtWidgets import QApplication
    from PyQt5.QtWidgets import QLabel
    from PyQt5.QtWidgets import QWidget
    app = QApplication(sys.argv)
    window = QWidget()
    window.setWindowTitle('PyQt5 App')
    window.setGeometry(100, 100, 280, 80)
    window.move(600, 15)
    helloMsg = QLabel('This is Test', parent=window)
    helloMsg.move(60, 30)
    window.show()
    sys.exit(app.exec_())

#3: Create view of application i.e. GUI
Create class named view.py
Import following modules
from PyQt5.QtWidgets import QMainWindow
from PyQt5.QtWidgets import QWidget
from PyQt5.QtWidgets import QGridLayout
from PyQt5.QtWidgets import QLineEdit
from PyQt5.QtWidgets import QPushButton
from PyQt5.QtWidgets import QVBoxLayout
Create class GUI with parent set to QMainWindow
class GUI(QMainWindow):
Add Constructor ...It will initiate main window by calling superclass constuctor and setting basic parametes such as ..* WindowTitle ..* Size ..* generalLayout ..* LED Display ..* Buttons

Define methods ..* _createDisplayLED ..* _createButtons ..* setDisplayText ..* getDisplayText ..* clearDisplay