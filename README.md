如果你希望创建一份诸如序列等复杂对象的副本（而非整数这种简单的对象
（Object）），你必须使用切片操作来制作副本。如果你仅仅是将一个变量名赋予给另一个名
称，那么它们都将“查阅”同一个对象，如果你对此不够小心，那么它将造成麻烦。
举例：
print('Simple Assignment')
shoplist = ['apple', 'mango', 'carrot', 'banana']

mylist = shoplist
del mylist[0]
print('shoplist is', shoplist)
print('mylist is', mylist)

mylist = shoplist[:]
del mylist[0]

print('shoplist is', shoplist)
print('mylist is', mylist)
