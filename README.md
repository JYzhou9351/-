a=0
while a<3:
    b=int(input("请输入密码："))
    if b==8888 :
        print("密码正确")
        a1 = 0
        c2=10000
        c=c2-b
        while a1 < 3:
            b = int(input('请输入取款金额：'))
            if c <0:
                print("余额不足")
                a1 += 1
                continue
            else:
                print(f'取款成功，余额：{c2 - b}')
                a=0
                c2=c2-b
                d=input('是否需要继续取款（yes/no）:')
                if d=='yes':
                    continue
                elif d=='no':
                    break
                else:
                    print('格式错误')

        else:
            print('goodbye')
            break
    else:
        print('密码错误')
        a+=1
else:
        print('该帐户被冻结')
