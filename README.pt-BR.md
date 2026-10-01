# Snake starter repository

[English](README.md)

## Ideia e processo

Apesar do nome, o repositório contém o template de terminal Python do Code Institute, não um Snake implementado. Código revisado em 01/10/2026. `run.py` só tem comentários e requirements.txt um placeholder. Não foram encontrados loop, tabuleiro, colisões, planejamento ou diário de design no código revisado.

## Arquitetura e design

Wrapper Node/Total.js serve terminal no navegador e WebSocket raw. `controllers/default.js` inicia `python3 run.py` em pseudo-terminal 80x24 para cada cliente. index.js inicia Total.js em release; Procfile roda `node index.js`. Infraestrutura de template de terceiros, não implementação de jogo.

## Configuração e testes

Não há programa Python jogável. Para inspecionar template local, revise package.json e requisitos nativos de node-pty em ambiente isolado. `npm test` é placeholder que termina com erro. Nada instalado/executado; deploy público não confirmado.

Antes de implementar, defina controles, tabuleiro, comida, crescimento e colisões. Teste regras separadamente do wrapper. Não exponha serviço que inicia processos sem revisar acesso, limites e ambiente. Controller pode escrever creds.json por CREDS; credenciais não consultadas ou usadas nesta atualização.

## Capturas

Nenhuma captura adicionada; não há estado real de jogo. Futuras imagens datadas em `docs/assets/` devem mostrar jogo implementado, não tabuleiro inventado ou imagem de banco.

## Créditos e licença

Direitos de curso/template/dependências mantidos. Manifest existente declara ISC; nenhuma licença nova adicionada ou aplicada a terceiros. README original preservado no [apêndice em inglês](README.md#original-readme).
