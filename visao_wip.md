# ... Documento de visão

## 4 Ambiente do usuário

### 4.1 Ambiente físico

<!-- TODO: Adicionar informações do totem -->
Não possui ambiente físico, apenas digital.

### 4.2 Ambiente computacional

Os usuários que irão utilizar o sistema devem possuir um dispositivo móvel (celular, tablet) que possua acesso a internet para poder realizar o acesso ao sistema e realizar suas operações.

## 5 Público alvo

O público-alvo do aplicativo Vaga Livre são motoristas frequentes que enfrentam as dificuldades da busca por vagas de estacionamento em seu dia a dia. Seja para encontrar um lugar rapidamente em áreas congestionadas, evitar o estresse de dar voltas desnecessárias ou simplesmente ganhar praticidade e otimizar seu tempo, o Vaga Livre oferece uma solução completa para quem busca tranquilidade e segurança ao estacionar seu veículo.

## 6 Não Escopo do Vaga-Livre

1. Foco no Usuário Final
    - Aplicativo para Proprietários: No momento, o foco do projeto está em desenvolver um aplicativo completo e intuitivo para o usuário final, o motorista que busca uma vaga de estacionamento. O desenvolvimento de um aplicativo para proprietários de estacionamentos será considerado em etapas posteriores.
    - Gerenciamento por Proprietários: As funcionalidades relacionadas à gestão de vagas por parte dos proprietários, como atualização de disponibilidade, controle de acesso e preços dinâmicos, não serão contempladas nesta fase.

2. Integração com Hardware:
    - Integração com Totens: A integração com totens de entrada e saída dos estacionamentos não está prevista no escopo inicial. O foco está na busca e reserva de vagas através do aplicativo.
    - Pagamento via App: O pagamento da tarifa de estacionamento não será realizado através do aplicativo nesta fase. Os métodos tradicionais de pagamento (dinheiro, cartão, etc.) serão utilizados.

3. Expansão Geográfica:
    - Abrangência Nacional: A plataforma Vaga Livre será inicialmente lançada em uma região específica, com foco na validação do modelo de negócio e na otimização da experiência do usuário. A expansão para outras cidades e regiões será considerada em etapas posteriores.

4. Visualização detalhada do Estacionamento
    - Fotos e vídeos do local, mapa interativo com trajeto e informações detalhadas sobre o estacionamento (preço por hora, tipos de vagas, serviços disponíveis, regras e normas, etc.) serão consideradas em etapas posteriores do projeto.

5. Funcionalidades Adicionais:
    - Sistema de Navegação: A integração com sistemas de navegação para direcionamento ao estacionamento não será implementada nesta fase. O foco está na busca e reserva de vagas.

## 7 Características do Produto

Esta seção lista os requisitos de produto derivado das necessidades dos usuários.

### 7.1 Necessidades do Usuário

|| Índice | Descrição
-|-|-
`Conta e Acesso` | 001 | Registro de novos usuários com informações básicas (nome, emai, senha, etc)
|| 002 | Login com autênticação segura
|| 003 | Opção de logout e exclusão de conta
| `Localização e Busca de Estacionamentos` | 004 | Busca de estacionamentos por nome ou características 
|| 005 | Busca de estacionamentos por meio de proximidade com localização (endereço digitado ou localização atual)
| `Visualização Detalhada de Estacionamentos` | 006 | Informações detalhadas sobre o estacionamento, como preço por hora, tipo de vagas, serviços disponíveis, regras e normas, etc
|| 006 | Opção de abrir rota para o estacionamento em app externo
| `Reserva de Vagas` | 007 | Seleção de data e horário desejados para a reserva da vaga
|| 008 | Confirmação da reserva por meio do pagamento
|| 009 | Cancelamento ou alteração da reserva com antecedência
| `Gerenciamento de Reservas` | 010 | Visualização de todas as reservas ativas futuras do usuário
|| 011 | Detalhes de reservas
|| 012 | Histórico de reservas para consulta e acompanhamento
| `Controle de Acesso ao estabelecimento` | 013 | Ativação da cancela do estacionamento por meio de leitura de QR code do totem
|| 014 | Acesso a contato do estacionamento para suporte em caso de ajuda para reservas

### 7.2 Necessidades do proprietário

| | índice | Descrição
-|-|-
| `Conta e Acesso` | 001 | Login com autenticação segura usando as informações repassadas pela equipe do Vaga Livre
| `Gerenciamento de Vagas` | 002 | Visualizar todas as vagas do seu estacionamento incluindo sua identificação e informações adicionais
|| 003 | Monitorar o status das vagas em tempo real, com atualizações instatâneas
|| 004 | Visualizar o histórico de reservas em seu estacionamento
| `Controle de Reservas` | 005 | Visualizar todas as reservas ativas e futuras com todos seus detalhes
|| 006 | Cancelar reservas manualmente
| `Gestão financeira` | 007 | Visualizar um resumo financeiro com o valor total em caixa (somatório de reservas finalizadas)
| `Configurações e Administração` | 008 | Definir horário de funcionamento do estacionamento, regras de reserva e tarifas (valor hora)


### 7.3 Cancela automática

Para simular o funcionamento da cancela automática, deve ser desenvolvido uma aplicação web que consiga performar as seguintes ações.

| | Índice | Descrição
-|-|-
| `Autorização de Entrada` | 001 | Solicitar ao sistema um novo código de verificação
|| 002 | Abrir a cancela
|| 003 | Fechar a cancela
|| 004 | Gerar um código QR que deve ser mostrado na tela
