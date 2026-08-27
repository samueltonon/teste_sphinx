
===========================================
Publicação no GitHub Pages
===========================================

A publicação da documentação gerada pelo Sphinx é feita utilizando o repositório do GitHub e o recurso de hospedagem estática **GitHub Pages**.

Estruturação da Pasta docs
==========================
O GitHub Pages pode servir arquivos estáticos diretamente de uma pasta chamada ``docs`` na raiz do repositório.

1. Copie todo o conteúdo gerado dentro de ``build/html`` para uma pasta chamada ``docs`` na raiz do projeto.
2. Crie um arquivo em branco chamado **``.nojekyll``** dentro da pasta ``docs`` para garantir que o suporte a arquivos CSS do Sphinx não seja bloqueado pelo GitHub.

Envio do Código ao Repositório
==============================
No terminal do VS Code, execute a sequência de comandos para registrar o histórico e enviar a documentação para o GitHub:

.. code-block:: powershell

   git add .
   git commit -m "Atualizacao da documentacao Sphinx"
   git branch -M main
   git remote add origin https://github.com/SEU_USUARIO/SEU_REPOSITORIO.git
   git push -u origin main

Ativação do GitHub Pages
========================
1. Acesse o repositório no [GitHub](https://github.com).
2. Vá na aba **Settings** > **Pages** no menu lateral.
3. Em **Source / Branch**, selecione a branch **main**.
4. No campo do diretório, altere de ``/ (root)`` para **``/docs``**.
5. Clique em **Save**.

Após cerca de 2 minutos, o site da documentação estará publicado e acessível publicamente via navegador.