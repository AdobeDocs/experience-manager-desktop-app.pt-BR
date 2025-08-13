---
title: Notas de versão do aplicativo de desktop [!DNL Adobe Experience Manager]
description: Detalhes da versão, melhorias, novos recursos, compatibilidade e links de download para o aplicativo de desktop  [!DNL Adobe Experience Manager] .
mini-toc-levels: 1
feature: Desktop App,Release Information
exl-id: e058e7a2-fcc8-4ad1-899e-20695db6bc72
source-git-commit: 3ee1e39553b81e335e07c278537a826df3ad9482
workflow-type: tm+mt
source-wordcount: '2502'
ht-degree: 9%

---

# Notas de versão do aplicativo de desktop [!DNL Adobe Experience Manager] {#release-notes-v2}

A seguir estão informações sobre a versão mais recente do aplicativo de desktop 3.0.0. A data de lançamento é 31 de julho de 2025.

Esta versão oferece vários aprimoramentos para coleções, uploads, entrada/saída, gerenciamento de metadados e usabilidade geral. Essas atualizações melhoram a eficiência, simplificam o manuseio de ativos e fornecem uma experiência mais intuitiva e em tempo real no aplicativo de desktop do AEM.

![Interface do Usuário do Aplicativo de Desktop](assets/dekktop-app-user-interface.png)

**Coleções**

* Agora você pode exibir, baixar e procurar coleções.

* Adição de suporte para baixar pastas disponíveis em coleções.

* O recurso de sincronização automática agora permite que os ativos baixados em coleções sincronizem periodicamente o Gerenciamento de ativos da AEM com o sistema de arquivos local.

* Ao atualizar um ativo que faz parte de uma coleção, o sistema o atualiza automaticamente na pasta de cache temporária e na interface do aplicativo de desktop.

**Carregamentos**

* Você pode fazer upload de ativos recém-criados de sua máquina local para o AEM, onde o repositório central está armazenado, e visualizá-los em seu aplicativo de desktop.

* O aplicativo de desktop agora identifica automaticamente novos arquivos criados em uma pasta já baixada no sistema de arquivos local e os carrega no AEM. O aplicativo de desktop deve ser mantido aberto para identificar os novos arquivos no sistema de arquivos local.

**Check-in e check-out**

* O recurso de check-in e check-out permite gerenciar o acesso a arquivos bloqueando um arquivo para edição (check-out) e salvando as alterações enquanto o disponibiliza para outros (check-in).

* Capacidade de arrastar um ativo do Aplicativo de desktop para o aplicativo do Creative Cloud de destino. O Aplicativo de desktop verifica automaticamente os ativos e os baixa no sistema de arquivos local.

**Metadados**

* É possível atribuir metadados ao criar uma nova pasta.

* O aplicativo de desktop do Experience Manager agora permite mover ativos ou pastas para um novo local, preservando os metadados, ajudando a organizar e simplificar seu sistema de arquivos.

* O aplicativo de desktop do AEM agora permite visualizar as propriedades da pasta, como miniatura da pasta, tamanho, caminho, data de criação, tags, metadados e assim por diante.

**Melhorias de usabilidade**


* O recurso de atualização automática atualiza automaticamente o conteúdo em tempo real, garantindo que você sempre veja as informações mais recentes sem recarregar manualmente a página e obter a lista de ativos atualizados.

* O recurso de fixar ou desfixar pasta permite manter pastas importantes facilmente acessíveis, fixando-as ou distorcendo a visualização ao desfixá-las quando não forem mais necessárias.

* O recurso Renomear título permite atualizar ou modificar facilmente o título de um ativo, ajudando você a manter os nomes precisos e organizados conforme o conteúdo evolui.

* É possível preservar o arquivo original e fazer alterações em um arquivo semelhante, duplicando arquivos em locais locais e na nuvem usando a operação duplicar arquivos.

* A opção de exportação agora permite baixar arquivos e pastas selecionados do Aplicativo de desktop para o local de destino específico em uma estrutura simples.

* Agora é possível acessar ativos na exibição de Cartão, em Grade ou em Árvore para obter um layout limpo, organizado e visualmente atraente dos ativos.

* Vários rótulos para várias opções são atualizados na interface para tornar o aplicativo mais intuitivo.

As **versões [!DNL Experience Manager] com suporte** são:

