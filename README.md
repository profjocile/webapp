# webapp
 Minha aplicação web com Python
1. Criar uma Conta no PythonAnywhere
Acesse PythonAnywhere.
Clique em "Sign Up".
Escolha um nome de usuário, e-mail e senha.
Confirme seu e-mail.
2. Criar uma Conta no GitHub
Acesse GitHub e crie uma conta.
Após criar a conta, faça login.
Crie um novo repositório.
3. Instalar o GitHub Desktop
Baixe e instale o GitHub Desktop.
Abra o GitHub Desktop e conecte-o à sua conta do GitHub.
4. Configurar o Ambiente de Desenvolvimento
No GitHub Desktop, crie um novo repositório com o nome que preferir.
Abra o repositório no Visual Studio Code (ou outro editor de sua preferência).
5. Desenvolver a Aplicação em Python
Utilize a biblioteca Flask, que é fácil e poderosa para desenvolvimento web com Python.
Crie um arquivo app.py e adicione o código básico do Flask.
from flask import Flask, render_template

```python
app = Flask(__name__)

@app.route('/')
def home():
    return render_template('index.html')

if __name__ == '__main__':
    app.run(debug=True)
```

Crie a pasta templates e, dentro dela, o arquivo index.html.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Meu App</title>
</head>
<body>
    <h1>Hello, World!</h1>
</body>
</html>
```

6. Configurar o Ambiente Virtual
No terminal, crie um ambiente virtual.
python -m venv venv
source venv/bin/activate  # Para Linux/Mac
venv\Scripts\activate  # Para Windows
Instale as dependências necessárias.
pip install flask
pip freeze > requirements.txt
7. Subir o Código para o GitHub
No terminal, inicialize o repositório Git.
git init
git add .
git commit -m "Initial commit"
git remote add origin <URL do repositório>
git push -u origin master
8. Configurar o PythonAnywhere
No PythonAnywhere, clique em "Web" e depois em "Add a new web app".
Escolha Flask e a versão do Python que você está usando.
Configure o caminho do seu arquivo app.py.
Conecte o repositório do GitHub ao PythonAnywhere.
9. Deploy da Aplicação
No terminal do PythonAnywhere, puxe o código do GitHub.
git pull origin master
Reinicie a aplicação web no PythonAnywhere.
Conclusão
Seguindo esses passos, você terá sua aplicação Python rodando na nuvem usando PythonAnywhere. Espero que tenham gostado. Qualquer dúvida, deixe um comentário que responderei assim que possível.

Valeu!

Referências
Vídeo explicativo: Como colocar um App no PythonAnywhere - YouTube
Tutorial: Quickstart — Flask Documentation (3.0.x)
Para este guia, utilizei diversas fontes e referências que fornecem informações detalhadas sobre cada etapa do processo. Aqui estão algumas das principais referências usadas:

Documentação do PythonAnywhere:

PythonAnywhere Help fornece tutoriais e guias detalhados sobre como hospedar aplicativos Python na plataforma.
Documentação do GitHub:

GitHub Docs oferece informações completas sobre como criar e gerenciar repositórios no GitHub, além de como usar o GitHub Desktop.
Documentação do Flask:

Flask Documentation é a fonte oficial para aprender a usar o Flask para desenvolvimento web em Python.
Documentação do Visual Studio Code:

Visual Studio Code Docs fornece guias sobre como usar este popular editor de código, incluindo a integração com o GitHub.
Tutoriais Online e Artigos:

Diversos tutoriais online e artigos de blogs que explicam como configurar ambientes virtuais, instalar pacotes Python, e conectar repositórios Git ao PythonAnywhere.
Utilizando essas referências, você conseguirá entender melhor cada etapa do processo e aprofundar seus conhecimentos sobre as ferramentas usadas. Boa sorte com o seu projeto!