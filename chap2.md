# Text Manipulation (thao tác trên văn bản)

### Taking the Head
**head *diretory of filename***: display the first 10 lines of a file. If you want to see more or fewer than the default, use dash (-)
   Ex: head /etc/snort/snort.conf : the default
       head -20 /etc/snort/snort.conf : the first 20 lines
       
### Grabing the tail
**tail *diretory of filename***: show 10 last lines of a file, some of the last *include* lines of *the rules* files. and use dash to adjust the lines you want to see.
   Ex: tail /etc/snort/snort.conf
       tail -20 /etc/snort/snort.conf

### Numbering the lines
**nl *diretory of filename*** : display a file with line numbers
    Ex: nl /etc/snort/snort.conf
    
### Filtering text with grep
cat *diretory of filename* | grep *content* : filter the content of a file for display.
Ex: cat /etc/snort/snort.conf | grep output
    > see all lines that include the word output in *snort.conf*

   
