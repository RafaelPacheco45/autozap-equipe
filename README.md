# Central da Equipe AutoZap

Portal publico de materiais comerciais: https://equipe.autozap.log.br

Biblioteca com posts exportaveis em PNG, logos, cartas, propostas, mensagens, guias, busca e favoritos.

## Executar localmente

Requer Python 3, sem instalacao de dependencias:

```sh
python -m http.server 8791 --directory dist
```

Abra http://localhost:8791.

## Atualizar materiais

- `dist/app.js`: catalogo, textos e geracao das artes.
- `dist/assets/`: logos e arquivos.
- `dist/index.html`: estrutura da central.
- `dist/style.css`: estilos responsivos.

Os dados preenchidos nos modelos ficam na pagina. Favoritos sao salvos no navegador. Nao ha banco de dados, login de representantes ou painel administrativo.

## Hospedagem

O dominio principal esta hospedado no Sites, com acesso publico. Este repositorio mantem o codigo-fonte; um push no GitHub nao atualiza automaticamente a hospedagem Sites. A configuracao do projeto esta em `.openai/hosting.json`.

## Validacao

```sh
node --check dist/app.js
```
