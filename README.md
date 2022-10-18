## Masm組合語言HelloWorld補上傳 
```asm
	MOV AX,@DATA          ; 將DATA放入AX
	MOV DS,AX             ; 將AX放入DS
	MOV DX,OFFSET mesg    ; DX取mesg偏移量
	MOV AH,09H	      ; 打印DX
	INT 21H               ; 調用系統命令
	MOV AH,4CH            ; 結束當前進程
	INT 21H               ; 調用系統命令
```
