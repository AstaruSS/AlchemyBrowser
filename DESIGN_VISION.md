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

---

## 2. Menu Principal

Acionado pelo clique no ícone do Alchemy na barra superior, este menu é a porta de entrada para as funções principais do navegador.

*   **Design:** Um menu suspenso (dropdown) vertical, limpo e com bom espaçamento entre os itens.
*   **Itens do Menu:** Cada item terá um ícone SVG minimalista à sua esquerda.
    *   Nova Aba
    *   Nova Janela
    *   Histórico
    *   Downloads
    *   Favoritos
    *   Extensões
    *   Imprimir...
    *   --- (Linha separadora)
    *   **Configurações**
    *   **Estúdio de Customização** (Este é o link para a nossa área de customização ampla)
    *   --- (Linha separadora)
    *   Ajuda
    *   Sobre o Alchemy
    *   Sair

---

## 3. Página de Configurações ("Configurações Diretas")

Esta página é um pilar da nossa filosofia. O objetivo é ser o oposto de páginas de configuração confusas.

### 3.1. Filosofia de Design

*   **Clareza e Intenção:** O usuário deve encontrar o que procura em segundos. A linguagem usada será simples e direta, evitando jargão técnico sempre que possível.
*   **Busca em Primeiro Lugar:** A ferramenta mais proeminente na página de configurações será a barra de busca.

### 3.2. Layout

*   **Estrutura de Duas Colunas:**
    *   **Coluna da Esquerda:** Um menu de navegação com as categorias principais (Aparência, Privacidade, Desempenho, etc.).
    *   **Coluna da Direita:** A área principal onde as opções da categoria selecionada são exibidas.
*   **Barra de Busca:** Localizada no topo da coluna da direita. Conforme o usuário digita, as opções relevantes de TODAS as categorias são exibidas instantaneamente.

### 3.3. Categorias Principais (Coluna da Esquerda)

1.  **Perfil:** Gerenciar perfis de usuário (se houver mais de um).
2.  **Aparência:**
    *   Opções simples: Modo Claro, Modo Escuro, Usar tema do sistema.
    *   **Link de Atalho:** "Quer mais opções? Visite nosso **Estúdio de Customização**."
3.  **Privacidade e Segurança:**
    *   Controles do uBlock Origin: Ligar/Desligar bloqueio de anúncios, Ligar/Desligar bloqueio de rastreadores.
    *   Opções para limpar dados de navegação (histórico, cookies, cache).
4.  **Desempenho:**
    *   Modo de Economia de Memória (para abas inativas).
    *   Ativar/Desativar aceleração de hardware.
    *   Controles simples para o usuário se sentir no comando.
5.  **Motor de Busca:** Escolher o buscador padrão da barra de endereço.

---

## 4. Estúdio de Customização

Esta não é uma página de configurações, é um ateliê. O Estúdio de Customização é onde o usuário tem liberdade total para moldar o Alchemy à sua imagem. A interface aqui será mais visual e interativa.

### 4.1. Filosofia de Design

*   **Poder e Clareza:** Oferecer opções avançadas sem sobrecarregar. A interface será organizada em abas para separar os diferentes domínios da customização.
*   **Feedback Instantâneo:** Todas as alterações feitas no Estúdio (cores, fontes, layout) serão refletidas na interface do navegador em tempo real, para que o usuário veja o resultado de suas escolhas imediatamente.

### 4.2. Layout em Abas

A página do Estúdio será organizada nas seguintes abas:

1.  **Temas**
2.  **Fontes**
3.  **Estrutura**
4.  **Atalhos**

### 4.3. Detalhes das Abas

*   **Aba "Temas":**
    *   **Seletor de Cores Completo:** O usuário terá um seletor de cores (color picker) para cada elemento principal da interface:
        *   Cor de fundo da barra superior
        *   Cor de fundo da aba ativa
        *   Cor do texto da aba ativa
        *   Cor de fundo das abas inativas
        *   Cor do texto das abas inativas
        *   Cor da barra de endereço
        *   Cor de destaque principal (usada em menus e seleções)
    *   **Gerenciador de Temas:** Capacidade de salvar o conjunto de cores atual como um novo tema, dar um nome a ele e alternar entre temas salvos.
    *   **Importar/Exportar:** Opções para exportar um tema para um arquivo de texto (JSON) e importar temas criados por outros usuários.

*   **Aba "Fontes":**
    *   **Fonte da Interface:** Opção para escolher qualquer fonte instalada no sistema para ser usada na interface do navegador (menus, abas, etc.).
    *   **Fonte Padrão para Páginas:** Definir fontes padrão para conteúdo de páginas web (serif, sans-serif, monoespaçada).
    *   **Carregar Fonte Personalizada:** Botão para fazer upload de um arquivo de fonte (`.ttf`, `.otf`) diretamente do computador do usuário.

*   **Aba "Estrutura":**
    *   **Posição da Barra de Abas:** Botões de opção para definir a barra de abas no topo (padrão), na lateral esquerda, na lateral direita ou na parte inferior.
    *   **Barra de Favoritos:** Opções para "Sempre mostrar", "Mostrar apenas na página inicial" ou "Esconder (mostrar ao passar o mouse)".
    *   **Modo Zen:** Um interruptor para ativar um modo de foco total, que esconde toda a interface do navegador, mostrando apenas o conteúdo da página.

*   **Aba "Atalhos":**
    *   Uma lista de todas as ações do navegador (Nova Aba, Fechar Aba, Abrir Configurações, etc.).
    *   Ao lado de cada ação, um campo editável para o usuário definir sua própria combinação de teclas de atalho.
6.  **Sistema:** Configurações de download, gerenciamento de senhas.
