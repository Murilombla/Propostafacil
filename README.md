# PropostaFácil

Gerador simples de propostas comerciais para freelancers e pequenos prestadores de serviços. O projeto é uma página estática, sem dependências, que pode ser aberta localmente ou publicada em um serviço de hospedagem estática.

## O que já funciona

- Pré-visualização atualizada enquanto os campos são preenchidos.
- Cálculo de horas × valor por hora, custos adicionais, desconto aplicado e total.
- Aviso quando o desconto digitado ultrapassa o subtotal; o total não fica negativo.
- Impressão / opção de salvar a proposta como PDF.
- Cópia de um resumo em texto.
- Rascunho salvo localmente no navegador e opção de limpar os campos e apagar o rascunho.
- Layout responsivo para desktop e celular.

## Rodar localmente

Basta abrir `index.html` em um navegador moderno. Não é necessário instalar pacotes ou executar um build.

Para servir a pasta via HTTP durante o desenvolvimento, abra um terminal nesta pasta e execute:

```bash
python -m http.server 8000
```

Depois acesse `http://localhost:8000`.

## Versionar com Git

Na pasta do projeto, execute:

```bash
git init
git add index.html README.md .gitignore
git commit -m "Cria primeira versão do PropostaFácil"
git branch -M main
```

Depois de criar um repositório vazio no GitHub, conecte-o e envie o código (substitua o endereço pelo URL do seu repositório):

```bash
git remote add origin https://github.com/SEU-USUARIO/propostafacil.git
git push -u origin main
```

## Publicação

O site não precisa de backend nem de etapa de build. Pode ser publicado em uma hospedagem estática, como GitHub Pages ou Netlify. Para GitHub Pages, o arquivo inicial já está no local esperado: `index.html` na raiz do repositório. A configuração de publicação será feita na próxima etapa.

## Privacidade e limitações do protótipo

- Os dados do formulário não são enviados a um servidor pelo código desta página.
- O rascunho é mantido no armazenamento local do navegador. Em computadores compartilhados, use **Limpar tudo** ao terminar.
- O botão de PDF abre a janela de impressão do navegador. Para evitar que a URL, data ou título do navegador apareçam no documento, desmarque **Cabeçalhos e rodapés** nas configurações de impressão.
- A ferramenta ainda não tem contas de usuário, sincronização entre dispositivos, envio por e-mail ou armazenamento em nuvem.

## Estrutura

```text
propostafacil-site/
├── index.html
├── README.md
└── .gitignore
```
