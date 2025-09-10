nomes = []
carnes = []
bebidas = []

def entrada_valida(suzu):
    while True:
        valor = input(suzu).strip()
        if all(c.isalpha() or c.isspace() for c in valor) and valor != "":
            return valor
        else:
            print("Use apenas caracteres.")

while True:
    print("--- MENU ---")
    print("1: Cadastrar")
    print("2: Listar")
    print("3: Atualizar")
    print("4: Remover")
    print("5: Sair")

    escolha = input("Escolha uma opção: ").strip()

    if escolha == "1":
        nome = entrada_valida("Nome: ")
        carne = entrada_valida("Carne: ")
        bebida = entrada_valida("Bebida: ")

        if nome in nomes:
            print("Já existe esse nome cadastrado!")
        else:
            nomes.append(nome)
            carnes.append(carne)
            bebidas.append(bebida)
            print(f"{nome} cadastrado com sucesso!")

    elif escolha == "2":
        if len(nomes) == 0:
            print("Cadastre um nome primeiro.")
        else:
            print("\n--- Lista de Cadastros ---")
            for i in range(len(nomes)):
                print(f"{i}: {nomes[i]} - {carnes[i]} + {bebidas[i]}")

    elif escolha == "3":
        if len(nomes) == 0:
            print("Cadastre um nome primeiro.")
        else:
            print("--- Lista de Cadastros ---")
            for i in range(len(nomes)):
                print(f"{i}: {nomes[i]} - {carnes[i]} + {bebidas[i]}")
            
            nome = entrada_valida("Qual nome deseja atualizar? ")
            if nome in nomes:
                i = nomes.index(nome)

                print("Qual a opção para atualizar?")
                print("1: Carne")
                print("2: Bebida")
                print("3: Ambos")
                opcao = input("Escolha uma opção: ").strip()

                if opcao == "1":
                    carnes[i] = entrada_valida("Nova carne: ")
                    print("Nova carne adicionada.")
                elif opcao == "2":
                    bebidas[i] = entrada_valida("Nova bebida: ")
                    print("Nova bebida adicionada.")
                elif opcao == "3":
                    carnes[i] = entrada_valida("Nova carne: ")
                    bebidas[i] = entrada_valida("Nova bebida: ")
                    print("Nova carne e bebida adicionados com sucesso.")
                else:
                    print("Opção inválida, escolha uma das opções.")

            else:
                print("Nome não encontrado.")

    elif escolha == "4":
        if len(nomes) == 0:
            print("Cadastre um nome primeiro.")
        else:
            print("--- Lista de Cadastros ---")
            for i in range(len(nomes)):
                print(f"{i}: {nomes[i]} - {carnes[i]} + {bebidas[i]}")
            
            nome = entrada_valida("Qual nome quer remover?")
            if nome in nomes:
                i = nomes.index(nome)
                del nomes[i]
                del carnes[i]
                del bebidas[i]
                print(f"{nome} foi removido.")
            else:
                print("Nome não encontrado.")

    elif escolha == "5":
        print("Tchau!")
        break

    else:
        print("Opção inválida. Tente novamente.")








  #Lucas Vedovello(Criou a função cadastrar e o código base.), Pietro Coelho(Criou a função sair.) , Matheus Suzuki(Criou as função atualizar e Listar.), Pedro Raposo(Criou a função sair.), Vinicius Perozzo(Passou o código a limpo corrigindo os erros.), Vinicius Rhis(Definiu as variáveis.).
  
