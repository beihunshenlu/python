1.
如果你希望创建一份诸如序列等复杂对象的副本（而非整数这种简单的对象
（Object）），你必须使用切片操作来制作副本。如果你仅仅是将一个变量名赋予给另一个名
称，那么它们都将“查阅”同一个对象，如果你对此不够小心，那么它将造成麻烦。
举例：<br>
print('Simple Assignment')<br>
shoplist = ['apple', 'mango', 'carrot', 'banana']<br>

mylist = shoplist<br>
del mylist[0]<br>
print('shoplist is', shoplist)<br>
print('mylist is', mylist)<br>

mylist = shoplist[:]<br>
del mylist[0]
<br>
print('shoplist is', shoplist)<br>
print('mylist is', mylist)<br>

2.
python 2.7版本需要用raw_input代替input，若仍使用input，则输入的字符串需要加引号，否则会当成变量
