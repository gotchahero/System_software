<h1>System software 1</h1>

<h3>Four computer system<h/3>

<h4>User input(or output to user)</h4>
ex)input by C, java, Kernal, vim ,.., database,..
<=> (connect)
<h5>Bridge between User and Computer(compiler..assembler..test editor..database system)</h5>
>> (Union down)
<h4>System and application program(시스템 및 응용프로그램)</h4>
text editor, compiler ...
 
<h4>Operating system(운영체제)</h4>
Controls hardware among various applications and users.
ex)Linux, Window, ...
 
<h4>Computer hardware</h4>
Provide basic computing resources
ex)CPU, DRAM(Memory), ...

 So what is System software?
 ==>Controlling and allocating resources(CPU, Memory, I/o devices(mouse..keyboard ..)

 ==>효율적으로 컴퓨터의 리소스를 관리하고 할당하는 소프트웨어.
 
 <h4>Type of system software(or programming)</h4>
 
 1. File management (ex)Linxu command like cp, cd, ls, rm, mv, rename, ...
 
 2. Status information : ask the system for information like available memory, disk space, number of users ... 
                         and logging and debugging information 
 ex)<a href="https://jangpd007.tistory.com/54/" type="blank">gdb</a>
 
 3. Programming language support (ex) gcc, g++, javac, jython ...(somthing like compile option of linux ...)
 
 4. Programming loading and execution
 ex)<a href="https://ehpub.co.kr/tag/absolute-loader/" type="blank">absolute loader</a>
 
 5. Communication : provide the mechanism for creating virtual connections among processes, users, and computer systems.
 ==> 좀 뒤에 나오는 open() close()의 과정에서 개념을 좀 잡음.
 ex) telenet, ping, kill

 
 <h4>System-Level I/O</h4>
 
 <======> : connect
 
 
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
 


 
