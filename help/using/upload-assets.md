---
title: 'Carregar ativos usando o aplicativo de desktop  [!DNL Experience Manager] '
description: Carregar ativos usando o aplicativo de desktop  [!DNL Adobe Experience Manager] .
feature: Desktop App,Asset Management
exl-id: f082c712-dc04-4bed-bac8-fa78f93de1c7
source-git-commit: db592420ded4d2f7288982a1ea17618484c82537
workflow-type: tm+mt
source-wordcount: '798'
ht-degree: 1%

---

# Upload de ativos {#upload-assets}

Os usuários do aplicativo de desktop do AEM com direitos para adicionar ativos podem adicionar ativos (como imagens, documentos, vídeos ou outras mídias).

## Editar ativos e carregar ativos atualizados para [!DNL Experience Manager] {#edit-assets-upload-updated-assets}

Abra ativos para edição quando quiser fazer alterações e carregue os ativos atualizados no servidor [!DNL Experience Manager]. Para evitar conflitos com as edições de outros usuários, use o aplicativo para iniciar uma sessão de edição. Antes de começar a editar, verifique se o ativo não tem um ícone de cadeado indicando que outro usuário está editando o ativo.

Para editar um ativo, pesquise pelo ativo ou navegue até o local do ativo. Clique em ![Mais ícone](assets/do-not-localize/more2_da2.png) e em **[!UICONTROL Edit]**.

Use **[!UICONTROL Toggle Check-out]** para bloquear o ativo e evitar conflitos com edições de outros usuários nas seguintes situações:

* Você começou a editar um ativo sem fazer o check-out dele primeiro (digamos apenas abrindo-o).
* Você pretende começar a editar um ativo em breve e não deseja que outros editem.

