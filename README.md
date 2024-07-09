(NOTE - All the commands executed in ubuntu virtual machine )
# LEVEL - 1 
# To Extract the system calls
# we use command 
  
    strace -o mkdir_output.txt mkdir my_directory
# this will create a directory named "my_directory"
# and give all system calls made by mkdir to file named mkdir_output.txt
# To view the saved System Calls - Open the mkdir_output.txt



# LEVEL -2 
# make file of any name(for ex- info) in text editor and use extension ".c"
# code to print name and branch
            #include <iostream.h> 
            #include <stdio.h> 
                int main() {
                            print("NAME : A");
                            print("DEPT : P");
                            return 0;
             }
# then save 
# To compile the file , open terminal and give command 

              gcc -o test.out info.c
# This will change the info.c file into a executable file name "test.out"
# Now to extract syestem calls , give command in the terminal 
             strace -o test_syscalls.txt ./test.out
# This will give the output in a text file named "test_syscalls.txt"
