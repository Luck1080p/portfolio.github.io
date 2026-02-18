# Portfolio - Lucas Brito

Este é o repositório do meu portfólio pessoal, focado em minha atuação como Cloud Architect, DevOps & SRE. O projeto apresenta uma interface moderna, inspirada em terminais e estética tech, utilizando HTML, CSS e JavaScript puro.

## 🚀 Funcionalidades

- **Splash Screen Interativa**: Uma tela inicial que simula uma conexão SSH, reforçando o tema de infraestrutura e DevOps.
- **Animações de Entrada**: Transições suaves e animações de "fade-up" para os elementos da página.
- **Design Responsivo**: Adaptado para diferentes tamanhos de tela (desktop e mobile).
- **Fallback de Avatar**: Caso a imagem de perfil não carregue, um gradiente estilizado é exibido automaticamente.
- **Seções Detalhadas**:
    - **Sobre**: Breve resumo profissional.
    - **Habilidades**: Grid de badges com as principais tecnologias (GCP, AWS, Terraform, Kubernetes, etc).
    - **Experiência**: Lista de passagens profissionais com destaque visual.
    - **Projetos**: Cards interativos linkando para repositórios ou demonstrações.
    - **Certificações**: Seção dedicada a credenciais profissionais.
    - **Formação**: Histórico acadêmico.

## 📂 Estrutura do Projeto

```text
.
├── index.html          # Estrutura principal da página
├── README.md           # Documentação do projeto
└── assets/
    ├── luck1080p.png   # Imagem de perfil (avatar)
    ├── css/
    │   └── style.css   # Estilização completa (Variáveis, Grid, Flexbox, Animações)
    └── js/
        └── main.js     # Lógica de interação (Splash screen, transições)
```

## 🛠️ Tecnologias Utilizadas

- **HTML5**: Estrutura semântica.
- **CSS3**: Uso extensivo de variáveis (Custom Properties), Flexbox, Grid e Keyframes para animações.
- **JavaScript (Vanilla)**: Manipulação simples do DOM para controle da Splash Screen e efeitos de opacidade.
- **Google Fonts**: Fontes 'IBM Plex Mono' (para estética de código) e 'IBM Plex Sans' (para textos e títulos).

## 🚀 Como Executar

O projeto é estático e não requer compiladores ou servidores complexos.

1.  Clone o repositório.
2.  Abra o arquivo `index.html` diretamente em seu navegador preferido.
3.  Ou utilize uma extensão como **Live Server** no VS Code para visualizar as alterações em tempo real.

## 🔧 Como Funciona o Código

### JavaScript (`main.js`)
A principal função é o `entrar()`. Quando o usuário clica no botão "[ ENTRAR ]" na Splash Screen:
1. A classe `.hidden` é adicionada à Splash Screen, disparando uma transição de opacidade definida no CSS.
2. O elemento `<main>` (que contém o conteúdo real) é alterado de `display: none` para `display: block`.
3. Um pequeno `setTimeout` é usado para garantir que o navegador processe o `display: block` antes de alterar a `opacity` para `1`, permitindo uma transição suave de fade-in.

### CSS (`style.css`)
- **Variáveis (`:root`)**: Centralizam as cores (accent, surface, bg) e fontes, facilitando manutenções futuras.
- **Grid Background**: Um efeito de malha criado com `linear-gradient` no pseudo-elemento `body::before`.
- **Animações (`@keyframes fadeUp`)**: Aplicadas a cada seção para criar um efeito de revelação sequencial conforme a página carrega.

---
Built with ♥ by Lucas Brito
