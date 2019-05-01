# RSA-2048-implementation
use PyCrypto and Cryptography package to develop RSA algorithm

1.先利用pip安裝PyCrypto和Cryptography這兩個套件，可參考：

  (1) https://cryptography.io/en/latest/ 

  (2) https://www.dlitz.net/software/pycrypto/
  
  (3) https://www.blog.pythonlibrary.org/2016/05/18/python-3-an-intro-to-encryption/

2.若無法順利安裝，可以參考以下解決步驟：

  (1)作業系統沒有Microsoft VC compiler，安裝WindowsCompiler或者下載VC Build Tools。安裝完後，操作以下步驟：

     a. Open command prompt with admin privileges

     b. Run vsvars32.bat from your version of VC

     c. set CL=-FI"%VCINSTALLDIR%\INCLUDE\stdint.h"

     d. pip install PyCrypto.
     
   參考 https://stackoverflow.com/questions/41843266/microsoft-windows-python-3-6-pycrypto-installation-error 

  (2)出現找不到GMP or MPIR linrary，請安裝第一項VC compiler。

   參考 https://stackoverflow.com/questions/32800336/pycrypto-on-python-3-5

  (3)pip安裝文件(必須先安裝pip才能下載package)

   參考 https://pip.pypa.io/en/stable/

  (4)亦可使用easy_install此指令安裝或者python setup.py install來手動安裝(路徑必須在此package的目錄下)

  (5)使用另外一個套件:PyCryptodome

   參考 https://pycryptodome.readthedocs.io/en/latest/

