# criptograffrase=input("Qual a frase para criptografar: ")

resultado=""
metade=int(len(frase)/2)
for i in range(metade):
   resultado=resultado+frase[metade+i]+frase[i]

if (len(frase)%2==1):
   resultado=resultado+frase[len(frase)-1]

print("Frase criptografada:", resultado)

parte1=''
parte2=""
for i in range(1,len(resultado),2):
   parte1+=resultado[i]
for i in range(0,len(resultado),2):
    parte2+=resultado[i]
print("Frase descriptografada:",parte1+parte2)
