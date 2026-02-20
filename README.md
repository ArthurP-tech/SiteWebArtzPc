Claro, Arthur! Preparei um **README completo** em Markdown com base no seu site **ArtZ Pc** para você **copiar e colar** no GitHub. Ajuste somente o que for necessário (como imagens, links e licença).

***

# ArtZ Pc — E-commerce de PCs e Hardware

Site de e-commerce responsivo para catálogo e venda de **PCs gamers**, **peças** e **kits de upgrade**. Desenvolvido com **HTML, CSS, Bootstrap** e **Font Awesome**, com foco em interface moderna, interatividade e navegação simples.

> **Resumo:** Carrossel de destaque, cards animados, navegação por categorias, acordions informativos, modal de compartilhamento, formulário de cadastro e controle de satisfação com *range* estilizado.

***

## ✨ Funcionalidades

*   **Navbar fixa** com menu, dropdowns e botões de ação (Perfil, Monte seu PC, Compartilhar).
*   **Carrossel** de imagens com controles.
*   **Acordeões** (Quem somos, Por que a ArtZ Pc, Política de Privacidade).
*   **Modal** de compartilhamento (vídeo do YouTube e link de referência).
*   **Formulário de Cadastro** (nome, e-mail, senha).
*   **Controle de Satisfação** (slider com valor percentual dinâmico).
*   **Cards de Produtos** (preço à vista e opções no cartão via dropdown).
*   **Alert animado** com cupom de desconto (ARTZ25).
*   **Paginação** para futuras páginas.
*   **Footer** com créditos e direitos.
*   **Scroll suave** e **animação hover** em cards.

***

## 🧰 Stack & Dependências

*   **HTML5** + **CSS3**
*   **Bootstrap 5** (componentes, grid e utilitários)
*   **Font Awesome** (ícones)
*   **Google Fonts** (Pirata One)
*   **JavaScript Vanilla** (interações simples)

> O projeto referencia **arquivos locais**: `css/bootstrap.min.css` e `js/bootstrap.bundle.min.js`. Se preferir, você pode trocar para CDNs (ver seção “CDNs opcionais”).

***

## 📁 Estrutura de Pastas (sugerida)

    ArtZ-Pc/
    ├── index.html
    ├── css/
    │   └── bootstrap.min.css
    ├── js/
    │   └── bootstrap.bundle.min.js
    ├── fontawesome/
    │   └── css/
    │       └── all.min.css
    ├── Imagens/
    │   ├── A.jpg
    │   ├── B.jpg
    │   ├── C.jpg
    │   ├── D.webp
    │   ├── E.webp
    │   ├── F.webp
    │   ├── G.webp
    │   ├── H.webp
    │   └── I.webp
    └── salvar.php            (endpoint do formulário)

***

## 🚀 Como Rodar Localmente

1.  **Clone** o repositório:
    ```bash
    git clone https://github.com/seu-usuario/ArtZ-Pc.git
    cd ArtZ-Pc
    ```

2.  **Garanta os arquivos estáticos** nas pastas indicadas (Bootstrap, Font Awesome, imagens).

3.  **Abra o `index.html`** diretamente no navegador\
    *(para o formulário funcionar com PHP, rode um servidor local — ver próximo item).*

4.  **(Opcional – PHP)** Rode um servidor embutido do PHP:
    ```bash
    php -S localhost:8000
    ```
    E acesse: `http://localhost:8000`

> ⚠️ O formulário de cadastro usa `action="salvar.php"` e **método GET**. Em produção, recomenda-se **POST** e validação do lado do servidor.

***

## 🖼️ Screenshots (adicione depois)

> Substitua os caminhos abaixo pelos seus prints reais.

*   **Home com Navbar + Carrossel**\
    `Imagens/screenshot-home.png`

*   **Cards de Produtos (Peças e PCs Gamers)**\
    `Imagens/screenshot-cards.png`

*   **Formulário + Satisfação**\
    `Imagens/screenshot-form.png`

***

## 🔗 Navegação & Seções

