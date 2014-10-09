# Tray OpenCode Workflow

Estrutura e dependências do fluxo de trabalho do Tray OpenCode.

## Instalação

1. `git clone git@github.com:tray-tecnologia/opencode-workflow.git minha-area`
2. `cd minha-area`
3. `npm install` - instala as dependências
4. `gulp` - inicia as tarefas do gulp

**Obs:** Se o Gulp não estiver rodando corretamente no Windows, execute o seguinte comando: `node node_modules/gulp/bin/gulp.js`

## Estrutura de pastas

Para que o task runner funcione corretamente, precisará existir essa estrutura de pastas:

    minha-area/
        351572/
            css/
                sass/
                    a.scss
                    b.scss
                    c.scss
                theme.min.css
            js/
                modules/
                    a.js
                    b.js
                    c.js
                theme.min.js
        108099/
            css/
                sass/
                    a.scss
                    b.scss
                    c.scss
                theme.min.css
            js/
                modules/
                    a.js
                    b.js
                    c.js
                theme.min.js

## Criando e alterando lojas

1. Execute no terminal ssh: `sh clone.sh {ID_LOJA}`
2. Entre na pasta da loja `cd {ID_LOJA}`
3. Execute `opencode configure API_KEY API_PASSWORD THEME_ID`
4. Execute `opencode download` para baixar todos os arquivos do tema
