# 💈 Barbearia Don Gabriel

Site institucional de uma página (single-page) para a **Barbearia Don Gabriel**, com apresentação dos serviços, horários, localização e agendamento direto pelo WhatsApp.

Feito com **HTML, CSS e JavaScript puro** — sem frameworks, sem build, sem dependências.

---

## ✨ Funcionalidades

- **Hero com vídeo** de fundo (opcional) e logo da barbearia
- **Lista de serviços** com descrição e preço
- **Horários de funcionamento**
- **Localização** com endereço e link direto para o Google Maps
- **Botão de agendamento** que abre o WhatsApp com mensagem pré-preenchida
- **Botão flutuante do WhatsApp** sempre visível
- **Galeria de fotos** do trabalho com lightbox (ampliar ao clicar)
- Link para o **Instagram**
- Layout **responsivo** (celular, tablet e desktop)

---

## 📁 Estrutura do projeto

```
barbearia-dom-gabriel/
├── index.html                    # Site completo (HTML + CSS + JS)
├── haro.mp4                      # Vídeo do hero (opcional)
├── logo_don_gabriel_redonda.png  # Logo da barbearia
└── fotos/                        # Fotos dos trabalhos (galeria)
```

---

## ✏️ Como editar o conteúdo

Todo o conteúdo do site fica em **um único bloco** no `<script>` do `index.html`, chamado `CONFIG`. Não é preciso mexer no restante do código.

```js
const CONFIG = {
  nome: "Barbearia Don Gabriel",
  slogan: "...",                          // frase de destaque (opcional)
  logo: "logo_don_gabriel_redonda.png",
  video: { mp4: "haro.mp4", webm: "", poster: "" },  // vídeo do hero (opcional)
  whatsapp: "55XXXXXXXXXXX",              // DDI + DDD + número, só dígitos
  mensagem: "Olá! Quero agendar um horário.",
  endereco: "Rua, número - Bairro, Cidade - UF",
  mapsUrl: "https://maps.app.goo.gl/...",
  instagram: "https://www.instagram.com/...",
  servicos: [
    { nome: "Corte", desc: "Tesoura ou máquina, com acabamento na navalha.", preco: "R$ 00" },
    // ...
  ],
  horarios: [
    ["Terça a Sábado", "09h às 20h"],
    ["Domingo e Segunda", "Fechado"]
  ],
  // fotos: coloque os arquivos na pasta "fotos" e liste aqui
};
```

### O que você pode alterar

| Campo | O que faz |
|---|---|
| `nome` | Nome exibido no site |
| `logo` | Arquivo da logo |
| `video` | Vídeo do hero (deixe vazio para não usar) |
| `whatsapp` | Número que recebe os agendamentos (somente dígitos) |
| `mensagem` | Texto que já vem preenchido no WhatsApp |
| `endereco` / `mapsUrl` | Endereço e link do Google Maps |
| `instagram` | Link do perfil |
| `servicos` | Lista de serviços, descrições e preços |
| `horarios` | Dias e horários de atendimento |

### Adicionando fotos

1. Coloque as imagens na pasta `fotos/`
2. Liste os nomes dos arquivos no `CONFIG`, na seção de fotos

---

## 🚀 Como rodar localmente

**Opção 1 — direto no navegador:** abra o `index.html` com duplo clique.

**Opção 2 — com Live Server (VS Code):**

1. Instale a extensão **Live Server**
2. Clique com o botão direito no `index.html` → **Open with Live Server**
3. Acesse `http://localhost:5500`

---

## 🌐 Deploy

Por ser um site estático, pode ser publicado gratuitamente em:

- **[Vercel](https://vercel.com)** — importe o repositório do GitHub e faça o deploy (sem configuração extra)
- **GitHub Pages** — em *Settings → Pages*, selecione a branch `main`
- **Netlify**

Para usar um domínio próprio (ex.: `barbeariadongabriel.com.br`), configure o domínio no painel da hospedagem escolhida.

---

## 🛠️ Tecnologias

- HTML5
- CSS3
- JavaScript (ES6+)

---

## 👨‍💻 Autor

Desenvolvido por **Willian** — [github.com/willianjsilva-dev](https://github.com/willianjsilva-dev)

---

## 📄 Licença

Projeto desenvolvido para uso da Barbearia Don Gabriel. Todos os direitos sobre nome, logo e fotos pertencem ao estabelecimento.
