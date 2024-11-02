# A-Z
org 100h
mov dx,offset output
mov ah,9
int 21h
mov cx,26
mov al,'A'
mov dl,al
print:
mov ah,2
int 21h
inc dl
loop print
mov ah,4Ch
int 21h     
output db "A-Z are: $"
