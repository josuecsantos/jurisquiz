# JurisQuiz — Guia de Publicação no GitHub Pages

Siga este passo a passo para colocar o app no ar em menos de 10 minutos.
Você vai acessar pelo celular via link e instalar como app nativo.

---

## 1. Criar conta no GitHub (se ainda não tiver)

1. Acesse https://github.com
2. Clique em **Sign up**
3. Crie sua conta gratuitamente

---

## 2. Criar um repositório

1. Depois de entrar, clique no **+** no canto superior direito → **New repository**
2. Dê o nome: `jurisquiz`
3. Deixe em **Public** (obrigatório para GitHub Pages gratuito)
4. Clique em **Create repository**

---

## 3. Subir os arquivos

Na página do repositório recém-criado:

1. Clique em **uploading an existing file**
2. Arraste ou selecione **todos os arquivos** desta pasta:
   - `index.html`
   - `manifest.json`
   - `sw.js`
   - pasta `icons/` com os dois arquivos `.png`
3. Clique em **Commit changes**

---

## 4. Ativar o GitHub Pages

1. Vá em **Settings** (aba do repositório)
2. No menu lateral, clique em **Pages**
3. Em **Source**, selecione **Deploy from a branch**
4. Em **Branch**, selecione **main** → pasta **(root)**
5. Clique em **Save**

Aguarde ~1 minuto. Seu app estará em:

```
https://SEU-USUARIO.github.io/jurisquiz/
```

---

## 5. Instalar no celular

### Android (Chrome):
1. Abra o link acima no Chrome do celular
2. Um banner aparecerá: **"Instalar JurisQuiz"** → toque nele
3. Confirme — o ícone aparecerá na tela inicial como um app nativo

### iPhone (Safari):
1. Abra o link no Safari
2. Toque no botão **Compartilhar** (ícone de caixinha com seta)
3. Role e toque em **Adicionar à Tela de Início**
4. Toque em **Adicionar**

---

## Observações importantes

- **Seus dados ficam salvos no próprio celular** (localStorage). Se trocar de celular, use a função Exportar/Importar (disponível em versão futura).
- O app **funciona offline** depois de instalado — graças ao service worker.
- Para atualizar o app, basta subir novos arquivos no GitHub e aguardar ~1 min.

---

## Estrutura de arquivos

```
jurisquiz/
├── index.html      ← App principal
├── manifest.json   ← Configurações PWA (nome, ícone, cor)
├── sw.js           ← Service Worker (modo offline)
└── icons/
    ├── icon-192.png
    └── icon-512.png
```
