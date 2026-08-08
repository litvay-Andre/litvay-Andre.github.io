# Portfólio — André Oliver Litvay

Site estático (HTML/CSS puro, sem build) com página inicial + uma página por projeto.

## Estrutura

```
index.html
projects/
  rfid-node-red.html
  motorguard.html
  rogowski-coil.html
assets/
  style.css
  cv-andre-litvay.pdf
  img/
```

## Como publicar no GitHub Pages (grátis)

1. Crie um repositório novo no GitHub chamado **exatamente**: `litvay-Andre.github.io`
   (tem que ser `SEU-USUARIO.github.io`, senão o site não fica na raiz do domínio).
2. No repositório, clique em **Add file → Upload files** e arraste **todo o conteúdo desta pasta**
   (o `index.html` deve ficar na raiz do repositório, não dentro de uma subpasta).
3. Commit direto na branch `main`.
4. Vá em **Settings → Pages**. Em "Build and deployment", selecione **Deploy from a branch**,
   branch `main`, pasta `/ (root)`. Salve.
5. Em 1–2 minutos o site estará no ar em: **https://litvay-Andre.github.io/**

Se preferir usar o Git pela linha de comando em vez do upload pelo navegador:

```bash
cd pasta-do-site
git init
git add .
git commit -m "Primeira versão do portfólio"
git branch -M main
git remote add origin https://github.com/litvay-Andre/litvay-Andre.github.io.git
git push -u origin main
```

## Atualizando depois

Qualquer alteração nos arquivos + novo commit/push (ou novo upload) atualiza o site automaticamente
em 1–2 minutos — não precisa reconfigurar nada.

## QR code do currículo

O QR code no final do currículo (`Curriculo_Andre_Oliver_Litvay.docx`) já aponta para
`https://litvay-Andre.github.io/`. Ele só vai funcionar depois que os passos acima forem feitos —
até lá, o link fica "no ar" mas sem site publicado.

## Trocar/adicionar projetos

Cada projeto é um arquivo HTML independente em `projects/`. Para adicionar um novo projeto,
duplique um dos arquivos existentes como modelo e adicione um novo `<a class="card">` em
`index.html` na seção `#projetos`.