* [!DNL Experience Manager] como [!DNL Cloud Service]. Consulte as [notas de versão](https://experienceleague.adobe.com/pt-br/docs/experience-manager-cloud-service/content/release-notes/home).
* [!DNL Experience Manager] 6.5.0 ou mais recente, no Adobe Managed Services (AMS) ou no local. Consulte as [notas de versão do service pack](https://experienceleague.adobe.com/pt-br/docs/experience-manager-65/content/release-notes/release-notes).

O aplicativo de desktop [!DNL Adobe Experience Manager] está disponível para os **sistemas operacionais** a seguir:

* macOS X 10.14 ou mais recente, com as correções de erros mais recentes.
* Windows 10 com os service packs e correções de erros mais recentes.

Duas versões do instalador do Windows estão disponíveis para o aplicativo de desktop AEM versão 2.3.1 e versões posteriores. O instalador básico instala o aplicativo de desktop do AEM no diretório de dados do aplicativo local do usuário. A Adobe recomenda esse processo de instalação para a maioria de seus usuários. Um instalador Enterprise Windows também está disponível, o qual instala o aplicativo AEM Desktop no diretório compartilhado Arquivos de programas. Esses dois instaladores instalam a mesma versão do aplicativo de desktop do AEM, sem diferenças de funcionalidade.

As **URLs de download** do sistema operacional suportado são:

| Sistema operacional | [!DNL Experience Manager] as a [!DNL Cloud Service] | [!DNL Experience Manager] 6.x |
|---|---|---|
| macOS (v3.0.0) | [Link de download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aemcloud.html?package=/content/software-distribution/en/details.html/content/dam/aemcloud/public/aem-desktop-app/aem-desktop-osx-x64-3.0.0.dmg) | [Link de download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/adobe/aem-desktop-app/aem-desktop-osx-x64-3.0.0.dmg) |
| macOS Apple Silicon (M1) (v3.0.0) | [Link de download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aemcloud.html?package=/content/software-distribution/en/details.html/content/dam/aemcloud/public/aem-desktop-app/aem-desktop-osx-arm64-3.0.0.dmg) | [Link de download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/adobe/aem-desktop-app/aem-desktop-osx-arm64-3.0.0.dmg) |
| Windows de 64 bits (v3.0.0) | [Link de download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aemcloud.html?package=/content/software-distribution/en/details.html/content/dam/aemcloud/public/aem-desktop-app/aem-desktop-win-x64-3.0.0.exe) | [Link de download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/adobe/aem-desktop-app/aem-desktop-win-x64-3.0.0.exe) |
| Windows Enterprise de 64 bits (v3.0.0) | [Link de download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aemcloud.html?package=/content/software-distribution/en/details.html/content/dam/aemcloud/public/aem-desktop-app/aem-desktop-win-x64-ent-3.0.0.msi) | [Link de download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/adobe/aem-desktop-app/aem-desktop-win-x64-ent-3.0.0.msi) |
| macOS (v2.3.3) | [Link de download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aemcloud.html?package=/content/software-distribution/en/details.html/content/dam/aemcloud/public/aem-desktop-app/aem-desktop-osx-x64-2.3.3.dmg) | [Link de download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/adobe/aem-desktop-app/aem-desktop-osx-x64-2.3.3.dmg) |
| macOS Apple Silicon (M1) (v2.3.3) | [Link de download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aemcloud.html?package=/content/software-distribution/en/details.html/content/dam/aemcloud/public/aem-desktop-app/aem-desktop-osx-arm64-2.3.3.dmg) | [Link de download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/adobe/aem-desktop-app/aem-desktop-osx-arm64-2.3.3.dmg) |
| Windows de 64 bits (v2.3.3) | [Link de download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aemcloud.html?package=/content/software-distribution/en/details.html/content/dam/aemcloud/public/aem-desktop-app/aem-desktop-win-x64-2.3.3.exe) | [Link de download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/adobe/aem-desktop-app/aem-desktop-win-x64-2.3.3.exe) |
| Windows Enterprise de 64 bits (v2.3.3) | [Link de download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aemcloud.html?package=/content/software-distribution/en/details.html/content/dam/aemcloud/public/aem-desktop-app/aem-desktop-win-x64-2.3.3.msi) | [Link de download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/adobe/aem-desktop-app/aem-desktop-win-x64-2.3.3.msi) |
| macOS (v2.3.1) | [Link de download](https://nam04.safelinks.protection.outlook.com/?url=https%3A%2F%2Fexperience.adobe.com%2F%23%2Fdownloads%2Fcontent%2Fsoftware-distribution%2Fen%2Faemcloud.html%3Fpackage%3D%2Fcontent%2Fsoftware-distribution%2Fen%2Fdetails.html%2Fcontent%2Fdam%2Faemcloud%2Fpublic%2Faem-desktop-app%2Faem-desktop-osx-x64-2.3.1.dmg&data=05%7C02%7Canujm%40adobe.com%7Cfcf599743bd649c5cd7308dcab9ea5cd%7Cfa7b1b5a7b34438794aed2c178decee1%7C0%7C0%7C638573945081954149%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C0%7C%7C%7C&sdata=mwSX5ilZL0he2raIx8t5ecQ%2FWuizky4MpcCXX3mEN38%3D&reserved=0) | [Link de download](https://nam04.safelinks.protection.outlook.com/?url=https%3A%2F%2Fexperience.adobe.com%2F%23%2Fdownloads%2Fcontent%2Fsoftware-distribution%2Fen%2Faem.html%3Fpackage%3D%2Fcontent%2Fsoftware-distribution%2Fen%2Fdetails.html%2Fcontent%2Fdam%2Faem%2Fpublic%2Fadobe%2Fpackages%2Fadobe%2Faem-desktop-app%2Faem-desktop-osx-x64-2.3.1.dmg&data=05%7C02%7Canujm%40adobe.com%7Cfcf599743bd649c5cd7308dcab9ea5cd%7Cfa7b1b5a7b34438794aed2c178decee1%7C0%7C0%7C638573945081981239%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C0%7C%7C%7C&sdata=LJH3OCFq7yRykN4wU8HN9%2FBXC%2BjfXLJH4QizeFZfRHE%3D&reserved=0) |
| macOS Apple Silicon (M1) (v2.3.1) | [Link de download](https://nam04.safelinks.protection.outlook.com/?url=https%3A%2F%2Fexperience.adobe.com%2F%23%2Fdownloads%2Fcontent%2Fsoftware-distribution%2Fen%2Faemcloud.html%3Fpackage%3D%2Fcontent%2Fsoftware-distribution%2Fen%2Fdetails.html%2Fcontent%2Fdam%2Faemcloud%2Fpublic%2Faem-desktop-app%2Faem-desktop-osx-arm64-2.3.1.dmg&data=05%7C02%7Canujm%40adobe.com%7Cfcf599743bd649c5cd7308dcab9ea5cd%7Cfa7b1b5a7b34438794aed2c178decee1%7C0%7C0%7C638573945081965822%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C0%7C%7C%7C&sdata=2YENn0tDduiucogClt6aBZHDOE6dbzBdigq8VQawIO0%3D&reserved=0) | [Link de download](https://nam04.safelinks.protection.outlook.com/?url=https%3A%2F%2Fexperience.adobe.com%2F%23%2Fdownloads%2Fcontent%2Fsoftware-distribution%2Fen%2Faem.html%3Fpackage%3D%2Fcontent%2Fsoftware-distribution%2Fen%2Fdetails.html%2Fcontent%2Fdam%2Faem%2Fpublic%2Fadobe%2Fpackages%2Fadobe%2Faem-desktop-app%2Faem-desktop-osx-arm64-2.3.1.dmg&data=05%7C02%7Canujm%40adobe.com%7Cfcf599743bd649c5cd7308dcab9ea5cd%7Cfa7b1b5a7b34438794aed2c178decee1%7C0%7C0%7C638573945081986151%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C0%7C%7C%7C&sdata=jCepldg4dMej0%2BrK2mUonXwqsWL8ksE8%2BLMSgsH9qTA%3D&reserved=0) |
| Windows de 64 bits (v2.3.1) | [Link de download](https://nam04.safelinks.protection.outlook.com/?url=https%3A%2F%2Fexperience.adobe.com%2F%23%2Fdownloads%2Fcontent%2Fsoftware-distribution%2Fen%2Faemcloud.html%3Fpackage%3D%2Fcontent%2Fsoftware-distribution%2Fen%2Fdetails.html%2Fcontent%2Fdam%2Faemcloud%2Fpublic%2Faem-desktop-app%2Faem-desktop-win-x64-2.3.1.exe&data=05%7C02%7Canujm%40adobe.com%7Cfcf599743bd649c5cd7308dcab9ea5cd%7Cfa7b1b5a7b34438794aed2c178decee1%7C0%7C0%7C638573945081970892%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C0%7C%7C%7C&sdata=sRn2UWW%2Bi7SMEvSO74ZGGvJ40vHh1KhLc7zAfKc37Es%3D&reserved=0) | [Link de download](https://nam04.safelinks.protection.outlook.com/?url=https%3A%2F%2Fexperience.adobe.com%2F%23%2Fdownloads%2Fcontent%2Fsoftware-distribution%2Fen%2Faem.html%3Fpackage%3D%2Fcontent%2Fsoftware-distribution%2Fen%2Fdetails.html%2Fcontent%2Fdam%2Faem%2Fpublic%2Fadobe%2Fpackages%2Fadobe%2Faem-desktop-app%2Faem-desktop-win-x64-2.3.1.exe&data=05%7C02%7Canujm%40adobe.com%7Cfcf599743bd649c5cd7308dcab9ea5cd%7Cfa7b1b5a7b34438794aed2c178decee1%7C0%7C0%7C638573945081991004%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C0%7C%7C%7C&sdata=aQWZtEK%2F3cWX8n8Au%2FwZ5Zd9xPVo5phvk%2FuF%2Be0HRrE%3D&reserved=0) |
| Windows Enterprise de 64 bits (v2.3.1) | [Link de download](https://nam04.safelinks.protection.outlook.com/?url=https%3A%2F%2Fexperience.adobe.com%2F%23%2Fdownloads%2Fcontent%2Fsoftware-distribution%2Fen%2Faemcloud.html%3Fpackage%3D%2Fcontent%2Fsoftware-distribution%2Fen%2Fdetails.html%2Fcontent%2Fdam%2Faemcloud%2Fpublic%2Faem-desktop-app%2Faem-desktop-win-x64-2.3.1.msi&data=05%7C02%7Canujm%40adobe.com%7Cfcf599743bd649c5cd7308dcab9ea5cd%7Cfa7b1b5a7b34438794aed2c178decee1%7C0%7C0%7C638573945081976350%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C0%7C%7C%7C&sdata=v9C0sLDSkuL%2FMIyae2WkbitJPVgSlAw2BqcaH5Im0uw%3D&reserved=0) | [Link de download](https://nam04.safelinks.protection.outlook.com/?url=https%3A%2F%2Fexperience.adobe.com%2F%23%2Fdownloads%2Fcontent%2Fsoftware-distribution%2Fen%2Faem.html%3Fpackage%3D%2Fcontent%2Fsoftware-distribution%2Fen%2Fdetails.html%2Fcontent%2Fdam%2Faem%2Fpublic%2Fadobe%2Fpackages%2Fadobe%2Faem-desktop-app%2Faem-desktop-win-x64-2.3.1.msi&data=05%7C02%7Canujm%40adobe.com%7Cfcf599743bd649c5cd7308dcab9ea5cd%7Cfa7b1b5a7b34438794aed2c178decee1%7C0%7C0%7C638573945081995827%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C0%7C%7C%7C&sdata=2btCh0aIrUBiyeG37K9YorvzTeIJOggbq%2FRauUMn4LY%3D&reserved=0) |
| macOS (v2.3.0) | [Link de download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aemcloud.html?package=/content/software-distribution/en/details.html/content/dam/aemcloud/public/aem-desktop-app/aem-desktop-osx-x64-2.3.0.dmg) | [Link de download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/adobe/aem-desktop-app/aem-desktop-osx-x64-2.3.0.dmg) |
| macOS Apple Silicon (M1) (v2.3.0) | [Link de download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aemcloud.html?package=/content/software-distribution/en/details.html/content/dam/aemcloud/public/aem-desktop-app/aem-desktop-osx-arm64-2.3.0.dmg) | [Link de download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/adobe/aem-desktop-app/aem-desktop-osx-arm64-2.3.0.dmg) |
| Windows de 64 bits (v2.3.0) | [Link de download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aemcloud.html?package=/content/software-distribution/en/details.html/content/dam/aemcloud/public/aem-desktop-app/aem-desktop-win-x64-2.3.0.exe) | [Link de download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/adobe/aem-desktop-app/aem-desktop-win-x64-2.3.0.exe) |
| macOS (v2.2.2) | [Link de download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aemcloud.html?package=/content/software-distribution/en/details.html/content/dam/aemcloud/public/aem-desktop-app/aem-desktop-osx-x64-2.2.2.dmg) | [Link de download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/adobe/aem-desktop-app/aem-desktop-osx-x64-2.2.2.dmg) |
| macOS Apple Silicon (M1) (v2.2.2) | [Link de download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aemcloud.html?package=/content/software-distribution/en/details.html/content/dam/aemcloud/public/aem-desktop-app/aem-desktop-osx-arm64-2.2.2.dmg) | [Link de download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/adobe/aem-desktop-app/aem-desktop-osx-arm64-2.2.2.dmg) |
| Windows de 64 bits (v2.2.2) | [Link de download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aemcloud.html?package=/content/software-distribution/en/details.html/content/dam/aemcloud/public/aem-desktop-app/aem-desktop-win-x64-2.2.2.exe) | [Link de download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/adobe/aem-desktop-app/aem-desktop-win-x64-2.2.2.exe) |
| macOS (v2.2.1) | [Link de download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aemcloud.html?package=/content/software-distribution/en/details.html/content/dam/aemcloud/public/aem-desktop-app/aem-desktop-osx-x64-2.2.1.dmg) | [Link de download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/adobe/aem-desktop-app/aem-desktop-osx-x64-2.2.1.dmg) |
| macOS Apple Silicon (M1) (v2.2.1) | [Link de download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aemcloud.html?package=/content/software-distribution/en/details.html/content/dam/aemcloud/public/aem-desktop-app/aem-desktop-osx-arm64-2.2.1.dmg) | [Link de download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/adobe/aem-desktop-app/aem-desktop-osx-arm64-2.2.1.dmg) |
| Windows de 64 bits (v2.2.1) | [Link de download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aemcloud.html?package=/content/software-distribution/en/details.html/content/dam/aemcloud/public/aem-desktop-app/aem-desktop-win-x64-2.2.1.exe) | [Link de download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/adobe/aem-desktop-app/aem-desktop-win-x64-2.2.1.exe) |
| macOS (v2.2.0) | [Link de download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aemcloud.html?package=/content/software-distribution/en/details.html/content/dam/aemcloud/public/aem-desktop-app/aem-desktop-osx-x64-2.2.0.dmg) | [Link de download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/adobe/aem-desktop-app/aem-desktop-osx-x64-2.2.0.dmg) |
| macOS Apple Silicon (M1) (v2.2.0) | [Link de download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aemcloud.html?package=/content/software-distribution/en/details.html/content/dam/aemcloud/public/aem-desktop-app/aem-desktop-osx-arm64-2.2.0.dmg) | [Link de download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/adobe/aem-desktop-app/aem-desktop-osx-arm64-2.2.0.dmg) |
| Windows de 64 bits (v2.2.0) | [Link de download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aemcloud.html?package=/content/software-distribution/en/details.html/content/dam/aemcloud/public/aem-desktop-app/aem-desktop-win-x64-2.2.0.exe) | [Link de download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/adobe/aem-desktop-app/aem-desktop-win-x64-2.2.0.exe) |
| macOS (v2.1.5.0) | [Link de download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aemcloud.html?package=/content/software-distribution/en/details.html/content/dam/aemcloud/public/aem-desktop-app/aem-desktop-osx-2.1.5.0.dmg) | [Link de download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/adobe/aem-desktop-app/aem-desktop-osx-2.1.5.0.dmg) |
| Windows de 64 bits (v2.1.5.0) | [Link de download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aemcloud.html?package=/content/software-distribution/en/details.html/content/dam/aemcloud/public/aem-desktop-app/aem-desktop-win64-2.1.5.0.exe) | [Link de download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/adobe/aem-desktop-app/aem-desktop-win64-2.1.5.0.exe) |
| Windows de 32 bits (v2.1.5.0) | [Link de download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aemcloud.html?package=/content/software-distribution/en/details.html/content/dam/aemcloud/public/aem-desktop-app/aem-desktop-win32-2.1.5.0.exe) | [Link de download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/adobe/aem-desktop-app/aem-desktop-win32-2.1.5.0.exe) |
| macOS (v2.1.4.0) | [Link de download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aemcloud.html?package=/content/software-distribution/en/details.html/content/dam/aemcloud/public/aem-desktop-app/aem-desktop-osx-2.1.4.0.dmg) | [Link de download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/adobe/aem-desktop-app/aem-desktop-osx-2.1.4.0.dmg) |
| Windows de 64 bits (v2.1.4.0) | [Link de download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aemcloud.html?package=/content/software-distribution/en/details.html/content/dam/aemcloud/public/aem-desktop-app/aem-desktop-win64-2.1.4.0.exe) | [Link de download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/adobe/aem-desktop-app/aem-desktop-win64-2.1.4.0.exe) |
| Windows de 32 bits (v2.1.4.0) | [Link de download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aemcloud.html?package=/content/software-distribution/en/details.html/content/dam/aemcloud/public/aem-desktop-app/aem-desktop-win32-2.1.4.0.exe) | [Link de download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/adobe/aem-desktop-app/aem-desktop-win32-2.1.4.0.exe) |
| macOS (v2.1.3.4) | [Link de download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aemcloud.html?package=/content/software-distribution/en/details.html/content/dam/aemcloud/public/aem-desktop-app/aem-desktop-osx-2.1.3.4.dmg) | [Link de download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/adobe/aem-desktop-app/aem-desktop-osx-2.1.3.4.dmg) |
| Windows de 64 bits (v2.1.3.4) | [Link de download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aemcloud.html?package=/content/software-distribution/en/details.html/content/dam/aemcloud/public/aem-desktop-app/aem-desktop-win64-2.1.3.4.exe) | [Link de download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/adobe/aem-desktop-app/aem-desktop-win64-2.1.3.4.exe) |
| Windows de 32 bits (v2.1.3.1) | [Link de download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aemcloud.html?package=/content/software-distribution/en/details.html/content/dam/aemcloud/public/aem-desktop-app/aem-desktop-win32-2.1.3.1.exe) | [Link de download](https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/adobe/aem-desktop-app/aem-desktop-win32-2.1.3.1.exe) |

## Suporte para diferentes ativos e tipos de arquivos {#support-for-file-types}

O aplicativo dá suporte a ativos armazenados em [!DNL Experience Manager] que representam arquivos binários para suas operações básicas. A abertura de arquivos no aplicativo de desktop nativo depende da associação do sistema operacional dos tipos de arquivos específicos, como PNG ou JPG, para aplicativos específicos, como Mac Preview ou Adobe Photoshop.

Alguns tipos de arquivo oferecem suporte para a inserção de ativos vinculados no binário. O aplicativo baixa previamente os ativos vinculados, se o ativo estiver presente no repositório [!DNL Experience Manager] quando esses arquivos binários forem abertos usando o aplicativo de desktop. Os tipos de arquivos compatíveis no momento incluem o seguinte:

* [!DNL Adobe InDesign] arquivos (formato INDD)
* [!DNL Adobe Illustrator] arquivos (formato AI)
* [!DNL Adobe Photoshop] arquivos (formato PS)

O recurso é compatível com as versões do aplicativo acima para o [!DNL Adobe Creative Cloud] 2018 e o [!DNL Adobe Creative Cloud] 2019. O aplicativo usa uma abordagem heurística e de melhor correspondência para mapear os caminhos de desktop locais dos ativos vinculados para URLs no servidor [!DNL Experience Manager]. Baseia-se em algumas suposições:

* Os caminhos para os arquivos colocados no aplicativo nativo usam um caminho de área de trabalho global (posicionado a partir do compartilhamento de rede local mostrado com a opção [!UICONTROL Reveal]).

* Os caminhos são armazenados no registro XMP do arquivo pelo aplicativo nativo.

* [!DNL Experience Manager] extraiu o registro XMP com os caminhos para o registro de metadados do ativo.

* Os caminhos podem corresponder aos ativos em [!DNL Experience Manager], ou seja, os arquivos colocados também estão em [!DNL Experience Manager] sob um caminho correspondente.

## Novos recursos, melhorias e correções de erros {#what-is-new}

Para conhecer os detalhes, consulte [Novidades na v2.0](introduction.md#whats-new-v2).

**Atualizações no aplicativo v2.3.1**

* O novo instalador do Enterprise Windows instala o aplicativo em Arquivos de programas.
* Suporte para **Autenticação Básica** durante logons AEM e SSO.
* Número configurável de ativos permitidos durante a operação de upload

**Atualizações no aplicativo v2.3.0**

* Adição de Suporte para logon IMS. A integração IMS permite que o aplicativo de desktop execute a atualização do token de acesso automaticamente, permitindo que o usuário permaneça conectado por até 14 dias.

* Aprimoramento do suporte para proxies corporativos e filtragem da Web.

**Atualizações no aplicativo v2.2.2**

* (Somente para Windows) O aplicativo de desktop exibe uma tela em branco após a instalação das versões 2.2.0 e 2.2.1.

**Atualizações no aplicativo v2.2.1**

* O aplicativo de desktop exibe uma mensagem de erro de tempo limite de sessão quando você clica em **[!UICONTROL Sign In]**.

* Problemas ao acessar o aplicativo de desktop v2.2.0 no macOS.

* O aplicativo de desktop exibe uma mensagem de erro ao classificar ativos clicando em **[!UICONTROL Edited Locally]**.

**Atualizações no aplicativo v2.2.0**

* Suporte para Apple Silicon (M1).

* Capacidade de lembrar a cadeia de conexão ao fazer logon no aplicativo de desktop.

**Atualizações no aplicativo v2.1.5.0**

* O aplicativo de desktop para de responder quando você carrega arquivos em uma pasta que contém caracteres chineses (ASSETS-9237).

* o aplicativo de desktop substitui pontos por traços nos nomes de arquivo (ASSETS-10955).

**Atualizações no aplicativo v2.1.4.0**

A nova versão do aplicativo oferece correções de erros.

**Atualizações no aplicativo v2.1.3.4**

A nova versão do aplicativo oferece uma correção de erro.

**Atualizações no aplicativo v2.1.3.3**

A nova versão do aplicativo oferece uma correção de erro.

**Atualizações no aplicativo v2.1.3.2**

Esta versão do aplicativo oferece uma correção de erro.

**Atualizações no aplicativo v2.1.3.1**

O erro corrigido nesta versão é:

* As velocidades de upload e download de ativos melhoraram, mesmo com ativos grandes. Esta versão corrigiu um problema em que os uploads de ativos com o [!DNL desktop app] falhavam às vezes quando arquivos muito grandes eram carregados.

**Atualizar no aplicativo v2.1.2.0**

* Uma nova opção para [!UICONTROL Clear Cookies] é adicionada ao menu principal do aplicativo. Isso ajuda com possíveis problemas de logon, por exemplo, ao alterar uma conexão de um servidor para outro. Consulte [limpar cookies antes de se conectar](/help/using/troubleshoot.md#cannot-login-cookies-issue).

* Uma nova opção foi adicionada que, se selecionada, permite que o aplicativo carregue pastas e arquivos com nomes de nó em [!DNL Adobe Experience Manager] que correspondam aos nomes de arquivo e pasta locais. Esse processo garante a consistência entre nomes locais e carregados.

  Esse comportamento é semelhante ao comportamento padrão na versão 1 do aplicativo de desktop. Enquanto na versão atual, se a opção não estiver habilitada, os espaços em branco e os caracteres `% ; # , + ? ^ { } "` nos nomes de pastas serão substituídos por traços nos caminhos de pastas. Além disso, os caracteres em maiúsculas são convertidos em minúsculas nos caminhos de pastas. No entanto, em nomes de arquivos, os caracteres `# % { } ? &` são substituídos por traço; mas espaços em branco e caracteres maiúsculos são mantidos. Para obter mais informações, consulte [Preferências do aplicativo](/help/using/install-upgrade.md#set-preferences) e [Carregar e adicionar novos ativos](/help/using/upload-assets.md#upload-and-add-new-assets-to-aem).

**Atualizar no aplicativo v2.1.1.0**

* Uma configuração avançada permite que o aplicativo emule o comportamento do aplicativo v1.10 ao carregar pastas. Na v1.10, os nomes de nó criados no repositório respeitam os espaços e a capitalização dos nomes de pasta fornecidos pelo usuário. Na versão 2.1, o comportamento padrão é inalterado: vários espaços nos nomes de pastas são substituídos por hifens no nome do nó do repositório e os nomes dos nós são convertidos em minúsculas. Consulte [as preferências do aplicativo](/help/using/install-upgrade.md#set-preferences).

**Atualizar no aplicativo v2.1.0.0**

* Para fazer upload de ativos, os usuários agora podem arrastar os arquivos ou pastas para a interface do aplicativo, diretamente do Windows Explorer ou do Mac Finder. Esse processo funciona além da opção de upload disponível no aplicativo. Consulte [carregar ativos](/help/using/upload-assets.md#upload-and-add-new-assets-to-aem) <!-- CQ-4309527 -->

**Atualizar no aplicativo v2.0.3**

O erro corrigido nesta versão é:

* Correção do problema de logon para usuários do aplicativo no Windows que tentam acessar o repositório DAM em [!DNL Adobe Experience Manager] 6.5.5.0.

**Atualizações no aplicativo v2.0.2**

As correções de erros e atualizações são:

* A configuração de aceleração de upload agora está disponível para aumentar o desempenho do upload. Quando essa configuração é ativada, o aplicativo é carregado mais rapidamente usando mais threads locais do CPU e consome mais recursos.

* O ativo é carregado quando os nomes de arquivo ou caminhos que contêm determinados caracteres GB18030 são fixos. <!-- CQ-4283494 -->

* A opção Classificar por relevância está disponível após alternar para outro tipo de classificação nos resultados da pesquisa. <!-- CQ-4286874 -->

* O aplicativo de desktop agora lista subpastas sem a necessidade de atualização explícita. <!-- CQ-4285711 -->

* (Windows) Correção de um problema raro de interface de aplicativo inutilizável em algumas máquinas Windows. Os usuários não podem clicar na interface do aplicativo, pois ela aparece distorcida com a área de clique dos elementos da interface &quot;deslocados&quot; ao lado. <!-- CQ-4280785 -->

**Atualizações no aplicativo v2.0.1**

As correções de erros e atualizações são:

* Permitir opção para configurar o diretório `%Temp%` para corresponder ao caminho `%APPDATA%`. <!-- CQ-4282665 -->

* Permitir que os usuários façam logon no Autor [!DNL Experience Manager] por meio da autenticação SAML do Okta. <!-- CQ-4278134 -->

## Instruções de instalação {#installation-instructions-v2}

Para saber como instalar e configurar o aplicativo, consulte [Instalar [!DNL Experience Manager] aplicativo de desktop](install-upgrade.md).

Se você estiver atualizando de um aplicativo de desktop [!DNL Experience Manager] anterior, siga estas práticas recomendadas para transição que estão listadas em [atualizar da versão anterior](install-upgrade.md#upgrade-from-previous-version).

## Observações importantes sobre como funciona o aplicativo {#how-app-works}

É importante entender o seguinte sobre o aplicativo e como ele funciona.

* O aplicativo fornece controle total sobre operações que exigem transferência total de binários de ativos de e para [!DNL Experience Manager] (**Abrir**, **Editar**, **Carregar Alterações** e **Carregar Assets**).

   * Se quiser trabalhar com o ativo no desktop, você deve abrir, editar ou baixar explicitamente no desktop, individualmente, em uma pasta ou por meio de várias seleções.

   * Se você deseja obter alterações locais em ativos carregados em [!DNL Experience Manager], é necessário selecionar [!UICONTROL Upload Changes], individualmente ou por meio de várias seleções.

   * O aplicativo não é um &#39;cliente de sincronização&#39; que sincroniza ativos na área de trabalho e no [!DNL Experience Manager].

   * O aplicativo não fornece um compartilhamento de rede que mapeia o repositório [!DNL Experience Manager] como uma estrutura de pasta virtual.

* A lista de ativos mostrada pelo aplicativo se baseia no status do repositório do Assets. Os arquivos baixados localmente e subsequentemente renomeados nos arquivos locais ou na pasta de cache não são exibidos ou gerenciados com o aplicativo.

* Se o aplicativo não exibir os resultados esperados, clique no ícone atualizar na barra superior.

* O compartilhamento de rede local, mostrado quando você usa a ação [!UICONTROL Reveal File], mostra somente os arquivos (e pastas) que estão disponíveis localmente. O [!UICONTROL Reveal File] e o [!UICONTROL Reveal Folder] baixam previamente os ativos para ajudar a obter os ativos certos exibidos no compartilhamento de rede local.

* O compartilhamento de rede local SMB (Mac) / WebDAV (Win) é usado quando um aplicativo do Adobe Creative Cloud lê os arquivos de ativos vinculados/colocados em um arquivo nativo do aplicativo do Creative Cloud.

O diagrama a seguir ilustra o fluxo de ativos e arquivos da nuvem para o sistema de arquivos local e o oposto, conforme iniciado pelas ações do usuário.

![Fluxo de ativos do servidor [!DNL Experience Manager] para aplicativos de desktop nativos por meio do aplicativo de desktop](assets/da20_flow_diagram.png)

## Problemas conhecidos {#known-issues-v2}

**Problemas da interface do usuário:**

* Às vezes, a interface do aplicativo de desktop pode ficar em branco. Clique com o botão direito do mouse e clique em [!UICONTROL Refresh] para recarregar o aplicativo. Após essa atualização, você inicia na raiz do repositório DAM. As atualizações ou os status de seus ativos são retidos. <!-- CQ-4270267 -->

* Difícil de navegar pelas pastas/resultados de pesquisa sem um trackpad ou ponteiro do mouse. A barra de rolagem não é exibida com dispositivos de mouse sem roda. <!-- CQ-4269947 -->

* Raramente, a barra de andamento não é exibida corretamente quando o ativo de upload é alterado.

* Depois de aplicar e remover o filtro para localizar todos os ativos editados localmente, o aplicativo não leva os usuários até os resultados da pesquisa ou a visualização de pasta com os quais os usuários começaram a trabalhar. O aplicativo exibe a pasta raiz do repositório DAM.

* Às vezes, quando você se conecta a uma URL que não tem um servidor [!DNL Experience Manager] em execução, a tela de conexão fica sem resposta. Saia do aplicativo e reinicie.

**Problemas de CRUD (Create, Read, Update, and Delete, Criar, ler, atualizar e excluir):**

* Ao carregar alterações em um ativo com comentários, os comentários são armazenados com o ativo em [!DNL Experience Manager], mas não ficam visíveis como comentários de versão. Este problema foi resolvido em [!DNL Experience Manager] 6.4.5 e [!DNL Experience Manager] 6.5.1. A Adobe recomenda instalar os service packs mais recentes. <!-- CQ-4268990 -->

* Um usuário não pode cancelar transferências de ativos. Se você acionou uma transferência volumosa não intencional, saia do aplicativo e reinicie. <!-- CQ-4278940 -->

**Problemas de plataforma:**

* Às vezes, no Windows, o status de um ativo pode mudar imediatamente para [!UICONTROL Edited Locally] depois de abri-lo, mesmo que você não o tenha editado. Clique em [!UICONTROL Refresh] para atualizar.

>[!MORELIKETHIS]
>
>* [[!DNL Experience Manager] documentação das  [!DNL Cloud Service] as a](https://experienceleague.adobe.com/pt-br/docs/experience-manager-cloud-service)
>* Documentação do [[!DNL Experience Manager] as a [!DNL Cloud Service] [!DNL Assets]](https://experienceleague.adobe.com/pt-br/docs/experience-manager-cloud-service/content/assets/overview)
>* [Como usar [!DNL Experience Manager] aplicativo de desktop](using-desktop-app.md)
>* [Instalar e atualizar o aplicativo de desktop](install-upgrade.md)
>* [Práticas recomendadas e dicas para solução de problemas](troubleshoot.md)
