# Python
 homework
1.
請撰寫一程式,讓使用者輸入 5 個數字,計算並輸出這 5 個數字之數
值、總和及平均數。
提示:總和與平均數皆輸出到小數點後第 1 位。
'''
A = (int(input('請輸入數字:')))
B = (int(input('請輸入數字:')))
C = (int(input('請輸入數字:')))
D = (int(input('請輸入數字:')))
E = (int(input('請輸入數字:')))
Z = (A, B, C, D, E)
print(Z)
print('總和:', sum(Z), '平均', sum(Z) / 5)


2.
假設一賽跑選手在 x 分 y 秒的時間跑完 z 公里,請撰寫一程式,輸入
x、y、z 數值,最後顯示此選手每小時的平均英哩速度(1 英哩等於
1.6 公里)。
提示:輸出浮點數到小數點後第一位。

x = eval(input('請輸入數字 X分:'))
y = eval(input('請輸入數字 Y秒:'))
z = eval(input('請輸入數字 Z公里:'))
Speed = (z / 1.6) / ((60 * x + y) / (60 * 60))
print('Speed = %.1f' % (Speed))


3.
請撰寫一程式,輸入兩個正數,代表一矩形之寬和高,計算並輸出此
矩形之高(Height)、寬(Width)、周長(Perimeter)及面積
(Area)。
提示:輸出浮點數到小數點後第二位。

A = eval(input('請輸入正數:'))
B = eval(input('請輸入正數:'))
print("高 = %.1f" % A)
print("寬 = %.1f" % B)
print("周長 = %.1f" % ((A + B) * 2))
print("面積 = %.1f" % (A * B))




4.
請使用選擇敘述撰寫一程式,讓使用者輸入三個邊長,檢查這三個邊
長是否可以組成一個三角形。若可以,則輸出該三角形之周長;否則
顯示【Invalid】。
提示:檢查方法 = 任意兩個邊長之總和大於第三邊長。

A = eval(input('請輸入邊長:'))
B = eval(input('請輸入邊長:'))
C = eval(input('請輸入邊長:'))

if A + B >= C and A + C >= B and B + C >= A:
    print("三角形之周長", (A + B + C))
else:
    print("Invalid")
    
    
    
    
5.
請使用選擇敘述撰寫一程式,讓使用者輸入一個十進位整數 num(0 ≤
num ≤ 15),將 num 轉換成十六進位值。
提示:轉換規則 = 十進位 0~9 的十六進位值為其本身,十進位
10~15 的十六進位值為 A~F。


num=eval(input('請輸入0~15:'))
if num>=0 and num<=9 :
  print(num)
if num==10:
  print("A")
elif num==11:
  print("B")
elif num==12:
  print("C")
elif num==13:
  print("D")
elif num==14:
  print("E")
elif num==15:
  print("F")





6.
請使用選擇敘述撰寫一程式,要求使用者輸入購物金額,購物金額需
大於 8,000(含)以上,並顯示折扣優惠後的實付金額。購物金額折扣
方案如下表所示:
金額 折扣
8,000(含)以上 9.5 折
18,000(含)以上 9 折
28,000(含)以上 8 折
38,000(含)以上 7 折

num = eval(input('請輸入購物金額:'))
if num >= 38000:
    print('折扣優惠後的實付金額:%d' % (num * 0.7), '元')
elif num >= 28000:
    print('折扣優惠後的實付金額:%d' % (num * 0.8), '元')
elif num >= 18000:
    print('折扣優惠後的實付金額:%d' % (num * 0.9), '元')
elif num >= 8000:
    print('折扣優惠後的實付金額:%d' % (num * 0.95), '元')
    
    
7.
請使用選擇敘述撰寫一程式,根據使用者輸入的分數顯示對應的等
級。標準如下表所示:
分數 等級
80 ~ 100 A
70 ~ 79 B
60 ~ 69 C
<= 59 F

grade = eval(input('請輸入分數:'))

if grade >= 80 and grade < 100:
    print('等級:A')
elif grade >= 70 and grade < 80:
    print('等級:B')
elif grade >= 60 and grade < 70:
    print('等級:C')
elif grade <= 59:
    print('等級:F')
    
    
8.
請使用選擇敘述撰寫一程式,讓使用者輸入一個正整數,然後判斷它
是 3 或 5 的倍數,
顯示【x is a multiple of 3.】或【x is a multiple of5.】
;若此數值同時為 3 與 5 的倍數,顯示【x is a multiple of 3 and5.】;
如此數值皆不屬於 3 或 5 的倍數,顯示【x is not a multiple of 3
or 5.】,將使用者輸入的數值代入 x。

x = eval(input('請輸入一個正整數:'))
if (x % 3 == 0 and x % 5 != 0):
    print(x, "x is a multiple of 3.")
elif (x % 3 != 0 and x % 5 == 0):
    print(x, "x is a multiple of 5.")
elif x % 3 == 0 and x % 5 == 0:
    print(x, "x is a multiple of 3and 5.")
elif x % 3 != 0 and x % 5 != 0:
    print(x, "x is not a multiple of 3 or 5.")
    
    
    
    
    
9.
請使用迴圈敘述撰寫一程式,提示使用者輸入金額(如 10,000)、年
收益率(如 5.75),以及經過的月份數(如 5),接著顯示每個月的
存款總額。
提示:四捨五入,輸出浮點數到小數點後第二位。
舉例:
假設您存款$10,000,年收益為 5.75%。
過了一個月,存款會是:10000 + 10000 * 5.75 / 1200 = 10047.92
過了兩個月,存款會是:10047.92 + 10047.92 * 5.75 / 1200 =
10096.06
過了三個月,存款將是:10096.06 + 10096.06 * 5.75 / 1200 =
10144.44
以此類推。

money = int(input('請輸入金額:'))
rate = float(input('請輸入年收益率:'))
month = int(input('請輸入經過的月份數:'))

#print('%s \t  %s' % ('月份', '存款'))  ## /t是縮排等於一個tag
for i in range(month):
   money = money + (money * rate / 1200)
   print('過了%d個月'%(i+1),',存款將是',round(money,2),'元')
   
   
   
   
 
10.
請使用迴圈敘述撰寫一程式,讓使用者輸入一個正整數 a,利用迴圈
計算從 1 到 a 之間,所有 5 之倍數數字總和。
'''
a = eval(input('請輸入一個整數:'))
c = 0# 從0起始
for i in range(1,a+1,1):
    if i%5 == 0:
        c += i
        print('總和是',c)
##range(start, stop[, step]) 可創建整數列表，一般用在for迴圈
##從0開始算
##算到stop-1結束,不包括stop
##間隔，從1開始 range(0, 20, 5) = [0, 5, 10, 15])
    
  
  
 
 輸入一個數字,用@排出一個直角三角型 
 例如:輸入7
 @
 @@
 @@@
 @@@@
 @@@@@
 
 n = int(input('請輸入數字:'))

for i in range(1,n+1):

    print(' '*(n-i),'@'*i)
    
  
    
    
  9X9乘法表
  for i in range(1, 10):
    for c in range(2, 6):
        print('{}*{}={}'.format(c, i, c * i), end='\t')
    print('')
print('')

for i in range(1, 10):
    for c in range(6, 10):
        print('{}*{}={}'.format(c, i, c * i), end='\t')
    print('')
# 2.
for d in (2, 6):
    print('\n')
    for i in range(1, 10):
        print('\r')
        for j in range(d, d + 4):
            print("%d*%d=%d" % (j, i, i * j), end='\t')    
