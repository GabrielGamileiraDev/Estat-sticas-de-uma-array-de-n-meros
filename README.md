# Estatísticas-de-uma-array-de-números
#Neste programa vamos fazer algumas estatísticas numa lista adicionadas por você.

def numeros_na_lista():
    n = len(listaN)
    return n

def soma_dos_numeros():
    s = sum(listaN)
    return s

def media_dos_numeros():
    m = sum(listaN) / len(listaN)
    return m
    
def maioresN():
   for numeroM in listaN:
       if numeroM > media_dos_numeros():
           return numeroM

def beleza():
    print("_"*30)
    print("\n")
    
def titulo():
    print("ESTATÍSTICAS DA LISTA")


listaN = []
cont = 1
while cont > 0:
    insiraN = int(input("Insira um número para adicionar na sua lista: "))
    listaN.append(insiraN)
    continuar = input("Deseja continuar? Se sim, digite 'S'. Se não, digite 'N'. ")
    if continuar == 'S'.lower():
        cont = 1
    elif continuar == 'N'.lower():
        cont = 0
    else:
        print("Letra errada!")
        while cont > 0:
         continuar = input("Deseja continuar? Se sim, digite 'S'. Se não, digite 'N'. ")

beleza()
titulo()
beleza()
print(f"Essa é a quantidade de números desta lista: {numeros_na_lista()}\n")
print(f"Essa é o resultado da soma entre esse números: {soma_dos_numeros()}\n")
print(f"Essa é a média entre os números da lista: {media_dos_numeros()}\n")
print(f"Esse(s) é(são) o(s) número(s) maior(es) que a média: {maioresN()}")