*   **Navbar:** Início, Computadores (#card1), Peças (#card2), Dropdown de Hardware, Monte seu PC/Compartilhar.
*   **Carrossel:** Destaques (3 banners).
*   **Acordeões:**
    *   *Quem Somos* (proposta da ArtZ Pc)
    *   *Por que a ArtZ Pc* (diferenciais)
    *   *Política de Privacidade*
*   **Cadastro:** `salvar.php` (GET)
*   **Satisfação:** *range* com % dinâmico (JS)
*   **Peças:** Processadores, Memórias, Kit Upgrade
*   **PCs Gamers:** Linhas S, S+, X
*   **Paginação:** futura expansão de conteúdo

***

## 🎨 Estilo & UI

*   **Tipografia:** *Pirata One* para o logotipo “ArtZ Pc”.
*   **Tema:** Base **Bootstrap** com cores **primary / info / success**.
*   **Animações:**
    *   Cards com **hover** (elevação e sombra azul).
    *   Alert com **animação de cores** (keyframes).
    *   **Scroll suave** para âncoras.
*   **Slider personalizado** (track azul e *thumb* branca com borda azul).

***

## 🛡️ Boas Práticas & Observações

*   **Formulário:**
    *   Trocar `method="get"` para `method="post"` para dados sensíveis.
    *   Validar e sanitizar dados no `salvar.php`.
    *   Considerar *honeypots* ou reCAPTCHA contra spam.

*   **Acessibilidade (a melhorar):**
    *   Adicionar `alt` descritivo em todas as imagens (algumas estão como `"..."`).
    *   Garantir contraste suficiente no texto dos botões.
    *   Associar `label for` corretamente (você já usa, ótimo!).

*   **SEO:**
    *   Adicionar `<meta name="description">`.
    *   Títulos hierárquicos (`h1`, `h2`, etc.) coerentes.
    *   Texto alternativo em imagens.

*   **Performance:**
    *   Otimizar imagens (`.webp` já ajuda 👍).
    *   Minificar CSS/JS (se usar arquivos próprios).
    *   Usar `loading="lazy"` em imagens fora do viewport.

***

## 🧪 Testes Manuais Sugeridos

*   [ ] Navegação em dispositivos móveis (menu *hamburger*).
*   [ ] Carrossel auto-play e setas funcionando.
*   [ ] Acordeões abrindo/fechando corretamente.
*   [ ] Modal “Compartilhar” abrindo e fechando.
*   [ ] Slider exibindo o valor correto (`50%`, etc.).
*   [ ] Dropdown de preços nos cards.
*   [ ] Formulário enviando dados para `salvar.php`.
*   [ ] Links de âncora (#card1, #card2).
*   [ ] Paginação com estilo ativo e desabilitado.

***

## 🔌 CDNs Opcionais

Se quiser reduzir arquivos locais, substitua por CDNs:



***

## 🗺️ Roadmap

*   [ ] Página “Monte seu PC” com configurador (compatibilidade de peças).
*   [ ] Carrinho e checkout (frontend).
*   [ ] Integração com API de CEP/frete.
*   [ ] Sistema de login/cadastro real (PHP + MySQL).
*   [ ] Área de perfil e pedidos.
*   [ ] Notificações/inbox do botão “Perfil”.

***

## 🤝 Contribuições

Sinta-se à vontade para abrir **Issues** e enviar **Pull Requests** com melhorias, correções ou novas seções.

**Sugestões de PRs:**

*   SEO e acessibilidade
*   Padrões de código (HTML semântico, BEM para CSS)
*   Otimização de imagens
*   Novas categorias ou filtros

***

## 📄 Licença

Defina a licença do projeto (recomendado: **MIT**).\
Crie um arquivo `LICENSE` ou escolha no GitHub ao criar o repositório.

***

## 👨‍💻 Autor

**Arthur Pereira**\
Design & desenvolvimento do frontend.\
Créditos de ícones: **Font Awesome**.\
Framework CSS: **Bootstrap**.\
Fonte: **Google Fonts (Pirata One)**.

***

## ✅ Notas Técnicas Diretas do Código

*   `navbar` fixa (classe `fixed-top`) → adiciona `padding-top` no `body` para evitar sobreposição (já implementado).
*   Dois modais com o **mesmo `id="exampleModal"`** em pontos diferentes do HTML. ✅ **Recomendação:** usar IDs únicos (ex.: `modalCompartilharVideo` e `modalLinkLoja`).
*   `footer` com créditos “Desing by” → **typo**: “Design by”.
*   Política de Privacidade: menciona “StudioPC” em um trecho. Se o projeto é “ArtZ Pc”, padronize o nome.
*   **Atributo `alt`** das imagens está como `"..."`. Substitua por descrições reais (importante para SEO/A11y).
*   Utilize `rel="noopener noreferrer"` em links externos (se abrir em nova aba).

***

Se quiser, eu também posso:

*   **Converter este README para inglês**;
*   **Ajustar o HTML** (IDs duplicados, acessibilidade, SEO);
*   **Criar um `README.md` como arquivo** e te entregar pronto para download.

Quer que eu também gere um **`LICENSE`** (ex.: MIT) e um **`.gitignore`** padrão?
