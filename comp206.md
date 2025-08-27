
- TODO: fork with text files
- TODO: learn how char and strings work

### C Programming
```C
int main (int argc, char *argv[]){
	int final, i, init;
	final=-1;
	
	if (argc>1){
		init = atoi(argv[1]);
		final = 1;
	}
	
	if (init >= 0){
		for (i=1;i<init+1;i++){
			final = final * i;
		}
		printf ("The input value is %d and its factorial is %d", init, final);
		
	} else {
		printf ("Error: NUMBER is either missing or negative");
	}
	return 0;
	
}
```

#### Q2
```C
long int result;

void factorial (int n){
	if (n==0){
		result=1
	} else {
		factorial(n-1);
		result*=n;
	}
}

recursion.h
extern long int result;
void factorial(int n);
```

``` make
makefile
recursion: recursion.o main.o
gcc -o factorials recursion.o main.o

recrusion.o: recursion.c recursion.h
gcc -c cursion.c

main.o: main.c recursion.h
gcc -c main.c
```

### arrays and characters
```C
#include <string.h>


```
### bash 
- read and executed line-by-line by the Bash interpreter **at runtime**.
- the default script ran on linux login is .bash_profile
- 
```bash
#!/bin/bash
filename="$1"
word="$2"

if [ $# -ne 2 ]; then
    echo "Error: Exactly 2 arguments required (filename and word)."
    exit 1
fi

if [ ! -f "$filename" ]; then
    echo "Error: File '$filename' does not exist."
    exit 2
fi

if grep -qw "$word" "$filename"; then
    echo "The file $filename contains the word $word."
else
    echo "$word not found in file $filename."
fi

exit 0
```

```bash
#!/bin/bash
alias add 'git add'
alias commit 'git commit'
if[! -d Project/backup]; then; mkdir Project/backup; fi
cp Project/source/*.c Project/source/*.h Project/backup
git pull ssh://master@git.repo
chmod g-w+rx Project/backup
```

### GDB
##### 1. **Compile with Debug Info**
add the -g flag to compile with source code and symbol table
`gcc -g program.c -o program`

##### 2. **Start GDB**
`gdb ./program`

##### 3. **Set a Breakpoint**
`break main              # at the start of main break 10                # at line 10 break function_name     # before a function runs`

##### 4. **Run the Program**

`run`

##### 5. **Step Through Code**
`next      # go to next line (skips over functions) step      # go into function calls continue  # run until next breakpoint or program ends`

##### 6. **Inspect Variables**
`print x       # shows the value of variable x display x     # automatically shows x after every step`

##### 7. **Backtrace on Crash**
`backtrace     # shows function call stack`

##### 8. **Exit GDB**
`quit`

### Cross Process Communication 
- use files when the processes are not in the same computer
- use sockets when not on the same network
- use shared memory when operating on the same structure
- use environment variables when operating in the same shell


### Make files
```make
all: mod1.o mod2.o mod3.o // to build all i need mod1-3.o
	gcc -o exe_release mod1.o mod2.o mod3.o

debug: mod1.o mod2.o mod3.o
	gcc -g -o exe_debug mod1.o mod2.o mod3.o

profile: mod1.o mod2.o mod3.o
	gcc -pg -o exe_profile mod1.o mod2.o mod3.o

clean:
	rm -f *.o exe_*

mod1.o: mod1.c
	gcc -c mod1.c

mod2.o: mod2.c
	gcc -c mod2.c

mod3.o: mod3.c // too build mod3.o i need mod3.c
	gcc -c mod3.c

```

### GIT
```git
git init - in an empty dir with the dir name being the git repo intended name
git add
git commit -m "message"
git push
git pull
git branch branchName
git checkout branchName
git merge
```
##### Advantages
- **easier access to change history (backup only keeps a single backup instance)**
- **better suited for team work (everyone backs up to the same place)**
- **easier to maintain (permissions, moveable)**
- **easier to know who modified what and when (tracks programmers