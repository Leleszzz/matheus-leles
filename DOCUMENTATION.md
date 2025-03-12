# Devops Challenge Documentação 

## Descrição
Este é um plugin para WordPress que exibe uma frase aleatória da música "Segure o Tchan" no painel de administração do WordPress. O objetivo deste plugin é servir como um desafio de desenvolvimento, onde um texto aleatório é mostrado para os administradores do site.

## função
Quando ativado, o plugin exibe uma das frases da música **"Segure o Tchan"** no painel de administração do WordPress, no canto superior direito. A frase exibida é aleatória e é gerada a partir de uma lista de versos da música.

Além disso, o plugin também inclui um estilo CSS simples para ajustar a exibição do texto.

## Como instalar
1. Faça o download do plugin.
2. Faça login no painel de administração do seu site WordPress.
3. Vá para **Plugins > Adicionar Novo**.
4. Clique em **Enviar Plugin** e selecione o arquivo zip do plugin.
5. Clique em **Instalar Agora** e, depois, em **Ativar**.

## Como Funciona
- O plugin gera uma frase aleatória a partir da música "Segure o Tchan" toda vez que o administrador acessar o painel do WordPress.
- A frase é mostrada como um aviso no painel de administração.
- O plugin utiliza uma função chamada `apiki_segura_o_tchan()` para escolher aleatoriamente uma frase da música.
- A frase é exibida usando a função `devops_challenge()`, que é chamada através do hook `admin_notices` no WordPress.
- O estilo CSS da frase é ajustado através da função `devop_css()` para garantir que ela fique bem posicionada e visível.

# arquitetura

## O plugin Devops Challenge Júnior tem uma arquitetura simples, com base em três funções principais e utilizando hooks do WordPress para integração com o painel administrativo. Aqui está uma visão geral de como a arquitetura do plugin foi projetada:

devops-challenge-junior/
│
├── devops-challenge-junior.php    # Arquivo principal do plugin
└── README.md                      # Arquivo de documentação