Quando terminar de fazer as edições, o aplicativo exibirá o status **[!UICONTROL Edited Locally]** dos ativos alterados. Todas as alterações salvas nos ativos são somente locais até você carregar as alterações em [!DNL Experience Manager]. Para carregar um indivíduo ou alguns ativos individualmente, clique em **[!UICONTROL Upload Changes]** nas opções de um ativo. Uma versão do ativo é criada em [!DNL Experience Manager]. Usando a interface da Web de [!DNL Assets], você pode ver o histórico de ativos na [exibição da Linha do Tempo](https://experienceleague.adobe.com/en/docs/experience-manager-65/content/assets/using/activity-stream).

![Opção Carregar alterações no aplicativo](assets/upload_changes_single1_da2.png "Opção Carregar alterações no aplicativo")

![Opção Carregar alterações ao visualizar uma grande visualização de um ativo](assets/upload_changes_single2_da2.png "Opção Carregar alterações ao visualizar uma grande visualização de um ativo")

Para obter as práticas recomendadas sobre a edição colaborativa, consulte [Fluxo de trabalho avançado: colaborar nos mesmos arquivos e evitar conflitos de edição](#adv-workflow-collaborate-avoid-conflicts).

Nos casos a seguir, talvez você queira descartar as alterações e edições no ativo local. Clique em **[!UICONTROL Discard Changes]**.

* Se não quiser salvar suas alterações localmente no [!DNL Experience Manager].
* Comece a fazer alterações no ativo original depois de salvar algumas alterações.
* Pare de editar o ativo, pois ele não é mais necessário.

Se necessário, alterne o check-out. O ativo atualizado é removido da pasta de cache local e é baixado novamente quando você o edita ou abre.

## Carregar e adicionar novos ativos a [!DNL Experience Manager] {#upload-and-add-new-assets-to-aem}

Os usuários podem adicionar novos ativos ao repositório DAM. Por exemplo, você pode ser um fotógrafo ou um contratado de agências que deseja adicionar um grande número de fotos de uma sessão de fotos ao repositório do [!DNL Experience Manager]. Para adicionar novo conteúdo a [!DNL Experience Manager], selecione ![opção de carregamento na nuvem](assets/do-not-localize/upload_to_cloud_da2.png) na barra superior do aplicativo. Navegue até os arquivos de ativos no sistema de arquivos local e clique em **[!UICONTROL Select]**. Como alternativa, para fazer upload de ativos, arraste os arquivos ou as pastas para a interface do aplicativo. No Windows, se você arrastar ativos em uma pasta dentro do aplicativo, os ativos serão carregados na pasta. Se demorar mais para carregar, o aplicativo exibe uma barra de progresso.

<!-- ![Download progress bar for large-sized assets](assets/upload_status_da2.png "Download progress bar for large-sized assets")
-->

Você pode fazer upload de pastas ou arquivos individuais do seu sistema de arquivos local. A hierarquia de uma pasta é preservada ao ser carregada. Antes de carregar ativos em massa, consulte [Carregamentos em massa](#bulk-upload-assets).

Para exibir a lista de ativos transferidos em uma determinada sessão, clique em **[!UICONTROL View]** > **[!UICONTROL Assets transfers]**. A lista permite visualizar e verificar rapidamente as transferências de arquivos da sessão atual.

![Lista de ativos transferidos em uma sessão específica](assets/assets_transfered_da2.png "Lista de ativos transferidos em uma sessão específica")

Você pode controlar a simultaneidade de carregamento (aceleração) na configuração **[!UICONTROL Preferences]** > **[!UICONTROL Upload acceleration]**. Em geral, mais simultaneidade resulta em uploads mais rápidos, mas pode consumir muitos recursos, consumindo mais potência de processamento da máquina local. Se o sistema for lento, tente fazer upload novamente usando um valor de simultaneidade menor.

>[!NOTE]
>
>A lista de transferência não é persistente e não estará disponível se você sair do aplicativo e reabri-la.

## Fazer upload de ativos em massa {#bulk-upload-assets}

Usuários ou organizações, como fotógrafos ou agências de criação, podem criar vários ativos locais durante atividades como sessões de fotos, retoque ou seleção em um conjunto maior. Essas tarefas geralmente são realizadas fora de [!DNL Experience Manager]. Eles podem carregar essas pastas locais grandes para [!DNL Assets] diretamente do aplicativo de desktop. As hierarquias de pastas são preservadas e todas as subpastas aninhadas e os ativos incluídos são carregados. Os ativos carregados também ficam disponíveis imediatamente para outros usuários do mesmo servidor para consumo. Os Assets são carregados em segundo plano, portanto, a operação não é vinculada a uma sessão do navegador da Web.

![Carregar várias pastas locais em massa da área de trabalho para o [!DNL Experience Manager]](assets/upload_local_folders_da2.png "Carregar várias pastas locais em massa da área de trabalho para a Experience Manager")

Após o carregamento, se as alterações esperadas não forem refletidas no aplicativo, clique no ícone de atualização ![Ícone de atualização](assets/do-not-localize/refresh.png).

>[!NOTE]
>
>Não use a funcionalidade de carregamento para migrar ativos em duas implantações do [!DNL Experience Manager]. Em vez disso, consulte o [guia de migração](https://experienceleague.adobe.com/en/docs/experience-manager-65/content/assets/administer/assets-migration-guide).

## Próximas etapas {#next-steps}

* [Assista a um vídeo para começar a usar o Adobe Experience Manager Desktop App](https://experienceleague.adobe.com/en/docs/experience-manager-learn/assets/creative-workflows/aem-desktop-app)

* Forneça feedback sobre a documentação usando a [!UICONTROL Edit this page] ![edite a página](assets/do-not-localize/edit-page.png) ou [!UICONTROL Log an issue] ![crie um problema do GitHub](assets/do-not-localize/github-issue.png) disponível na barra lateral direita

* Entre em contato com o [Atendimento ao cliente](https://experienceleague.adobe.com/pt-br?support-solution=General#support)

>[!MORELIKETHIS]
>
>* [Baixar ativos](/help/using/download-assets.md)
>* [Entender a interface de usuário](/help/using/user-interface.md)
>* [Pesquisar](/help/using/search.md)
