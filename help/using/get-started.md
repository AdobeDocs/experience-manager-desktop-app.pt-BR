---
title: 'Introdução ao aplicativo de desktop [!DNL Experience Manager] '
description: Saiba como o aplicativo de desktop  [!DNL Experience Manager]  aprimora a criação e a publicação de conteúdo com fluxos de trabalho simplificados e recursos de produtividade.
feature: Desktop App,Asset Management
exl-id: 6cf29b6a-74e6-4860-a25b-d3e91abbaa9d
source-git-commit: 2bf5ee7454846c288cc1c976d8f69c6bfed8eabf
workflow-type: tm+mt
source-wordcount: '1213'
ht-degree: 0%

---

# Introdução ao uso do [!DNL Adobe Experience Manager] Desktop App {#getting-started-desktop-app}

Use o aplicativo de desktop do [!DNL Adobe Experience Manager] para acessar ativos digitais armazenados em um repositório DAM do [!DNL Adobe Experience Manager] na área de trabalho local. Em seguida, você pode usar esses ativos em qualquer aplicativo de desktop. Você pode abrir e editar os ativos localmente em aplicativos de desktop. Depois de fazer alterações, carregue-as de volta para [!DNL Experience Manager] com controle de versão para compartilhar atualizações com outros usuários. Você também pode carregar novos arquivos e hierarquias de pastas para o [!DNL Experience Manager], criar pastas e excluir ativos ou pastas do DAM [!DNL Experience Manager].

A integração permite que várias funções na organização gerenciem os ativos de forma central no [!DNL Experience Manager Assets] e acessem os ativos no desktop local nos aplicativos nativos no Windows ou macOS.

Quando você abrir o aplicativo depois de fazer logoff ou pela primeira vez, forneça a URL do servidor [!DNL Experience Manager] no formato `https://[aem-server-url]:[port]/`. Em seguida, selecione a opção [!UICONTROL Connect]. Forneça credenciais para conectar o aplicativo ao servidor.

