# lig4.py
TRABALHO DE PROGRAMAÇÃO ORIENTADA A OBJETOS

  import random

print("Bem vindos ao LIG 4")
print("-------------------")

Possiveisletras = ["A", "B", "C", "D", "E", "F", "G"]
Tabuleiro = [["", "", "", "", "", "", "",], ["", "", "", "", "", "", "",], ["", "", "", "", "", "", "",], [
    "", "", "", "", "", "", "",], ["", "", "", "", "", "", "",], ["", "", "", "", "", "", "",]]
linhas = 6
colunas = 7


def printTabuleiro():
    print("\n    A   B   C   D   E   F   G", end="")
    for x in range(linhas):
        print("\n  +----+----+----+----+----+----+")
        print(x, " |", end="")
        for y in range(colunas):
            if (Tabuleiro[x][y] == "🔵"):
                print("", Tabuleiro[x][y], end=" |")
            elif (Tabuleiro[x][y] == "🔴"):
                print("", Tabuleiro[x][y], end=" |")
            else:
                print(" ", Tabuleiro[x][y], end=" |")
    print("\n +----+----+----+----+----+----+")


def modificarTurno(espacoEscolhido, turno):
    Tabuleiro[espacoEscolhido[0]][espacoEscolhido[1]] = turno


printTabuleiro()
