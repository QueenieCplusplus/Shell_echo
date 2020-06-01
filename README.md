# Shell_echo
一些變化球

# Common Variable

    $0	Current Working Script Doc Name.
    
    
    $n	Param Number to pass thru the function. $1 means Arg1, $2 means Arg2...and so on.
    $?      int type. retrun value or status of above function.
    
    
    $#	int type. The Arg Arregate Number passing thru function or Scripts.
    $*	All The Params passing thru function or Scripts.
    $@	All The Params passing thru function or Scripts. (there are also usage of escaping tool within different meaning.)
    

# Alternative Cmd

解決一個問題有很多方法，例如 awk、prinf、tr、 > or >>。

http://dannysun-unknown.blogspot.com/2016/11/shell-script-awk-sed.html

* awk 

AWK is a programming language that is designed for processing text-based data, either in files or data streams, or using shell pipes. In other words you can combine awk with shell scripts or directly use at a shell prompt.

However it cosumes the resource a lot. 

* tr

tr is a very useful UNIX command. It is used to transform string or delete characters from the string. 

Various type of transformation can be done by using this command, such as searching and replacing text, transforming string from uppercase to lowercase or vice versa, removing repeated characters from the string etc.

* printf

# > & >>

    > 也等同於 1>

overwrite the content body in target file.

1 代表標準輸出 ; 如果是 2 則是標準錯誤輸出 ; & 則是標準輸出和標準錯誤輸出一起。 


     >>

to add on after the content body in target file.

# echo $$

Show PID

    echo $$
    1264

# var = val, execute $var

➜  指令執行環境 1=2  

➜  指令執行環境 echo $1

2

# echo -n

解釋：讓訊息輸出時不自動換行。

    ✗ echo -n 'I luv Poupou, '; echo 'who is the most wondeful companion in the world.'

    I luv Poupou, who is the most wondeful companion in the world.


# $()

command substitution

解釋： $ 變數 = 方法名（ ）

也可以等同於 $() =  ` `

加強版本為 $(()) 或是 $[[]]

    echo $(date)
    2020年 5月19日 週二 19時33分42秒 CST

# ${}

variable within range

解釋： $ 變數 = {物件名稱呼叫變數}

也可以等同於 $var = ${var}

➜ 指令執行環境 name=foo
  
➜ 指令執行環境 echo ${name}

foo

# []

to matche the test pattern

也可以等同於 $[  ] = [  ]

加強版本為 $(()) 或是 $[[]]

# [0-9]

* [0-9]

數字字元集合：

* [a-zA-Z0-9]

數字和英文字母集合。

* [m-pA-C3-6]

字元區段集合。

* [abc]

a 或 b 或 c。

* [abc][123]

矩陣的字元組合概念。

# echo $-

Shell Flag

➜  指令執行環境 echo $-

himBH
https://chainsawonatireswing.com/2012/02/02/find-out-what-your-unix-shells-flags-are-then-change-them/?from=@


➜  指令執行環境 echo $-

569JNRXZghiklms

# so on...

/ 跳脫字元

~ 位置求反

＆ 和

｜ 或

＆＆ 邏輯和

｜｜ 邏輯或

> > 右位移

< < 左位移

# Ref Doc

https://swcarpentry.github.io/shell-novice/reference/

http://benjr.tw/97062