>[!VIDEO](https://video.tv.adobe.com/v/28868?quality=12&learn=on){transcript=true}

As principais tarefas que você executa usando o aplicativo de desktop [!DNL Adobe Experience Manager] são:

![Fluxos de trabalho e tarefas que você pode realizar usando o aplicativo de desktop [!DNL Experience Manager]](assets/aem_desktop_app_usecases_v2.png)

## Como o aplicativo de desktop funciona {#how-app-works2}

Antes de começar a usar o aplicativo, [entenda como o aplicativo funciona](release-notes.md#how-app-works). Além disso, familiarize-se com os seguintes termos:

* **[!UICONTROL Desktop Actions]**: na interface da Web do Assets, de dentro de um navegador, você pode explorar os locais dos ativos ou fazer check-out e abrir o ativo para edição no aplicativo de desktop nativo. Essas ações estão disponíveis na interface da Web e usam a funcionalidade do aplicativo de desktop.

* O status do arquivo é **[!UICONTROL Cloud Only]**: esses ativos não são baixados no computador local e estão disponíveis somente no servidor [!DNL Experience Manager].

* O status do arquivo é **[!UICONTROL Available locally]**: os ativos são baixados e disponibilizados no computador local como estão. Os ativos não são alterados.

* O status do arquivo é **[!UICONTROL Edited locally]**: esses ativos são modificados localmente e as alterações permanecem no arquivo carregado para o servidor [!DNL Experience Manager]. Após o carregamento, o status muda para [!UICONTROL Available locally]. Consulte [editar ativos](upload-assets.md#edit-assets-upload-updated-assets).

* O status do arquivo é **[!UICONTROL Editing conflict]**: se você e outras pessoas editarem um ativo simultaneamente, o aplicativo indicará que um conflito de edição ocorreu. O aplicativo também fornece opções para reter ou descartar suas alterações. Consulte [como evitar conflitos de edição](assets-management-tasks.md#adv-workflow-collaborate-avoid-conflicts).

* O status do arquivo é **[!UICONTROL Modified remotely]**: o aplicativo indica se um ativo que você baixou foi alterado no servidor [!DNL Experience Manager]. O aplicativo também oferece a opção de baixar a versão mais recente e atualizar a cópia local. Consulte [como evitar conflitos de edição](assets-management-tasks.md#adv-workflow-collaborate-avoid-conflicts).

* **[!UICONTROL Check-out]**: Se você está editando um arquivo ou pretende editar um arquivo, alterne o status para check-out. Ele adiciona um ícone de bloqueio no ativo no aplicativo e na interface da Web do [!DNL Experience Manager]. O ícone de bloqueio indica a outros usuários que eles devem evitar a edição simultânea do mesmo ativo, pois isso resulta em um conflito de edição.

* **[!UICONTROL Check-in]**: marque o ativo como seguro para outros usuários editarem sem causar um conflito de edição. Ao fazer upload das alterações, o ícone de bloqueio é removido automaticamente. Alterar o status de check-in também remove o ícone de bloqueio, embora a Adobe recomende que você evite fazer check-in manualmente sem fazer upload das alterações. Se você descartar as alterações, alterne o check-in manualmente.

* Ação **[!UICONTROL Open]**: basta abrir o ativo para visualizá-lo no aplicativo nativo. A Adobe recomenda que você evite editar o ativo usando esta ação. O motivo é porque ele não faz check-out do ativo. Enquanto isso, outros usuários podem fazer edições que geram conflitos de edição.

* Ação **[!UICONTROL Edit]**: use a ação para modificar a imagem. Clicar em [!UICONTROL Edit] faz check-out do ativo e adiciona um ícone de bloqueio no ativo. Depois de clicar em Editar, se você não quiser editar o ativo, clique em [!UICONTROL Toggle check-in]. Para excluir, renomear ou mover ativos na hierarquia de pastas do DAM [!DNL Experience Manager], use as ações da interface da Web [!DNL Experience Manager] e não a ação de edição.

* Ação do **[!UICONTROL Download]**: baixe o ativo no computador local. É possível baixar os ativos agora e editar depois; trabalhar offline e fazer upload das alterações posteriormente. Os Assets são baixados em uma pasta de cache no sistema de arquivos.

* Ação **[!UICONTROL Reveal File]** ou **[!UICONTROL Reveal Folder]**: enquanto os ativos são baixados para uma pasta de cache local, o aplicativo imita uma unidade de rede local. Ele fornece um caminho local para cada ativo. Para conhecer esse caminho, use a opção de revelação apropriada no aplicativo. É necessária uma ação de revelar para colocar ativos no aplicativo do Creative Cloud. Consulte [colocar ativos](search.md#place-assets-in-native-documents).

* Ação **[!UICONTROL Open In Web]**: para exibir o ativo na interface da Web [!DNL Experience Manager], abra-o na Web. Você pode iniciar mais fluxos de trabalho a partir da interface [!DNL Experience Manager], como atualizar metadados ou a descoberta de ativos.

* Ação **[!UICONTROL Delete]**: excluir o ativo do repositório DAM [!DNL Experience Manager]. A ação exclui a cópia original do ativo no servidor do Experience Manager. Se quiser descartar apenas as modificações feitas no ativo local, consulte [descartar alterações](upload-assets.md#edit-assets-upload-updated-assets).

* **[!UICONTROL Upload Changes]**: o aplicativo de desktop carrega o ativo atualizado apenas quando você carrega explicitamente para o servidor [!DNL Experience Manager]. Ao salvar suas edições, as alterações são salvas somente em seu computador local. Ao fazer upload, o ativo é automaticamente registrado e o ícone de bloqueio é removido. Consulte [editar ativos](upload-assets.md#edit-assets-upload-updated-assets).

## Habilitar ações da área de trabalho na interface da Web do [!DNL Experience Manager] {#desktopactions-v2}

A partir da interface de usuário do [!DNL Assets] em um navegador, você pode explorar os locais dos ativos ou fazer check-out e abrir o ativo para edição no aplicativo de desktop. Estas opções são chamadas de [!UICONTROL Desktop Actions] e não estão habilitadas por padrão. Para ativá-lo, siga estas etapas.

1. No console [!DNL Assets], clique no ícone **[!UICONTROL User]** na barra de ferramentas.
1. Clique em **[!UICONTROL My Preferences]** para exibir a caixa de diálogo **[!UICONTROL Preferences]**.

1. Na caixa de diálogo [!UICONTROL User Preferences], selecione **[!UICONTROL Show Desktop Actions For Assets]** e clique em **[!UICONTROL Accept]**.

   ![Selecione Mostrar Ações da Área de Trabalho para o Assets para habilitar ações da área de trabalho](assets/enable_desktop_actions1.png)

## Iniciar na interface da Web do [!DNL Assets] {#adv-workflow-start-from-aem-ui}

Se necessário, inicie o workflow na interface da Web do Assets. O aplicativo de desktop integra-se com o [!DNL Experience Manager] para assumir o controle quando solicitado usando as Ações de Desktop.

Um caso especial de iniciar um fluxo de trabalho a partir da interface da Web é a descoberta de ativos. A barra Omnisearch na interface do usuário do Assets oferece uma experiência de pesquisa avançada. Talvez você queira primeiro localizar um ativo desejado na Web e, em seguida, iniciar o fluxo de trabalho no aplicativo, usando [!UICONTROL Desktop Actions]. Alguns casos de amostra incluem filtrar resultados de pesquisa usando facetas, localizar um ativo específico licenciado da Adobe Stock ou uma personalização implementada pela organização que permite uma melhor descoberta na interface da Web.

A funcionalidade do aplicativo de desktop é usada quando você tenta as seguintes ações na interface da Web do Assets:

* O [!UICONTROL Desktop Actions] que permite [!UICONTROL Open], [!UICONTROL Edit] e [!UICONTROL Reveal]
* [!UICONTROL Upload folder]
* [!UICONTROL Check-out] ou [!UICONTROL check-in]

Por exemplo, as ações na interface da Web disponíveis para um ativo com check-out no aplicativo são [!UICONTROL Open], [!UICONTROL Reveal] e [!UICONTROL Check in].

![Ações da Área de Trabalho na [!DNL Experience Manager] interface da Web](assets/assets_web_actions_da2.png "Ações da Área de Trabalho na interface da Web do Experience Manager")

>[!NOTE]
>
>O navegador pode solicitar que você autorize a inicialização da Área de Trabalho [!DNL Adobe Experience Manager]. Para realizar transferências ininterruptas do navegador para o aplicativo todas as vezes, marque a caixa de seleção apropriada para permitir que o aplicativo assuma o controle.

Não é possível localizar as informações ou o fluxo de trabalho a seguir usando a interface da Web. Use o aplicativo de desktop, pois a interface da Web não rastreia alterações locais e não tem conhecimento do seguinte:

* Os arquivos são editados localmente.
* Arquivos que têm um conflito de edição e uma maneira de resolvê-lo.
* Carregar alterações locais em [!DNL Experience Manager].
* Vários status dos arquivos disponíveis localmente.

Ao contrário, você pode abrir o ativo na interface da Web a partir do aplicativo de desktop usando a ação **[!UICONTROL Open In Web]**.

## Próximas etapas {#next-steps}

* [Assista a um vídeo para começar a usar o Adobe Experience Manager Desktop App](https://experienceleague.adobe.com/en/docs/experience-manager-learn/assets/creative-workflows/aem-desktop-app)

* Forneça feedback sobre a documentação usando a [!UICONTROL Edit this page] ![edite a página](assets/do-not-localize/edit-page.png) ou [!UICONTROL Log an issue] ![crie um problema do GitHub](assets/do-not-localize/github-issue.png) disponível na barra lateral direita

* Entre em contato com o [Atendimento ao cliente](https://experienceleague.adobe.com/pt-br?support-solution=General#support)

>[!MORELIKETHIS]
>
>* [Entender a interface de usuário](/help/using/user-interface.md)
>* [Notas de versão e problemas conhecidos](/help/using/release-notes.md)
>* [Instalar ou atualizar o aplicativo de desktop](/help/using/install-upgrade.md)
