menu = """

[d] Depositar
[s] Sacar
[e] Extrato
[q] Sair

=> """

saldo = 0
limite = 500
extrato = ""
numero_saques = 0
LIMITE_SAQUES = 3

while True:

  opcao = input(menu)

  if opcao == "d":
    valor = float(input("\nInforme o valor do depósito: "))

    if valor > 0:
      saldo += valor
      extrato += f"\nDepósito R$ {valor:.2f}\n"

    else:
      print("\nInforme um valor válido!")

  elif opcao == "s":
      valor = float(input("\nInforme o valor do saque: "))

      excedeu_saldo = valor > saldo

      excedeu_limite = valor > limite

      excedeu_saques = numero_saques >= LIMITE_SAQUES

      if excedeu_saldo:
          print("\nSaldo insuficiente!")

      elif excedeu_limite:
          print("\nLimite ultrapassado!")

      elif excedeu_saques:
          print("\nLimite de saques atingido!")

      elif valor > 0:
          saldo -= valor
          extrato += f"Depósito R$ {valor:.2f}\n"
          numero_saques += 1

      else:
            print("\nInforme um valor válido!")

  elif opcao == "e":
          print(f"\nSaldo: R$ {saldo:.2f}")

  elif opcao == "q":
        break

  else:
        print("\nEscolha uma opção válida!")