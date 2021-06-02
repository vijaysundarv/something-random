# something-random :beers:

## 1. Print numbers between 1 to 10 in a random order.
### On Linux :zap:
Linux gives you a simple utility called ***shuf*** that comes part of the GNU CoreUtils.
What does *shuf* do?
It writes a random permutation of the input lines to standard output. Run the below commands to know more about ***shuf***.
```bash  
$ shuf --help
# OR
$ man shuf
```
How do you print numbers from 1 to 10 in a random order?
```bash  
$ shuf -i 1-10 -n 10
4  
2  
10 
6  
7  
1  
9  
8  
5  
3  
# To print all the above numbers in the same line, you can use various other linux utilities such as sed, awk, etc... but let's use tr
$ shuf -i 1-10 -n 10 | tr "\n" " "
1 4 2 5 3 8 6 10 9 7
$ shuf -i 1-10 -n 10 | tr "\n" " "
6 3 7 1 2 5 4 10 8 9
```
> Extra TIP: To print numbers in a sequential order, run **seq 10** in the terminal. It prints numbers from FIRST to LAST, in steps of INCREMENT.

*The above can also be used within a shell script as required.*

### On MacOS :zap:
***shuf*** is not installed by default in macOS. To run ***shuf*** commands, run the below in macOS.
```bash
$ brew install coreutils
$ shuf -i 1-10 -n 10 | tr "\n" " "
7 1 8 2 10 3 5 6 4 9
```

## 2. Metrics to monitor a server / application. :desktop_computer:	

[Click here](https://github.com/vijaysundarv/something-random/blob/main/Monitoring_Server_Applications.pdf) to view the documented solution.

