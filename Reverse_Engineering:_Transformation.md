
## Reverse Engineering: Transformation
```
Step: Run terminal then execute command below.
wget https://mercury.picoctf.net/static/dd6004f51362ff76f98cb8c699510f23/enc
cat enc
python3
decode = '灩捯䍔䙻ㄶ形楴獟楮獴㌴摟潦弸弰摤捤㤷慽'
print(decode.encode('utf-16-be'))
```
