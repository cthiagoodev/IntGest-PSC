# IntGest PSC (Portal de Serviços ao Cidadão) 🏛️

![Status](https://img.shields.io/badge/Status-Em_Produção-success?style=for-the-badge) ![Category](https://img.shields.io/badge/Categoria-GovTech_|_IoT-orange?style=for-the-badge) ![Tech](https://img.shields.io/badge/Stack-Flutter_|_Kotlin-blue?style=for-the-badge)

> **Nota:** Este repositório é um **estudo de caso** de um software proprietário desenvolvido por mim na [IntellGest](https://www.linkedin.com/company/intellgest/). Ele serve como demonstração de portfólio técnico e **não contém o código-fonte original**.

---

## 📱 Sobre o Projeto

O **IntGest PSC** é uma plataforma de transformação digital (GovTech) desenhada para ser o canal único de interação entre o cidadão e o governo municipal. O sistema visa desburocratizar a máquina pública através de um ecossistema multicanal: um aplicativo móvel para uso pessoal e totens físicos de autoatendimento nas sedes dos órgãos.

O projeto promove a **Inclusão Digital Híbrida**: atende tanto quem prefere resolver tudo pelo celular quanto quem precisa ir presencialmente ao órgão, mas deseja um atendimento ágil e automatizado.

## 👨‍💻 Desafios de Engenharia & Hardware

Como Engenheiro responsável, liderei o desenvolvimento de duas frentes tecnológicas distintas que operam de forma integrada:

### 1. App Mobile (Flutter): O Hub de Serviços 📲
Um "Super App" que centraliza serviços de diversos órgãos que originalmente não conversavam entre si.
* **Desafio:** Criar padrões de interface (Design System) capazes de acomodar fluxos muito distintos (ex: emissão de IPTU vs. poda de árvores) mantendo a usabilidade simples para idosos e nativos digitais.

### 2. Totem de Autoatendimento (Android Nativo/Kotlin) 🖨️
Desenvolvimento de uma aplicação nativa robusta para rodar em quiosques físicos de atendimento (Totens).
* **Integração de Hardware (IoT):** Implementei a comunicação direta via USB/Bluetooth com **impressoras térmicas** utilizando o protocolo **ESC/POS**.
* **Funcionalidade:** O sistema gerencia a emissão de senhas e comprovantes físicos instantaneamente, exigindo controle preciso de buffer de impressão e tratamento de erros de hardware (papel acabou, impressora desconectada).

### 3. Transparência em Tempo Real 📄
Sincronização eficiente com bases de dados legadas da gestão pública para garantir que informações sobre requisitos, prazos e status de solicitações sejam sempre oficiais e atualizadas em tempo real, tanto no App quanto no Totem.

## 🛠️ Tech Stack

O ecossistema utiliza tecnologias específicas para cada necessidade:

* **Mobile App:**
    * **Framework:** Flutter
    * **Arquitetura:** Clean Architecture
* **Totem (Kiosk):**
    * **Linguagem:** Kotlin (Android Nativo)
    * **Hardware:** Integração USB/Serial com Impressoras Térmicas (ESC/POS Commands)
* **Integração:** REST APIs unificadas.
