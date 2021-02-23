# Projeto-Poo
#2º Informática Matutino
#Disciplina:Programação Orientada a Objetos 
#integrantes: Amanda Vitória e Kevelyn Maria

main.py
from Pessoa import Pessoa
from Pizza import Pizza
from Pedido import Pedido

pessoa=Pessoa()

pizza= Pizza()

pedido=Pedido()


pedido.valor(pizza)

pedido.comprar(pessoa,pizza)

Pedido.py
class Pedido:
  def __init__(self):
    self._pessoa=None
    self._pizza=None

  def valor(self,pizza):
    self._pizza=pizza

  def comprar(self,pessoa,pizza):
    self._pessoa=pessoa
    self._pizza=pizza
