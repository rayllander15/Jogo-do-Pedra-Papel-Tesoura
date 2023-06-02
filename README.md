# Jogo-do-Pedra-Papel-Tesoura
Jogo do Pedra, Papel e Tesoura, o jogo contém a máquina e o player, escolha uma das opções e veja o vencedor. Jogo identifica quantos jogadores jogou o jogo.


from random import randint
from time import sleep

#computador(O computador vence, ou seja o computador se refere a máquina. Vale para perder também.)
#jogador(O jogador vence, se refere ao player. O vale para perder também.)

computador = randint(1,3)

cont = 0

lista= list()
nome = list()
lista = str(input('\033[34mQual nome do jogador? \033[m'))
nome.append(lista[:])

print(f'''\033[31;34mVamos começar a brincadeira do JOKENPO {nome}, para começarmos você tem que escolher uma das opções abaixo:
[1] PEDRA
[2] PAPEL
[3] TESOURA\033[m''')

jogador= int(input('\033[33mFaça sua escolha: \033[m'))
#print(f'{jogador} escolheu {opção} e o computador escolheu {computador}' )
print('\033[35m~\033[m'*10)
print('\033[33m   Jo\033[m')
sleep(0.5)
print('\033[33m   Ken\033[m')
sleep(0.5)
print('\033[33m   Pô!\033[m')
sleep(0.5)
print('\033[35m~\033[m'*10)

if jogador == 1: #Pedra
    if computador == 1:
        print(f'\033[34m{nome}\033[m \033[31mescolheu PEDRA e o\033[m \033[34mCOMPUTADOR\033[m \033[31mescolheu PEDRA, EMPATE!\033[m')
    elif computador == 2:
        print(f'\033[34m{nome}\033[m \033[31mescolheu PEDRA e o\033[m\033[34m COMPUTADOR\033[m \033[31mescolheu PAPEL, COMPUTADOR VENCE!\033[m')       
    elif computador == 3:
        print(f'\033[34m{nome}\033[m \033[31mescolheu PEDRA e o\033[m \033[34mCOMPUTADOR\033[m \033[31mescolheu TESOURA,\033[m \033[34m{nome}\033[m \033[31mVENCE!\033[m')       
elif jogador == 2: #Papel
    if computador == 1:
        print(f'\033[34m{nome}\033[m \033[31mescolheu PAPEL e o \033[34mCOMPUTADOR\033[m \033[31mescolheu PEDRA,\033[m \033[34m{nome}\033[m \033[mVENCE! \033[m')          
    elif computador == 2:
        print(f'\033[34m{nome}\033[m \033[31mescolheu PAPEL e o\033[m \033[34mCOMPUTADOR\033[m \033[31mescolheu PAPEL, EMPATE!\033[m')            
    elif computador == 3:
        print(f'\033[34m{nome}\033[m \033[31mescolheu PAPEL e o\033[m \033[34mCOMPUTADOR\033[m \033[31mescolheu TESOURA, COMPUTADOR VENCE!\033[m')           
elif jogador == 3: #TESOURA
    if computador == 1:
        print(f'\033[34m{nome}\033[m \033[31mescolheu TESOURA e o\033[m \033[34mCOMPUTADOR\033[m \033[31mescolheu PEDRA, COMPUTADOR VENCE!\033[m')
    elif computador == 2:
        print(f'\033[34m{nome}\033[m \033[31mescolheu TESOURA e o\033[m \033[34mCOMPUTADOR\033[m \033[31mescolheu PAPEL,\033[m \033[34m{nome}\033[m\033[31m VENCE!\033[m')           
    elif computador == 3:
        print(f'\033[34m{nome}\033[m \033[31mescolheu TESOURA e o\033[m \033[34mCOMPUTADOR\033[m \033[31mescolheu TESOURA, EMPATE!\033[m')
        
while True:
    resp =str(input('\033[33mReiniciar o game?[S/N]:  \033[m')).upper().strip()[0]
    cont +=1
    if resp == 'S':       
        nome=str(input('\033[34mQual nome do jogador? \033[m'))
    
        print(f'''\033[31;34mVamos começar a brincadeira do JOKENPO {nome}, para começarmos você tem que escolher uma das opções abaixo:
        [1] PEDRA
        [2] PAPEL
        [3] TESOURA\033[m''')

        jogador= int(input('\033[33mFaça sua escolha: \033[m'))
        #print(f'{jogador} escolheu {opção} e o computador escolheu {computador}' )
        print('\033[35m~\033[m'*10)
        print('\033[33m   Jo\033[m')
        sleep(0.5)
        print('\033[33m   Ken\033[m')
        sleep(0.5)
        print('\033[33m   Pô!\033[m')
        sleep(0.5)
        print('\033[35m~\033[m'*10)
        
        if jogador == 1: #Pedra
            if computador == 1:
                print(f'\033[34m{nome}\033[m \033[31mescolheu PEDRA e o\033[m \033[34mCOMPUTADOR\033[m \033[31mescolheu PEDRA, EMPATE!\033[m')                
            elif computador == 2:
                print(f'\033[34m{nome}\033[m \033[31mescolheu PEDRA e o\033[m\033[34m COMPUTADOR\033[m \033[31mescolheu PAPEL, COMPUTADOR VENCE!\033[m')                
            elif computador == 3:
                print(f'\033[34m{nome}\033[m \033[31mescolheu PEDRA e o\033[m \033[34mCOMPUTADOR\033[m \033[31mescolheu TESOURA,\033[m \033[34m{nome}\033[m \033[31mVENCE!\033[m')                
        elif jogador == 2: #Papel
            if computador == 1:
                print(f'\033[34m{nome}\033[m \033[31mescolheu PAPEL e o \033[34mCOMPUTADOR\033[m \033[31mescolheu PEDRA,\033[m \033[34m{nome}\033[m \033[mVENCE! \033[m')                
            elif computador == 2:
                print(f'\033[34m{nome}\033[m \033[31mescolheu PAPEL e o\033[m \033[34mCOMPUTADOR\033[m \033[31mescolheu PAPEL, EMPATE!\033[m')                
            elif computador == 3:
                print(f'\033[34m{nome}\033[m \033[31mescolheu PAPEL e o\033[m \033[34mCOMPUTADOR\033[m \033[31mescolheu TESOURA, COMPUTADOR VENCE!\033[m')           
        elif jogador == 3: #TESOURA
            if computador == 1:
                print(f'\033[34m{nome}\033[m \033[31mescolheu TESOURA e o\033[m \033[34mCOMPUTADOR\033[m \033[31mescolheu PEDRA, COMPUTADOR VENCE!\033[m')               
            elif computador == 2:
                print(f'\033[34m{nome}\033[m \033[31mescolheu TESOURA e o\033[m \033[34mCOMPUTADOR\033[m \033[31mescolheu PAPEL,\033[m \033[34m{nome}\033[m\033[31m VENCE!\033[m')                
            elif computador == 3:
                print(f'\033[34m{nome}\033[m \033[31mescolheu TESOURA e o\033[m \033[34mCOMPUTADOR\033[m \033[31mescolheu TESOURA, EMPATE!\033[m')
            
    if resp =='N':
        break

print('\033[31m-=\033[m'*15)
print(f'\033[34mAo todo temos {cont} jogadores\033[m') 
print('\033[31m-=\033[m'*15)   
