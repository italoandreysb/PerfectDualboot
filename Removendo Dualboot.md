# Removendo o linux do dualboot com windows 10 ou 11


1. abra o CMD, acesse o diskpart e liste os discos e selecione o desejado,  no meu caso o "disco 0"::
```	
diskpart
list disk
sel disk 0
```
2. Selecione o volume, geralmente é um **FAT32** com **100MB** do tipo **SISTEMA**, no meu caso é o volume 1:
```
list vol
sel vol 1
```
3. Monte a partição e dê uma letra, no meu caso escolhi a letra "X":
```
assign letter=x
```
4. Saia do diskpart:
```
exit
``` 
5. Acesse a partição montada:
``` 
x:
```
6. Acesse o diretório dentro da partição:
```
cd efi
```
7. Remova o arquivo de inicialição da sua distribuição linux, no meu caso se chama "ubuntu":
```
rmdir /S ubuntu
```

Obs: A partição de 100MB não pode ser apagada

Fonte: [Youtube: Como remover o Grub da inicialização do Windows](https://www.youtube.com/watch?v=agbQx9XQmMo)