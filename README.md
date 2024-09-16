# CAPTCHA NO TELEGRAM
🤤ESTE É UM BOT DE TELEGRAM QUE USA CAPTCHA BASEADO EM IMAGENS PARA VERIFICAR NOVOS MEMBROS DE GRUPOS.

<div align="center">
<img src="./IMAGENS/FOTO_1.gif" width="300"/>
<img src="./IMAGENS/FOTO_2.gif" width="300"/>
</div>

## DESCRIÇÃO:
O bot gera e envia captchas personalizados para novos usuários em grupos do Telegram, verificando suas respostas por meio de teclados interativos, e bane temporariamente aqueles que não resolvem o captcha no tempo limite.

## FUNCIONALIDADES:
1. **Criação de Captcha**:
   O bot gera um captcha na forma de uma imagem usando o pacote `svg-captcha`. A imagem contém uma expressão matemática simples (como `5 + 3`), e o usuário deve resolvê-la para ser admitido no grupo. O captcha é gerado com opções como cor, ruído, tamanho de fonte, e dimensões personalizáveis.

2. **Envio de Captcha**:
   Quando um novo usuário entra no grupo, o bot envia uma imagem do captcha. O usuário precisa responder corretamente dentro de um período de tempo configurável (padrão: 5 minutos). Caso não responda, ele será banido do grupo temporariamente.

3. **Resolução de Captcha**:
   O usuário recebe um teclado interativo com números e opções para apagar ou atualizar o captcha. Conforme ele insere os números, o bot verifica a resposta. Se a resposta for correta, o usuário é aprovado e admitido no grupo. Caso contrário, ele terá uma nova chance.

4. **Interatividade**:
   O bot usa teclados inline (teclados interativos no Telegram) para permitir que o usuário insira números, apague a entrada atual ou peça um novo captcha. O teclado interativo é gerado para cada usuário e associado à sua resposta ao captcha.

5. **Banimento Temporário**:
   Se o usuário falhar em resolver o captcha no tempo limite, o bot banirá temporariamente o usuário (por 24 horas). Isso impede spam ou bots de entrar no grupo.

## EXECUTANDO O PROJETO:
1. **Editar o código:**
   - Certifique-se de substituir "seu_token_aqui" pelas informações corretas das suas credenciais em `CODIGO/.env`, o qual pode ser obtido por meio do [@BotFather](https://t.me/BotFather).  Além disso, o bot depende de um arquivo JSON de linguagem (`language.json`) que deve ser configurado com mensagens personalizadas, incluindo a mensagem que o bot enviará com o captcha.
   
2. **Instalando as Depêndencias:**
   - Para instalar as dependências listadas no arquivo "package.json", você pode usar o comando `npm install` no terminal. Certifique-se de estar no diretório do seu projeto onde o arquivo "package.json" está localizado (`CODIGO`). O npm irá ler o arquivo "package.json" e instalar todas as dependências listadas nele. 

   ```bash
   npm install
   ```

3. **Inicie o Bot:**
   - Para usar o `NODE`, inicie o bot com o seguinte comando:
    ```bash
    npm start
    ```

    - Para usar o `NODEMON`, inicie o bot com o seguinte comando:
    ```bash
    npm dev
    ```

4. **Exemplo de Fluxo:**
   1. Um usuário entra no grupo.
   2. O bot envia uma imagem de captcha para o usuário, junto com um teclado interativo.
   3. O usuário insere os números para resolver o captcha.
   4. Se correto, o bot aprova a entrada do usuário no grupo. Se incorreto, o usuário pode tentar novamente até o tempo limite expirar.
   5. Caso o usuário falhe ou o tempo expire, o bot bane temporariamente o usuário.

## NÃO SABE?
- Entendemos que para manipular arquivos em muitas linguagens e tecnologias relacionadas, é necessário possuir conhecimento nessas áreas. Para auxiliar nesse aprendizado, oferecemos cursos gratuitos disponíveis:
* [VEJA A DOCUMENTAÇÃO](https://core.telegram.org/bots/api)
* [CURSO DE TELEGRAF](https://github.com/VILHALVA/CURSO-DE-TELEGRAF)
* [CURSO DE JAVASCRIPT](https://github.com/VILHALVA/CURSO-DE-JAVASCRIPT)
* [CURSO DE NODEJS](https://github.com/VILHALVA/CURSO-DE-NODEJS)
* [CONFIRA MAIS CURSOS](https://github.com/VILHALVA?tab=repositories&q=+topic:CURSO)

## CREDITOS:
- [PROJETO CRIADO PELO "VDS13"](https://github.com/VDS13/telegram-captcha)
- [PROJETO EDITADO PELO VILHALVA](https://github.com/VILHALVA)

