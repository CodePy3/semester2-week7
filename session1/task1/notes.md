C error message:

Done!
*** stack smashing detected ***: terminated
Aborted (core dumped)

-> provides no line numbers or intuitive errors that make sense based on the source code

Python error message:

Traceback (most recent call last):
  File "/workspaces/semester2-week7/session1/task1/crash.py", line 9, in <module>
    assign_values(data)
  File "/workspaces/semester2-week7/session1/task1/crash.py", line 5, in assign_values
    x[i] = (i + 1) * (i + 1);
    ~^^^
IndexError: list assignment index out of range

-> provides line numbers 9 and 5
-> line 9 is where the function that causes the crash is called
-> line 5 is the line in the function where the error occurs
-> tells us it is an index error which when compared with the source code makes it very obvious you have accessed an array index that does not exist