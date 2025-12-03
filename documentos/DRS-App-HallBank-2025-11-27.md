# Informações Gerais  

**Nome do projeto:** App Bancário – “HallBank”  
**Data:** 27/11/2025  
**Autor:** Felipe Barbosa  
**v1.0** — 27/11/2025 — Versão inicial.  
**v2.0** — 03/12/2025 — Versão Atual.  
  
**Descrição:**  
*Este documento especifica escopo, restrições, definições e abreviações, requisitos funcionais e não funcionais e requisitos de interface para o protótipo do aplicativo HallBank. O objetivo é definir claramente o comportamento, as características e os limites do sistema.* 

## Escopo

O protótipo consiste em:  

Tela de Login  
Tela Principal (Dashboard)  
Tela Extra 1: Transferência PIX  
Tela Extra 2: Extrato Bancário  

## Restrições

1. O app será entregue somente como protótipo, sem backend real.  
2. A interação será limitada ao que o Figma permitir.  
3. Somente funcionalidades definidas no escopo serão implementadas.  

## Definições e Abreviações
**DRS:** Documento de Requisitos de Software.  
**Dashboard:** Painel visual que reúne informações e métricas importantes.  
**PIX:** Sistema de pagamento instantâneo do Banco Central.  
**Chave PIX:** Identificador usado para receber Pix (CPF, e-mail, telefone ou aleatória).  
**TED:** Transferência eletrônica entre bancos com liquidação no mesmo dia.  
**QR code:** Código visual escaneável que armazena informações.  
**Extrato:** Registro das movimentações de uma conta.  
**Gutter:** Espaço entre colunas em um layout.   
**Tipografia:** Conjunto de estilos e características das letras usadas no design.  
**Input:** Informação ou dado inserido pelo usuário ou sistema.  
**Output:** Resultado ou dado gerado e entregue pelo sistema.  

## Requisitos Funcionais (RF)
*Os requisitos funcionais foram organizados em grupos temáticos para facilitar leitura, manutenção e compreensão do comportamento geral do sistema. Cada grupo reúne funcionalidades relacionadas a um mesmo contexto de uso.*

**RF-A: Autenticação e Segurança**  
**RF01 - Autenticação**  
O sistema deve permitir que o usuário faça login utilizando CPF e senha.  
**RF02 - Esqueci Senha**  
O sistema deve permitir a recuperação de senha em caso de esquecimento.  
**RF03 - Visibilidade**  
O sistema deve permitir ao usuário ver ou não os dados de cpf e senha no ato da digitação. 
  
**RF-B: Navegação e Estrutura**  
**RF04 - Pesquisa**  
O sistema deve permitir que o usuário pesquise funcionalidades e opções com facilidade.  
**RF05 - Menu**  
O sistema deve apresentar um menu que permita ao usuário navegar entre as informações do dashboard e as do perfil.  
**RF06 - Notificações**  
O sistema deve informar ao usuário quando ele receber notificações. 
  
**RF-C: Funcionalidades Bancárias**
**RF07 - Extrato**  
O sistema deve permitir ao usuário ver informações das ultimas transações realizadas.  
**RF08 - Transferências**  
O sistema deve apresentar funções de transferência por PIX, TED e pagamento de boletos.  
**RF09 - Cartões**    
O sistema deve permitir que o usuário visualize informações sobre seus cartões.  
**RF10 - Investimentos**  
O sistema deve permitir que o usuário visualize informações de seus investimentos e de novos aos quais ele pode optar  
investir.  
 **RF11 - Módulo Pix**  
O sistema deve apresentar todas as funcionalidades relacionadas ao pix que inclui:  
RF11.1 - Pagamento:  
  
    • Pagamento por QR code.  
    • Pagamento por chave pix.  
    • Pagamento agendado.  

RF11.2 - Recebimento:  
  
    • Receber por QR code.  
    • Contatos pix.  

RF11.3 - Gerenciamento de Chaves:  
  
    • O sistema deve permitir ao usuário gerenciar as próprias chaves pix.  

