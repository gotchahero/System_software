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
 
 
 Sequence of Systemcalls

 All the file has 'Inode'
 Inode == Address of file in Memory.
 cf)<a href="https://thenicesj.tistory.com/217" type="blank">Hard link, Symbolic link</a>


 
