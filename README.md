# study_OS
A repo for recording my journey of learning Operating System.


## Keywords to study

### Chapter 2: Operating-System Services
1. Services
* 從一台電腦去想：一台私人電腦包括：
UI, Program Execution(執行), I/O(滑鼠鍵盤),檔案管理,報錯（error detection）,網路（Communication with other cps）

* 如果是實驗室server：
分配運算資源給使用的大家（resource allocation）, 紀錄(Logging), 資安(Protection and security)


![image](https://miro.medium.com/max/1400/1*K7WuBcvuxmBb6mFqihKzSw.png)
[1] 
使用者透過UI傳達想做的事，透過system call傳達指定services，完成後再回傳給使用者。


2. CLI: Command Line interpreter
* 讓人可以直接輸入指令的黑色視窗（一般人可能在設定網路的時候用過）
* 有些implement在kernel裡面，有些則是system program


3. System call
***是什麼?***
* 通常是用C/C++寫的
* 功能：呼叫service
* 三大常見system call API(Application Programming Interface):
    - Win32 API for Windows
    - POSIX API for POSIX-based systems(ex: UNIX, Linux, and Mac OS X)
    - Java API for  Java virtual machine (JVM)
***長怎樣?***
* 以複製檔案的system call為例，會有一連串指令：
    1. 得到

***常見類型***

3. Strategies for designing OS
    * monolithic
    * layered
    * microkernel
    * modular
    * hybrid
4. Process for booting an OS
5. Monitoring OS performance
6. Kernel modules (interacting with a Linux kernel)
    * Design
    * Implement







### Chapter 3: Process
1. Process: 把program run起來
* 比較：
    - process：
        1. 可以兩個process同時跑，就可以平行跑program。（當有兩個CPU時，其實是輪流跑，但是速度很快我們會覺得平行）
        2. active: 主動跑的

    - program：
        1. 一條一條的指令，依照順序跑，沒有平行。
        2. Passive: 被動躺在disk裡面的。
        3. 可以由好幾個process組成。
    - job
    - text: 程式碼。

* program counter 
* Heap: 

stack什麼時候會長比較大？ 有迴圈的時候
Stop at 9:00





## Reference
[1] https://medium.com/@kiyoungju/operating-system-2-os-structures-d8430d1357a9 