# Olá Mundo com Flask

Minha primeira aplicação para criação do projeto simples "Olá Mundo"
Explicando linha a linha do código: 


### from flask import Flask
Importando o Flask:
from flask import Flask: Isso importa a classe Flask do módulo flask. O Flask é o principal objeto da minha aplicação web.


### app = Flask(__name__)
Criando uma Instância do Flask:
app = Flask(__name__): Cria uma instância da classe Flask. O argumento __name__ é usado para determinar a localização dos templates e arquivos estáticos.


### @app.route('/')
def hello_world():
    return 'Olá, Mundo!'
Definindo uma Rota e uma Função:
@app.route('/'): Isso define uma rota. Neste caso, é a rota raiz ('/'). Quando alguém acessa a raiz do meu site, a função seguinte será executada.
def hello_world():: Define a função associada à rota. Neste caso, a função se chama hello_world.
return 'Olá, Mundo!': Esta função retorna a string "Olá, Mundo!" como resposta à solicitação da rota.


### if __name__ == '__main__':
    app.run(debug=True)
Iniciando o Servidor Flask:
if __name__ == '__main__':: Garante que o servidor seja iniciado apenas se este script for executado diretamente, não se for importado como um módulo.
app.run(debug=True): Inicia o servidor Flask. O argumento debug=True ativa o modo de depuração, o que é útil durante o desenvolvimento.

Essencialmente, este é um aplicativo Flask muito simples. Ele cria um servidor web que responde à rota raiz com a mensagem "Olá, Mundo!". Quando você executa o arquivo app.py, o servidor Flask é iniciado e você pode acessar a aplicação no navegador em http://127.0.0.1:5000/.
