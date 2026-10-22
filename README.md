# Studio Penelope

Versão editorial do site demonstrativo, pronta para hospedar na Vercel a partir de um repositório do GitHub. Inclui os arquivos completos de HTML, CSS, JavaScript e imagens. Não depende do Codex ou do serviço Sites para funcionar.

## 1. Subir no GitHub

1. Extraia o ZIP no computador.
2. Crie um repositório no GitHub, por exemplo `studio-penelope`.
3. No repositório, escolha **Add file → Upload files**. Em um repositório vazio, use o link **uploading an existing file**.
4. Arraste o conteúdo da pasta extraída: a pasta `public`, o arquivo `vercel.json`, este `README.md` e, se exibido, `.gitignore`.
5. Clique em **Commit changes** para salvar.

Envie os arquivos extraídos. Não envie somente o ZIP. `vercel.json` e `public` devem aparecer diretamente na raiz do repositório, sem outra pasta envolvendo os dois.

Estrutura esperada:

```text
studio-penelope/
├── public/
│   ├── index.html
│   ├── style.css
│   ├── editorial.css
│   ├── app.js
│   └── assets/
├── vercel.json
├── .gitignore
└── README.md
```

## 2. Publicar na Vercel

1. Entre na Vercel com sua conta e conecte o GitHub.
2. Crie um novo projeto e importe o repositório `studio-penelope`.
3. Use a raiz do repositório como **Root Directory**. O arquivo `vercel.json` já informa a configuração para este site estático.
4. Confirme os valores abaixo e clique em **Deploy**.

| Configuração | Valor |
| --- | --- |
| Framework Preset | Other |
| Root Directory | Raiz do repositório, sem subpasta |
| Build Command | Vazio / sem comando |
| Output Directory | public |
| Install Command | Vazio / sem comando |
| Variáveis de ambiente | Nenhuma |

Não é necessário instalar dependências ou executar um processo de build. O site usa apenas arquivos estáticos. A Vercel fornecerá o endereço ao concluir a publicação. Este pacote foi conferido localmente; a implantação na sua conta Vercel ainda deverá ser executada.

Depois, alterações enviadas à branch de produção do repositório conectado podem gerar novas publicações automaticamente, conforme a configuração do projeto na Vercel.

## Editar o site

- **Textos, fotos e seções:** `public/index.html`.
- **Visual editorial mais recente:** `public/editorial.css`. Este arquivo complementa `public/style.css`; mantenha os dois.
- **Menu, WhatsApp, filtros e galeria:** `public/app.js`.
- **Imagens:** `public/assets/`. Preserve os nomes ou atualize as referências no HTML.

O WhatsApp usado é +55 12 99734-3779. As fontes são carregadas pelo Google Fonts, com fontes alternativas locais. Para uma visualização rápida, abra `public/index.html` no navegador com conexão à internet.

## Demonstração e materiais

O pacote conserva o aviso de conceito demonstrativo e a instrução `noindex,nofollow,noarchive`. Isso evita solicitar indexação em buscadores, mas não controla acesso: a visibilidade do endereço na Vercel depende das configurações da sua conta/projeto. A proteção privada da demonstração anterior não é transferida com os arquivos.

As imagens editoriais de pessoas foram geradas por IA e estão identificadas como ilustrativas. O portfólio utiliza recortes das capturas fornecidas e o logotipo original tem baixa resolução. Para o lançamento oficial, confirme os dados e as autorizações de divulgação, substitua as fotos por originais em alta resolução e revise o aviso de demonstração e os metadados de indexação.

## Referências oficiais

- [Enviar arquivos para o GitHub](https://docs.github.com/en/repositories/working-with-files/managing-files/adding-a-file-to-a-repository)
- [Começar na Vercel](https://vercel.com/docs/getting-started-with-vercel)
- [Configuração de build e sites estáticos](https://vercel.com/docs/builds/configure-a-build)
- [Configuração do vercel.json](https://vercel.com/docs/project-configuration/vercel-json)