## Requisitos não Funcionais (RNF)

**RNF01 – Usabilidade**  
O layout deve seguir padrões modernos e apresentar navegação simples e intuitiva.  
**RNF02 – Consistência Visual**  
Todas as telas devem usar a mesma paleta, espaçamentos e tipografia.  
**RNF03 – Responsividade**  
As interfaces devem manter boa legibilidade e organização visual em diferentes tamanhos de tela mobile.  

## Requisitos de Interface (RI)
*Os requisitos de interface definem as diretrizes visuais, componentes, estilos e padrões adotados na construção do protótipo.*  
   
**RI01 - Paleta de cores**  
*A paleta foi definida com foco em transmitir credibilidade e confiança ao usuário, utilizando o azul como cor primária por sua forte associação psicológica com segurança e estabilidade em interfaces financeiras.*  
  
    • Cor primária: #277EEF  
    • Cor secundária: #FFFFFF  
    • Cor campo input: #E6E6E6  
    • Cor campo pesquisa: #B5B5B5  
    • Cor texto simples: #000000  

**RI02 -  Tipografia**  
*As famílias tipográficas adotadas foram obtidas do serviço Google Fonts, assegurando disponibilidade gratuita, otimização para web e consistência visual entre dispositivos.*  
  
RI02.1 - Fontes:  
  
    • Changa One: Utilizada na logo para as letras "HB".  
    • Lobster: Utilizada no nome "HallBank" junto a logo.  
    • Cantora One: Utilizada para todos os outros demais casos.  

RI02.2 - Tamanho:  
  
    • 15px - 16px: textos informativos e botões menores.  
    • 20px: texto de botões maiores.  
    • 32px: Textos grandes.  

**RI03 - Grid e Estrutura de Layout**  
*Este projeto utiliza um grid baseado no 4-Point System, amplamente adotado em interfaces mobile modernas.*   
   
RI03.1 - Grid utilizado:  
  
    • 8 colunas.  
    • Largura da coluna: proporcional ao dispositivo.  
    • Gutter: 16px  
    • Margem lateral: 16px  

RI03.2 - Dimensões de componentes:  
  
    • Icones: 20px e 40px.  
    • Input e Output: 299px de largura e 57px de altura.  
    • Botões menores: 30px de altura.  
    • Arredondamento de canto: 20px.  

RI03.3 - Estilos e efeitos visuais:  
  
    • Sombra Projetada em cards: x: 4px, y: 4px, desfoque: 5px, tamanho: 1px e opacidade: 25%.  

**RI04 - Área de Funcionalidades**  
*O sistema deve apresentar áreas no layout dedicadas as seguintes funcionalidades:*  
  
    • Exibir saldo do usuário.  
    • Botões para ações rápidas de transferência PIX, TED e boletos com seus respectivos icones.  
    • Investimentos, com cards contendo informações de cada investimento.  
    • Barra de pesquisa que seja identificada com um icone de lupa.  
    • Botão com icone que acesse a área de cartões.  
    • Área clicável com icone que acesse as informações de perfil.  
    • Área de notificações com icone de sino.  
    • Exibir agência e conta do usuário.  

**RI05 - Tela Extrato**  
O sistema deve apresentar as informações do extrato bancário da seguinte forma:  
  
    • Sessões de cada dia com as transações realizadas no determinado dia.  
    • As sessões devem apresentar a data na parte superior.  
    • Cada transação deve exibir o valor, o horário, se foi recebido ou enviado e quem realizou a ação.  
    • Botão para voltar para a tela de dashboard.  

**RI06 - Tela Pix**  
O sistema deve apresentar as informações e funcionalidades pix em uma tela exclusiva da seguinte forma:  
  
    • Botões de pagar e receber pix em formato de card com o icone e o texto de cada função.  
    • Sessão que exiba as chaves pix do usuário.  
    • Botão para voltar para a tela de dashboard.  