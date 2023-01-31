## 作業系統的演進:
 <br>&emsp;&emsp;電腦的運作分為程式、硬體與作業系統三個部分，作業系統連結了其他兩個部分。作業系統的演進可以分為 Mainframe Systems、Computer-system architecture、Special-purpose Systems 三個部分。 <br>

1. Mainframe Systems:
<br>&emsp;&emsp;是最早期的作業系統，最早的電腦（Mainframe）昂貴、體積大，而且也只能用來管理專一的事情；
<br>Mainframe 一開始是使用一種叫做 Batch 的技術，將程式打在卡片上，讓它可以在電腦上面執行，此時的電腦一次也只能處理一個程式，要等這個動作結束之後才能接續執行下個指令，因此稱為 Batch

- 作業流程：
<br>・One job at a time

<br>&emsp;&emsp;・No interaction between users and jobs

<br>&emsp;&emsp;・CPU is often idle

<br>
- 缺點:
<br>&emsp;&emsp;因 I/O 時間通常很大，故，CPU 必須不停監控才能完成 I/O 循環所以閒置過長，為了有效利用資源，因此發展出 Multi-programming，
<br>用快速切換的方式讓多個使用者同時使用一台電腦。要完成 CPU 多工必須先引入 Spooling 的概念，也就是利用 I/O 與 CPU 運作的的時間差，讓 I/O 在處理任務時 CPU 不需介入，利用這段時間處理其它問題。


<br>&emsp;&emsp;有了 Multi-programming 之後，使用者發現電腦的執行效率雖然變高了，但因為沒有互動，在本質上電腦還是做跟之前一樣的事情。為了改善使用者體驗，電腦科技開始往互動功能發展，發展出 Time-sharing 的概念：CPU 捕捉到使用者的 I/O 即時作出回應，讓使用者產生互動感，同時利用 CPU 計算速度很快的特性，快速在每個程式間切換執行緒，讓使用者感覺電腦正在處理複數指令，產生多人同時使用電腦的感覺。
