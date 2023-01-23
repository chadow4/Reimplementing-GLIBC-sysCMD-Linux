# Reimplementing GLIBC, system commands and SHELL

## About the Project

In this project, the standard library was recreated from scratch as well as system commands and a SHELL in order to execute them.

### Developped with :
* C (only system Call)

## Getting Started

The project has a makefile in order to compile the library, the Test file, the SHELL file and the different system commands.



#### the library contains 4 files :

- mini_string.c

  - mini_printf
  - mini_scanf
  - mini_exit_string
  - mini_strlen
  - mini_strcpy
  - mini_strcmp
  - stringToInt (ATOI)
  - intToString (ITOA)
  - mini_perror
  
- mini_memory.c

  - mini_calloc
  - mini_free
  - mini_exit
 
- mini_io.c
  
  - mini_fopen
  - mini_fread
  - mini_fwrite
  - mini_fflush
  - mini_fclose
  - mini_exit_io
  - mini_fgetc
  - mini_fputc
  
- mini_lib.h

###### The SHELL and the system commands use only this library !!

#### List of system commands implemented : 
- mini_touch.c ```mini_touch file```
- mini_cp.c ``` mini_cp file1 file2```
- mini_echo.c ```mini_echo message```
- mini_cat.c ```mini_cat file```
- mini_head.c ```mini_head -n nline file```
- mini_tail.c ```mini_tail -n nline file```
- mini_clean.c ```mini_clean file```
- mini_grep.c ```mini_grep word file```
- mini_wc.c ```mini_wc file```

#### Test File : 
- main.c

#### SHELL File : 
- shell.c



### COMMANDS : 
- Compile All FIles : ```make all```
- Clear All FIles : ```make cleanall```
- Lunch Shell : ```./mini_shell```
- Lunch TestFile : ```./test```


## Credits : 

Created by Julien SANCHEZ 


task : 

mini_chmod : OK
mini_ls :
mini_mv : ok
mini_quickdiff : ok mais a fix
mini_ln : ok
mini_mkdir : ok
mini_rm : ok
mini_rmdir : ok 

mini_export :
mini_cd : ok
mini_getenv : ok 
mini_env : ok