#通讯录
x={}
def ppp(x):#新建联系人
    d1=input("请输入联系人")
    d2=input("请输入号码")
    if d1 not in x:#创建一个空的号码list
        x[d1]=[]
    x[d1].append(d2)
    print(x)
    
def   p1p(x):#删除联系人
    d1=input("请输入联系人")
    while d1 not in x:
        print("该联系人不存在")
        d1=input("请输入联系人")
    del x[d1]

def p2p(x):#查找联系人
    d1=input("请输入联系人")
    while d1 not in x:
        print("该联系人不存在")
        d1=input("请输入联系人")
    print(x[d1])

func='0'
while(func!='5'):
    print('''
    1.	新增联系人
    2.	删除联系人
    3.	显示联系人
    4.	查询联系人
    5.	其他任意键退出
    ''')
    func=input()
    if func=='1':
        ppp(x)
    elif func=='2':
        p1p(x)
    elif func=='3':
        print(x)
    elif func=='4':
        p2p(x)
    else:
        break
    



