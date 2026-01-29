Git Bash to GitHub Workflow

Command: pwd
Use: Current folder/location check করার জন্য
Description: Print Working Directory

Step-by-Step Folder Setup in Git Bash (C/D/E Drive)
Step 1: Move to D drive
Command: cd /d            (cd → Change Directory)

Step 2: Create a folder
Command: mkdir bongoDev           (mkdir → Make folder)

Step 3: Enter the folder
Command: cd bongoDev

Step 4: Check current directory
Command: pwd

Go one step back to the previous folder (parent directory)
Command: cd ..                  (“dot dot = back”)
[NOTE: 
           1. ধরো তুমি এখন এখানে আছো:
           → /d/bongoDev/project1

           2. এখন যদি লিখো:
           → cd ..

           3. তাহলে যাবে:
           → /d/bongoDev

	4. আর আবার cd .. দিলে:
	→ /d

cd ..  → এক ধাপ পিছনে
cd ../.. → দুই ধাপ পিছনে
]


The (ls) command is used to display a list of all files and folders inside the current directory.

Command: ls
Description: list directory contents 
[NOTE:
	যদি বর্তমান ফোল্ডারে থাকে:
	bongoDev
README.md
index.html
test.py

ls কমান্ড চালালে আউটপুট হবে:
bongoDev  README.md  index.html  test.py

Some useful variations:
ls        → সাধারণ তালিকা
ls -a    → hidden ফাইলসহ সব দেখায়
                          {
                               output: .  ..  bongoDev  README.md  .gitignore
                                 Notes:
                                . = current directory
                                        .. = parent directory
                          }
ls -l     → details (size, permission) সহ দেখায়
ls -la   →সব ফাইল (hidden + normal) দেখানো সাথে detailed info
]



The clear command is also very common in Git Bash. Let me explain it step by step:

Command: clear
[NOTE:
Purpose:
Terminal / Git Bash স্ক্রিন খালি করা
যাতে আগের আউটপুট বা কমান্ডগুলো আর দেখা না যায়
কিন্তু ফাইল বা folder-এর কোনো data মুছে যায় না!
]
Command to go to home directory:

Command: cd ~                 [~ = tilde]
Description: Goes to the home directory of the current user.


Creating a new file named README.md in Git Bash:

Command: touch README.md

[NOTE:
	touch = নতুন ফাইল তৈরি করা
যদি ফাইল আগে থেকেই থাকে, তাহলে শুধু last modified time update করে
	.md= Markdown file (যেটা GitHub এ documentation এর জন্য ইউজ হয়)
]


Editing files(nano / vim):
Command: nano README.md

[NOTE:
	nano editor খুলে তুমি লিখতে পারবে
লিখে Ctrl+O → Save, Ctrl+X → Exit
]


             
Git Bash-এ তুমি README.md ফাইলের ভিতরের content দেখতে চাইলে কয়েকটা সহজ command ব্যবহার করতে পারো:

Command: cat README.md
