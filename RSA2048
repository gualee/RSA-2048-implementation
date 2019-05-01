import Crypto
from Crypto.PublicKey import RSA
from Crypto import Random
import base64
import ast
import time

random_generator = Random.new().read
key = RSA.generate(1024, random_generator)  #產生公私鑰

publickey = key.publickey() # pub key export for exchange

start = time.time()                         #計時的起點

f = open(r'D:\randfile5.bin', 'rb')

message = f.read()                          #b'ascc' 

encrypted = publickey.encrypt(base64.b64encode(message),32)
#message to encrypt is in the above line 'encrypt this message'

print('encrypted message:', encrypted)      #密文

f.close()

end = time.time()                           #計時的終點
answer = end - start                        #時間差
print("RSA-2048的加密執行時間為: ", answer)  #印出執行時間
