# Shell_echo
一些變化球

# Alternative Cmd

解決一個問題有很多方法，例如 awk、prinf、tr。

* awk 

AWK is a programming language that is designed for processing text-based data, either in files or data streams, or using shell pipes. In other words you can combine awk with shell scripts or directly use at a shell prompt.

However it cosumes the resource a lot. 

* tr

tr is a very useful UNIX command. It is used to transform string or delete characters from the string. 

Various type of transformation can be done by using this command, such as searching and replacing text, transforming string from uppercase to lowercase or vice versa, removing repeated characters from the string etc.

* printf

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

解釋： $ 變數 = 方法名（ ）

    echo $(date)
    2020年 5月19日 週二 19時33分42秒 CST

# ${}

解釋： $ 變數 = {物件名稱呼叫變數}

➜ 指令執行環境 name=foo
  
➜ 指令執行環境 echo ${name}

foo

# echo $-

Shell Flag

➜  指令執行環境 echo $-

himBH
https://chainsawonatireswing.com/2012/02/02/find-out-what-your-unix-shells-flags-are-then-change-them/?from=@


➜  指令執行環境 echo $-

569JNRXZghiklms

