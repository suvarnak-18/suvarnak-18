**By Referring to C-based Lab videos and RISC-V-based lab videos**

**Snapshots of the compiled C code and RISC-V**

**Step 1: check whether the leafpad is installed in ur machine by using the commands
leafpad sum1ton.c& (sum1ton.c is the file name)
If the leafpad editor is opened without any errors then type the C code.**
****If the leafpad is not installed in ur machine then install by using the following command**

**sudo snap install leafpad****
![leafpad_install](https://![task31](https://github.com/suvarnak-18/suvarnak-18/assets/160591416/4f26d53e-2f68-401e-9157-8b51bc891d5e)



****Step 2: Writing the C code in the leafpad editor** using the following command

**leafpad sum1ton.c&**
![Leafpad_editor](https://![task32](https://github.com/suvarnak-18/suvarnak-18/assets/160591416/6119e131-f6fd-4957-b33e-3f33a510699d)


**Step 3: After writing the C code save the editor by Ctrl+s**

**Step 4: Check for the errors by using the following command(compilation step)**

**gcc sum1ton.c**
![complie the C Code](https://![task33](https://github.com/suvarnak-18/suvarnak-18/assets/160591416/3d40b464-3315-480f-815e-d6eb8e79c97d)


**Step 5: Check the output by using the command**

**./a.out**
![C Code Execution with results ](https://![task33](https://github.com/suvarnak-18/suvarnak-18/assets/160591416/92a336c7-c7cf-4f0d-8cf5-12b652bbd691)







**The results will be displayed as** 

**Sum of numbers from 1 to 500 is 125250**


********************************************************RISCV Compilation and Execution*****************************************************

**Step 1: View the C Code in the editor window using the following command**

**cat sum1ton.c**
![view in the C code in notepad](https://github.com/Abdulbitm/Abdul/assets/160620896/cd8e147a-6cf3-444d-a76c-1b24ed063636)

**Step 2: Compile the code in riscv using the following command**

**riscv64-unknown-elf-gcc -O1 -mabi=lp64 -march=rv64i -o sum1ton.o sum1ton.c**
![complie riscv](https://github.com/Abdulbitm/Abdul/assets/160620896/b85e4975-9bc1-4258-8091-6904692328cc)

**Step 3: The ls ltr command in Linux is used to list the contents of the current directory in long format, sorted by last modified time in reverse order.**

**use the command**

**ls -ltr sum1ton.c**

![view the directory contents](https://github.com/Abdulbitm/Abdul/assets/160620896/c7dd20be-b896-4d19-af98-077590a23b14)


![long directory content](https://github.com/Abdulbitm/Abdul/assets/160620896/3e2e473a-9f55-4bec-8ed3-4bd2732efbee)

**Search for the Main and check the instructions of the C code execution. It has 15 instructions in the C execution**

![checking instructions_in_main_C_Code_15_instructions](https://github.com/Abdulbitm/Abdul/assets/160620896/8d7d1502-a997-403d-a2cc-fcd459962a43)

![checking instructions_in_main_C_Code_15_instructions_highlighted](https://github.com/Abdulbitm/Abdul/assets/160620896/0a07ba3e-4a3d-41a7-a158-3ef976ce0292)


**Step 4:**

**riscv64-unknown-elf-gcc -Ofast -mabi=lp64 -march=rv64i -o sum1ton.o sum1ton.c**

![12 instructions with Ofast](https://github.com/Abdulbitm/Abdul/assets/160620896/f2ebdc19-c3a6-494d-a25d-6d71c2811440)



![12 instructions with Ofast_1](https://github.com/Abdulbitm/Abdul/assets/160620896/4904feb4-c3ab-4337-976c-9a94bacbf85a)






