# Documento de Visão de Design - Alchemy Browser

Este documento detalha a aparência (UI) e a experiência de uso (UX) do Alchemy Browser. Ele serve como um guia para o desenvolvimento, garantindo que o produto final seja fiel à nossa visão de simplicidade, clareza e controle.

---

## 1. Janela Principal

A primeira impressão do usuário. A janela principal deve transmitir calma e competência. A filosofia é "menos é mais".

### 1.1. Filosofia Geral

*   **Espaço Negativo:** A interface deve "respirar". Usar margens e espaçamentos generosos para evitar a sensação de aperto.
*   **Animações Sutis:** As animações devem ser funcionais e suaves, nunca chamativas. Um leve "fade" ao abrir menus ou uma transição suave ao passar o mouse sobre um ícone. O objetivo é fluidez, não espetáculo.
*   **Paleta de Cores Padrão (Modo Claro/Escuro):**
    *   **Modo Claro:** Fundo branco ou quase branco (#FFFFFF / #F8F8F8), texto preto de alto contraste (#121212), cor de destaque sutil (um azul ou cinza calmo).
    *   **Modo Escuro:** Fundo cinza muito escuro (#1C1C1C), texto branco ou cinza claro (#EAEAEA), mesma cor de destaque.

### 1.2. Barra Superior (Header)

A área mais importante. Deve ser limpa e funcional.

*   **Botões de Navegação (Esquerda):**
    *   **Ícones:** Voltar, Avançar, Recarregar.
    *   **Design:** Ícones SVG minimalistas, de linhas finas. Sem bordas ou fundo. Ao passar o mouse, o ícone ganha um fundo circular muito sutil e de baixa opacidade.

*   **Barra de Abas (Tabs):**
    *   **Aba Ativa:** Destaca-se com uma cor de fundo sutil e o texto em negrito.
    *   **Abas Inativas:** Ficam em um tom mais apagado. O título da página é legível, mas não compete com a aba ativa.
    *   **Separadores:** Uma linha vertical muito fina (1px) separa as abas para organização.
    *   **Botão de Nova Aba (+):** Um ícone de "+" no final da barra de abas.

*   **Barra de Endereço/Busca (Omnibar):**
    *   **Design:** Uma pílula com cantos arredondados. Fundo ligeiramente diferente da barra superior para se destacar.
    *   **Ícone de Segurança (Cadeado):** À esquerda, dentro da barra.
    *   **Botão "Modo Alchemy":** O ícone de um frasco de alquimia fica posicionado à direita, dentro da barra. Este é o nosso botão principal. Ao ser clicado, ele ativa a IA para redesenhar a página. Quando ativo, o ícone pode brilhar sutilmente.

*   **Ícones de Ação (Direita):**
    *   **Menu Principal (Ícone do Alchemy):** Um ícone com o logo do Alchemy (o frasco) abre o menu principal (Configurações, Histórico, Downloads, etc.).
    *   **Extensões (Peça de Quebra-Cabeça):** Um único ícone para gerenciar as extensões, mantendo a barra limpa.
