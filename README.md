<div align="center">

# Kataka Bot

<img src="https://github.com/KatakaBot/Imagens/blob/main/656f9b578c5d45d9869a0a52723dd335.gif" width="600">

### Um bot completo para moderação, tickets, automação e gerenciamento de servidores Discord.

![Node.js](https://img.shields.io/badge/Node.js-20+-339933?style=for-the-badge&logo=node.js&logoColor=white)
![discord.js](https://img.shields.io/badge/discord.js-14-5865F2?style=for-the-badge&logo=discord&logoColor=white)
![Discord](https://img.shields.io/badge/Discord-Bot-5865F2?style=for-the-badge&logo=discord&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)

### Links Rápidos

[Adicionar ao Discord](https://discord.com/oauth2/authorize?client_id=1318350075684192340&permissions=1100317059126&integration_type=0&scope=bot)
•
[Comandos](https://kataka.freehosting.dev/comandos)
•
[FAQ](https://kataka.freehosting.dev/faq)
•
[Termos](https://kataka.freehosting.dev/termos)
•
[Privacidade](https://kataka.freehosting.dev/privacidade)

</div>

---

> [!NOTE]
> Os comandos do Kataka são registrados **globalmente**. Após a primeira execução do bot, pode levar até 1 hora para os comandos aparecerem em todos os servidores.

## Sistema de Tickets

Painel de atendimento completo, configurável direto pelo Discord com `/panel`.

| Recursos                              |
| -------------------------------------- |
| Painel público com botões e menus      |
| Título, descrição, imagem e banner personalizáveis |
| Cargos de staff e de gerência          |
| Cargo de notificação da equipe         |
| Reivindicar, notificar e fechar ticket |
| Adicionar usuários extras ao ticket    |
| Banir e punir (timeout) pelo ticket    |
| Blacklist de usuários                  |
| Transcript automático em HTML          |
| Canal de logs e canal de transcript    |

| Comando   | Descrição                                    |
| --------- | --------------------------------------------- |
| `/panel`  | Abre o painel central de configuração de tickets |

> [!IMPORTANT]
> Configurar o sistema (`/panel`) é restrito ao **dono do servidor** ou a membros com permissão de **Administrador**. Atender tickets requer apenas os cargos de staff/gerência definidos no painel.

## Sistema de Moderação

<details>
<summary>Clique para expandir a lista completa de comandos</summary>

| Comando       | Descrição                              |
| ------------- | --------------------------------------- |
| `/ban`        | Banir membros                           |
| `/unban`      | Remover um banimento                    |
| `/unban-all`  | Remover todos os banimentos do servidor |
| `/kick`       | Expulsar membros                        |
| `/mute`       | Silenciar usuários (timeout)            |
| `/unmute`     | Remover silenciamento                   |
| `/role`       | Adicionar ou remover cargo de um membro |
| `/nick`       | Alterar apelido de um membro            |
| `/moveall`    | Mover todos de um canal de voz para outro |
| `/warn`       | Aplicar advertências                    |
| `/warnings`   | Consultar histórico de advertências     |
| `/clearwarn`  | Retirar advertências                    |
| `/clear`      | Apagar mensagens do canal               |
| `/nuke`       | Recriar o canal, apagando o histórico   |
| `/slowmode`   | Definir modo lento no canal             |
| `/lock`       | Bloquear envio de mensagens no canal    |
| `/unlock`     | Desbloquear o canal                     |
| `/hide`       | Ocultar o canal para membros comuns     |
| `/show`       | Reexibir o canal para membros comuns    |

</details>

## Sistema de Boas-Vindas

Configure mensagens automáticas para novos membros.

| Recursos                 |
| ------------------------ |
| Embeds personalizadas    |
| Placeholders dinâmicos   |
| Envio via webhook        |
| Canal configurável       |
| Imagens customizadas     |

| Comando     | Descrição                                    |
| ----------- | --------------------------------------------- |
| `/welcome`  | Abre o painel de configuração de boas-vindas |

<details>
<summary>Clique para expandir os placeholders disponíveis</summary>

```
{user}
{user.name}
{user.display_name}
{user.id}
{user.avatar}
{guild.name}
{guild.member_count}
{guild.icon}
{guild.owner}
{now}
```

</details>

## Sistema de Cargos por Seleção

Permita que seus membros escolham seus próprios cargos.

| Recursos                   |
| -------------------------- |
| Select Menus               |
| Cargos automáticos         |
| Embeds customizadas        |
| Envio via webhook          |
| Configuração simplificada  |

| Comando   | Descrição                                     |
| --------- | ----------------------------------------------- |
| `/pings`  | Abre o painel de configuração de cargos por seleção |

## Criador de Embeds

Crie embeds profissionais diretamente pelo Discord.

| Recursos                 |
| ------------------------ |
| Múltiplos embeds         |
| Título, descrição e cor personalizada |
| Thumbnail, imagem e footer |
| Autor                    |
| Botões com link          |
| Importar / exportar JSON |
| Envio via webhook        |

| Comando         | Descrição                          |
| --------------- | ------------------------------------ |
| `/embed criar`  | Abre o editor avançado de embeds    |
| `/say`          | Envia uma mensagem de texto simples |

## Utilidades

| Comando   | Descrição                          |
| --------- | ------------------------------------ |
| `/avatar` | Exibe o avatar de um membro         |
| `/banner` | Exibe o banner de perfil de um membro |
| `/ping`   | Mostra a latência atual do bot      |

---

# Instalação

## Clone o repositório

```bash
git clone https://github.com/KatakaBot/Kataka.git
```

```bash
cd Kataka
```

## Instale as dependências

```bash
npm install
```

## Configure o token

Copie `.env.example` para `.env` e preencha:

```env
DISCORD_TOKEN=SEU_TOKEN
CLIENT_ID=ID_DA_APLICACAO
```

## Execute

```bash
npm start
```

---

# Permissões Necessárias

| Permissão      | Necessária  |
| -------------- | ----------- |
| Administrador  | Recomendado |

<details>
<summary>Ou, sem Administrador, conceda estas permissões individualmente</summary>

| Permissão                                     | Necessária |
| ---------------------------------------------- | ---------- |
| Gerenciar Servidor                              | ✅ |
| Gerenciar Cargos                                | ✅ |
| Gerenciar Canais                                | ✅ |
| Gerenciar Apelidos                              | ✅ |
| Gerenciar Webhooks                              | ✅ |
| Banir Membros                                   | ✅ |
| Expulsar Membros                                | ✅ |
| Moderar Membros                                 | ✅ |
| Mover Membros                                   | ✅ |
| Gerenciar Mensagens                             | ✅ |
| Enviar Mensagens                                | ✅ |
| Incorporar Links                                | ✅ |
| Anexar Arquivos                                 | ✅ |
| Ler Histórico de Mensagens                      | ✅ |
| Usar Comandos de Aplicação                      | ✅ |
| Mencionar @everyone, @here e Todos os Cargos    | ✅ |

</details>

---

## Perguntas Frequentes

**P: O bot funciona em vários servidores ao mesmo tempo?**

R: Sim. As configurações de tickets, boas-vindas e advertências são completamente separadas por servidor, identificadas pelo ID de cada guild.

**P: Os dados são perdidos se o bot reiniciar?**

R: Não. Tickets, advertências, painéis de pings e configurações de boas-vindas ficam salvos em disco e persistem entre reinicializações.

**P: Quem pode configurar o bot no meu servidor?**

R: Apenas o dono do servidor ou membros com permissão de Administrador podem usar `/panel`, `/embed`, `/pings`, `/welcome` e `/say`.

**P: Posso importar um embed criado em outro lugar?**

R: Sim. No painel `/embed`, use "Importar JSON" para colar um embed no formato compatível com ferramentas como discohook.org.

---

# Créditos

**Desenvolvimento:** Kataka Network e Tuxifer

## Licença

Este projeto é licenciado sob a **MIT License**. Veja o arquivo LICENSE para mais detalhes.

<div align="center">

### ム

</div>
