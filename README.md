# cadastrousuario
Cadastro de usuário em Python
class Usuario:
    def __init__(self, nome, endereco, telefone, email, cpf, foto):
        self.nome = nome
        self.endereco = endereco
        self.telefone = telefone
        self.email = email
        self.cpf = cpf
        self.foto = foto

def cadastrar_usuario():
    nome = input("Digite o nome do usuário: ")
    endereco = input("Digite o endereço do usuário: ")
    telefone = input("Digite o telefone do usuário: ")
    email = input("Digite o e-mail do usuário: ")
    cpf = input("Digite o CPF do usuário: ")
    foto = input("Digite o nome da foto do usuário: ")

    usuario = Usuario(nome, endereco, telefone, email, cpf, foto)
    return usuario

def main():
    # Cadastro do usuário
    usuario = cadastrar_usuario()

    # Exibindo os dados cadastrados
    print("\nDados do usuário cadastrado:")
    print("Nome:", usuario.nome)
    print("Endereço:", usuario.endereco)
    print("Telefone:", usuario.telefone)
    print("E-mail:", usuario.email)
    print("CPF:", usuario.cpf)
    print("Foto:", usuario.foto)

if __name__ == "__main__":
    main()
