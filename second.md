 <h4>System-Level I/O</h4>
 
 {<======> : connect}
 
 
 CPU[register, ALU(==산술 논리 장치), <-bus interface] <=====>(system <b>bus</b>) I/O Bridge <=====>(memory <b>bus</b>)
 
 <=======>(I/O <b>bus</b>)
 
 USB Controller[keyboard, mouse], Graphics adapter[monitor], disk controller[disk], //====>(expension slots) slots for other devices(like network adapters)
 
 만약 I/O 측에서 CPU에게 일정한 파일들을 저장하라는 요구가 왔을 때.
 1. I/O ==> (system bus) ==> CPU(bus interface==>registerfile<===> ALU)
 2. 저장할 위치에 대한 명령. CPU ==> (system bus ==> I/O bus) ==> disk controller(disk) <CPU는 명령을 내린 이후 다른 명령을 병렬로 처리한다.>
 3. 메인메모리로 저장. disk controller ==> (I/O bus ==> system bus) ==> main memory 
 
 <h4><a href="https://soobindeveloper8.tistory.com/175" type="blank>Unix files</a></h4>
 유닉스 체제 안에서 모든 I/O 장치와 커널은 파일로 표현된다.
 또한 유닉스 파일은 sequence of m bytes다.
 B0, B1, ... , Bk, ... Bm-1
 
 
 <h4>Sequence of Systemcalls</h4>
 
 If you want to open file, you may use function "open()".

 All the file has 'Inode'
 Inode == Address of file in Memory.
 
 cf)<a href="https://thenicesj.tistory.com/217" type="blank">Hard link, Symbolic link</a>
 


 
