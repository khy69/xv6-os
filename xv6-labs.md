# xv6-labs

## lecture1

- Extend os
- System software
- os
  - connect soft and hard
  - coordinate applications

## lab1

### sleep

- a combination:` kernal/type.h & user/user.h`

### Ping-pong

- Two pipes

### Primes

- for clarity

- a divides b->`b%a==0`
- Scale->get rid of increasing numbers(by sieve)
- Parent:filter,child:print the current lowest number
- a process:time series,first to print prime, then to filter for next process 

- redirection pipe:
  - Close fd in time to save resource
  - for read safe(wait for data in pipe or close all write end)

- Multi-process program:
  - just **close write** end after a part of write function
  - consider **wait and exit** as a small operation which would better to be included in a function
  - try **not to use redirection for pipe**, considering debug with printf
  - only **keep one** end for a process(**close another**)
  - Read:a risk function, block process!

### find

- `stat` store metadata for a file(consider a directory as a file)
- Directory is a file containing a sequence of `dirent` structures(include file name and number in current directory)

## xargvs

- learn to **handle string** with a better manner

#### todo

- [ ] dynamically teminate `argvs[]`using a buffer
