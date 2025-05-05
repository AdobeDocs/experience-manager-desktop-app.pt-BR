---
title: Use o  [!DNL Experience Manager] aplicativo de desktop versão 1.10.
description: Saiba como usar o aplicativo de desktop do Adobe Experience Manager versão 1.10 e otimizar seu trabalho com ativos no desktop.
feature: Desktop App,Asset Management
exl-id: 2fdc1c8d-b822-4cca-ad06-bd875a00aa6d
source-git-commit: 5676e7ece8bb43f051dae72d17e15ab1c34caefc
workflow-type: tm+mt
source-wordcount: '2329'
ht-degree: 0%

---

# Usar o aplicativo de desktop v1.10 do [!DNL Experience Manager] {#use-aem-desktop-app-v1x}

Usando o Aplicativo, os ativos no [!DNL Experience Manager] são facilmente acessíveis na área de trabalho local e podem ser usados em qualquer aplicativo de área de trabalho. O Assets pode ser facilmente revelado no Mac Finder ou no Windows Explorer, aberto em aplicativos de desktop e alterado localmente - as alterações são salvas novamente no [!DNL Experience Manager] com uma nova versão criada no repositório.

Essa integração permite o gerenciamento centralizado de ativos e o acesso por meio do Creative Cloud e de outros aplicativos, garantindo a conformidade com as marcas e outros padrões.

As principais tarefas que você executa usando o aplicativo de desktop [!DNL Experience Manager] v1 incluem:

1. [Conectar-se a um servidor  [!DNL Experience Manager] ](#installandconnect)
1. [Abrir ativos diretamente no aplicativo de desktop](#openondesktop)
1. [Editar e fazer check-out de ativos do aplicativo de desktop](#workonassets)
1. [Fazer upload de ativos e pastas em massa](#bulkupload)

Para os vários itens recomendados, consulte as [práticas recomendadas para usar o aplicativo de desktop](best-practices-for-v1.md). Se você enfrentar problemas ao usar o aplicativo, consulte como [solucionar problemas [!DNL Experience Manager] aplicativo de desktop](troubleshoot-app-v1.md).

>[!NOTE]
>
>O aplicativo de desktop foi introduzido na versão [!DNL Experience Manager] 6.1 e foi chamado de [!DNL Experience Manager Assets Companion App].

## Pontos de contato do aplicativo de desktop [!DNL Experience Manager] no fluxo de trabalho criativo {#aem-desktop-app-touch-points-in-the-creative-workflow}

O aplicativo de desktop do [!DNL Experience Manager], juntamente com o [!DNL Assets], integra-se ao seu fluxo de trabalho criativo e oferece os seguintes pontos de contato.

![[!DNL Experience Manager] pontos de contato do aplicativo de desktop para o fluxo de trabalho criativo](assets/aem_desktopapp_workflow.png)

[!DNL Experience Manager] pontos de contato do aplicativo de desktop para o fluxo de trabalho criativo

## Instalar e conectar o aplicativo ao servidor [!DNL Experience Manager] {#installandconnect}

Antes de começar a criar ou editar os ativos criativos, conecte o aplicativo de desktop ao servidor [!DNL Assets] para baixar e carregar ativos no repositório. Execute as seguintes tarefas:

1. [Instalar o aplicativo](#installapp).
1. [Defina suas preferências](#inapppref) e detalhes de conexão.
1. [Conecte-se a um [!DNL Experience Manager] servidor](#connect) e monte o repositório de ativos como unidade local.
1. [Habilitar ações da área de trabalho](#desktopactions) no servidor [!DNL Experience Manager].

O aplicativo de desktop [!DNL Experience Manager] usa uma conexão HTTPS para se conectar ao servidor [!DNL Experience Manager] e transferir seus ativos de forma robusta e segura.

>[!NOTE]
>
>Para todas ou parte das etapas de instalação e configuração, talvez você precise da ajuda do administrador ou do administrador do sistema do [!DNL Experience Manager].

### Instalar o aplicativo {#installapp}

Verifique se o aplicativo é compatível com a versão do servidor Experience Manager para usar o aplicativo de desktop Experience Manager. Baixe o arquivo de instalação apropriado (binário) para seu sistema operacional (Mac ou Windows) e instale o aplicativo.

A configuração detalhada pode ser necessária, dependendo das preferências da rede e do sistema. Consulte [Instalar e configurar [!DNL Experience Manager] aplicativo de desktop](install-configure-app-v1.md) para obter mais detalhes.

1. Vá para a [[!DNL Experience Manager] página de download do aplicativo de desktop v1.10](/help/using/release-notes-of-v1.md) e baixe o binário apropriado para seu sistema operacional.
1. Inicie o arquivo de instalação baixado e siga as instruções na tela para instalar o aplicativo.

   >[!NOTE]
   >
   >Somente uma instância do aplicativo de desktop [!DNL Experience Manager] pode ser instalada e estar ativa por vez.

### Entender as opções e preferências no aplicativo {#inapppref}

O aplicativo permite que as configurações se conectem e desconectem de [!DNL Experience Manager] servidores, exibam o status dos carregamentos, gerenciem o cache local e assim por diante. As configurações padrão funcionam para um usuário típico do aplicativo. É possível ajustar as configurações para obter mais do aplicativo. E obtenha mais da integração com o servidor [!DNL Experience Manager]. Estas são as várias configurações:

**Explorar Assets** Abra a unidade local na qual o repositório [!DNL Assets] está montado. Em outras palavras, explore os ativos que agora são disponibilizados em seu computador local.

**Exibir status do ativo** Quando ativos alterados são carregados ou novos ativos são adicionados ao repositório [!DNL Assets], o aplicativo carrega os ativos em segundo plano. O upload em segundo plano permite operações tranquilas, sem que seja necessário esperar a conclusão do upload, especialmente para ativos de grande porte. Você pode salvar suas alterações localmente e esquecê-las. O aplicativo leva algum tempo para enviar esses ativos ao servidor, dependendo da largura de banda disponível. Você pode verificar o status do upload, juntamente com algumas informações mais básicas.

**Opções** Clique nas opções na bandeja do aplicativo da área de trabalho para definir que o aplicativo seja iniciado na inicialização, conecte-se ao servidor [!DNL Experience Manager] na inicialização e altere a letra da unidade local para [!DNL Assets] após a montagem.

**Avançado > Gerenciar cache** Você pode controlar a quantidade de espaço em disco disponibilizada para fins de cache local. Os artefatos do servidor [!DNL Assets] são armazenados em cache localmente para proporcionar uma experiência mais suave. Você pode alterar os padrões para atender às suas necessidades. Além disso, é possível limpar o cache para buscar todos os ativos novamente. Quando você limpa o cache, ele preserva as alterações não salvas. Todos os ativos não verificados no servidor [!DNL Experience Manager] são retidos e não excluídos.

### Conectar a um servidor [!DNL Experience Manager] {#connect}

O aplicativo oferece suporte à configuração de proxy no Mac e no Windows. A configuração é lida quando o aplicativo é iniciado. Se você modificar as configurações de proxy, reinicie o aplicativo para que as alterações entrem em vigor.

>[!NOTE]
>
>Se você modificar as configurações de proxy, reinicie o aplicativo para que as alterações entrem em vigor. Caso contrário, o aplicativo continuará a usar o servidor proxy configurado anteriormente.

1. Inicie o aplicativo de desktop [!DNL Experience Manager]. Para mapear sua instância do [!DNL Experience Manager] com o aplicativo, especifique o servidor do [!DNL Experience Manager] no formato `https://[aem-server-url]:[port]`.

   ![Autentique no Mac e forneça a URL do servidor [!DNL Experience Manager]](assets/aem_desktop_app_server_url.png)

1. Na tela de logon, especifique o nome de usuário e a senha da instância. Para especificar uma instância [!DNL Experience Manager] alternativa, selecione a opção **[!UICONTROL Alternate Login URL]**.

   ![Forneça as credenciais de servidor [!DNL Experience Manager] na tela de logon no aplicativo de desktop [!DNL Experience Manager]](assets/login_screen_v1.png)

### Habilitar ações da área de trabalho na interface da Web do [!DNL Experience Manager] {#desktopactions}

Na interface do usuário do Assets, você pode explorar os locais dos ativos ou fazer check-out e abrir o ativo para edição no aplicativo de desktop. Essas opções são chamadas de ações do desktop e não são ativadas por padrão. Siga estas etapas para ativá-lo.

1. Na interface do Assets, clique/toque no ícone Usuário no canto superior direito da barra de ferramentas.
1. Clique em **[!UICONTROL My Preferences]** para exibir a caixa de diálogo **[!UICONTROL Preferences]**.

   ![[!DNL Experience Manager] interface com preferências de usuário](assets/aem_ui_user_preferences.png)

1. Na caixa de diálogo [!UICONTROL User Preferences], selecione **[!UICONTROL Show Desktop Actions For Assets]** e clique em **[!UICONTROL Accept]**.

   ![Marque [!UICONTROL Show Desktop Actions For Assets] para habilitar ações da área de trabalho](assets/enable_desktop_actions.png)

   *Figura: marque [!UICONTROL Show Desktop Actions For Assets] para habilitar as ações da área de trabalho.*

## Acessar e abrir ativos no desktop {#openondesktop}

Quando você clica em **Abrir** para abrir um ativo no computador local, o aplicativo baixa o ativo para seu cache interno. O aplicativo inicia o aplicativo de desktop nativo associado ao tipo de arquivo do ativo baixado.

No Mac, selecione **Abrir** no menu de contexto para abrir um ativo por meio do aplicativo de desktop [!DNL Experience Manager]. No Windows, selecione Abrir na Web no menu de contexto para abrir o ativo. Na janela Status do ativo, clique/toque em ![Ícone Abrir na área de trabalho](assets/do-not-localize/aemassets_icon_openondesktop.png) para abrir o ativo.

Para arquivos Adobe InDesign (INDD), selecione **[!UICONTROL Open]** no menu de contexto. Ao clicar nessa opção, o aplicativo baixa os ativos vinculados para o sistema de arquivos local e abre o arquivo INDD no Adobe InDesign. Esse método garante que os ativos necessários estejam disponíveis localmente ao editar o arquivo INDD.

![Opções do menu de contexto para acessar e abrir ativos usando o [!DNL Experience Manager] aplicativo de desktop](assets/aem_desktopapp_mac_context_menu.png)

*Figura: opções do menu de contexto para acessar e abrir ativos usando o aplicativo de desktop [!DNL Experience Manager].*

>[!NOTE]
>
>O Adobe recomenda que você vá para Opções de Exibição do Localizador no Mac e desative as opções **Mostrar informações do item**, **Mostrar visualização do item** e **Mostrar coluna de visualização** para a pasta [!DNL Assets] montada. Isso melhora o desempenho.

### Opções adicionais na interface [!DNL Experience Manager] {#additional-options-in-aem-assets}

Depois de mapear o repositório do [!DNL Assets] para a unidade local, você pode habilitar ícones adicionais e o recurso Carregamento de Pasta para serem exibidos para os ativos e pastas mapeados.

1. Abra a interface [!DNL Assets] e passe o mouse sobre uma pasta ou um ativo, para exibir as ações da área de trabalho como ações rápidas na exibição de Cartão.

   ![Na interface do Assets, abra o menu de ações rápidas para ver as ações da área de trabalho](assets/desktop_actions_in_card_view.png)

   *Figura: na interface do usuário do Assets, abra o menu de ações rápidas para ver as ações da área de trabalho.*

   Essas ações da área de trabalho também estão disponíveis quando você clica na opção **Ações da Área de Trabalho** da barra de ferramentas depois de selecionar o ativo ou na barra de ferramentas na página do ativo.

1. Para abrir o ativo no aplicativo de desktop associado à extensão de arquivo específica, clique no ícone de ação rápida ![Abrir na área de trabalho **Abrir na área de trabalho](assets/do-not-localize/aemassets_icon_openondesktop.png).**

   Como alternativa, escolha **Abrir** no menu **Ações da Área de Trabalho** da barra de ferramentas.

Para localizar o ativo específico no sistema de arquivos local, clique em **Revelar** ação rápida ![Ícone Revelar](assets/do-not-localize/aemassets_reveal_icon.png). Como alternativa, escolha **Revelar** no menu **Ações da Área de Trabalho** da barra de ferramentas.

## Entender os status do ativo {#understand-the-asset-statuses}

| ![Ícone de aplicativo padrão do Windows](assets/do-not-localize/win_default.png) | O aplicativo está conectado ao servidor e todos os ativos são sincronizados. |
--- |--- |
| ![Ícone do Windows desabilitado](assets/do-not-localize/win_disabled.png) | O aplicativo é iniciado, mas não está conectado ao servidor. Alguns ativos podem ter a sincronização pendente. |
| ![Ícone de sincronização de arquivos do Windows](assets/do-not-localize/win_sync.png) | O Assets está sincronizando. Os arquivos estão sendo carregados ou baixados. Você pode ver os status exatos e pausar as transferências a partir da janela Status do ativo. |
| ![Ícone de reconexão do Windows](assets/do-not-localize/win_refresh.png) | O aplicativo está tentando se reconectar. Possivelmente, os problemas de rede estão fazendo com que ele se desconecte. |

## Trabalhe seus ativos {#workonassets}

### Confira os ativos da interface da Web do [!DNL Experience Manager] {#check-out-assets-from-the-aem-web-interface}

[!DNL Experience Manager Assets] permite que você faça check-out dos ativos para edição e check-in novamente depois que você concluir as alterações. Depois de fazer check-out de um ativo, somente você pode editar, anotar, publicar, mover ou excluir o ativo. Fazer o check-out de um ativo bloqueia o ativo e impede que outros usuários executem qualquer uma dessas operações. Para fazer check-out/check-in de ativos, é necessário ter acesso de gravação a eles.

Há duas maneiras de fazer check-out dos ativos da interface da Web do [!DNL Experience Manager]. Para obter informações detalhadas sobre o primeiro método, consulte os [arquivos de check-in e check-out da interface do Assets](https://experienceleague.adobe.com/pt-br/docs/experience-manager-65/content/assets/managing/check-out-and-submit-assets). Siga estas etapas para os segundos métodos para fazer check-out e abrir o ativo quando o aplicativo de desktop [!DNL Experience Manager] estiver instalado.

1. Abra a interface [!DNL Assets] e passe o mouse sobre uma pasta ou um ativo, para exibir as ações da área de trabalho como ações rápidas na exibição de Cartão.

   ![Opção Propriedades na Exibição de Cartão](assets/desktop_actions_in_card_view.png)

   Essas ações da área de trabalho também estão disponíveis quando você clica/toque no ícone Ações da área de trabalho na barra de ferramentas após selecionar o ativo ou na barra de ferramentas na página Ativo.

1. Para abrir o ativo, clique/toque na ação rápida Abrir na área de trabalho ![Ícone Abrir na Área de Trabalho](assets/do-not-localize/aemassets_icon_openondesktop.png).

   Como alternativa, escolha Abrir no menu Ações da Área de Trabalho na barra de ferramentas.

   >[!NOTE]
   >
   >Ao editar um arquivo aberto, mas com check-out desfeito, outros usuários não sabem que você está atualizando o ativo.

1. Para abrir um ativo para edição em um aplicativo do Adobe Creative Cloud, clique em ![ícone Editar Área de Trabalho](assets/do-not-localize/aemassets_icon_editdesktop.png). Essa opção também faz check-out do ativo para edição. Depois que você terminar de editar, faça check-in do ativo para atualizar as alterações em [!DNL Assets].

   Como alternativa, escolha Editar no menu Ações da Área de Trabalho, na barra de ferramentas.

1. Selecione a opção de menu Abrir. Os ativos selecionados são abertos no modo de visualização.
1. Para editar os ativos, selecione a opção Editar. Os ativos são abertos no modo de edição.

### Confira os ativos do Localizador no macOS {#check-out-assets-on-mac}

O aplicativo permite que você faça check-out dos arquivos de ativos para impedir que outros usuários modifiquem os arquivos em que você está trabalhando.

1. No menu de contexto do Mac, selecione a opção Abrir pasta do AEM Assets para abrir o Localizador.

   ![Opções do menu de contexto para acessar e abrir ativos usando o [!DNL Experience Manager] aplicativo de desktop](assets/aem_desktopapp_mac_context_menu.png)

   *Figura: opções do menu de contexto para acessar e abrir ativos usando o aplicativo de desktop [!DNL Experience Manager].*

1. Navegue até o ativo do qual deseja fazer check-out.
1. Clique com o botão direito no ativo e selecione Mais informações do Assets no menu de contexto.
1. Na caixa de diálogo Informações do ativo, clique/toque no ícone Check-out para fazer check-out do ativo. O ícone Check-out é alternado para o ícone de check-in depois de clicar/tocar nele.

   ![Navegar até o ativo para check-out](assets/browse_assets_to_checkout.png)

1. Para fazer o check-in do ativo para que ele fique disponível para outros usuários, clique/toque no ícone de check-in na caixa de diálogo Informações do ativo.

### Fazer check-out de ativos no Windows {#check-out-assets-on-windows}

O aplicativo permite que você faça check-out dos arquivos de ativos para impedir que outros usuários modifiquem os arquivos em que você está trabalhando.

1. No menu Contexto, selecione Explorar Assets para abrir o Explorer.
1. No Explorer, navegue até o local do ativo do qual deseja fazer check-out.
1. Clique com o botão direito do mouse no ativo e selecione Abrir na Web no menu de contexto.
1. Na caixa de diálogo Informações do ativo, clique no ícone Check-out. O ícone Check-out alterna para o ícone Check-in.

   ![Alternância do ícone de check-out](assets/checkout_icon_toggles.png)

1. Revise o ativo no Explorer. O ícone de bloqueio no ativo ![ícone de bloqueio do ativo](assets/do-not-localize/aemassets_icon_lockcheckout.png) indica que você fez check-out do ativo.

   >[!NOTE]
   >
   >O ícone de bloqueio pode aparecer após algum atraso. O aplicativo de desktop [!DNL Experience Manager] armazena em cache os ativos para acesso rápido, portanto, pode levar alguns minutos para atualizar o status bloqueado.

1. Para fazer o check-in do ativo para que ele fique disponível para outros usuários, clique/toque no ícone de check-in na caixa de diálogo **Informações do ativo**.

### Fazer check-in de um ativo usando o Finder ou o Explorer e usando a interface da Web {#check-in-an-asset-using-finder-or-explorer-and-using-web-interface}

Quando terminar de editar os ativos, salve-os no aplicativo de desktop. No menu de contexto, selecione **Mais Informações do Assets** e clique em check-in.

Os ativos são carregados no servidor [!DNL Experience Manager]. Como opção, verifique o status do carregamento selecionando **Exibir status do ativo** no ícone da bandeja do sistema. Como alternativa, você pode fazer check-in de um ativo da interface da Web do [!DNL Experience Manager]. Clique nos ativos com check-out ou selecione-os. Na barra de ferramentas, clique no ícone check-in ![ícone check-in](assets/do-not-localize/aemassets_icon_checkin.png).

Um ativo é carregado para [!DNL Experience Manager] automaticamente depois que qualquer alteração é salva localmente. O check-in disponibiliza o ativo para edição para outros usuários do [!DNL Experience Manager].

### Carregar ativos e pastas em massa no servidor [!DNL Experience Manager] {#bulkupload}

Usando o aplicativo de desktop [!DNL Experience Manager], você pode carregar uma pasta inteira contendo ativos do diretório de arquivos local para [!DNL Assets]. Dessa forma, todos os ativos na pasta são carregados em massa em vez de ter que carregá-los um de cada vez.

1. Na interface do Assets, clique/toque em **Criar** na barra de ferramentas e, no menu, selecione **Pasta de Carregamento**.
1. Navegue até a pasta que deseja fazer upload e selecione-a.
1. Clique/toque em OK. A caixa de diálogo Status do Assets exibe o status do upload.

   ![Ver status do carregamento na janela Status do Ativo](assets/aem_desktopapp_bulkupload_status.png)

   Ver o status do upload na janela Status do ativo

   >[!NOTE]
   >
   >Você pode pausar ou cancelar manualmente o upload clicando/tocando no ícone apropriado.

1. Depois que a pasta for carregada, feche a caixa de diálogo e navegue até a interface do usuário do Assets. A pasta carregada é exibida na interface da Web.

O Adobe não recomenda copiar-colar ou arrastar um número maior de arquivos ou pastas aninhadas, do sistema de arquivos local, para a área de compartilhamento de rede. O aplicativo não pode controlar o processo de carregamento devido a limitações técnicas e o desempenho é insatisfatório.

Como alternativa, selecione arquivos/pastas no Finder ou no Explorer, copie-os, navegue até a pasta de destino na área de compartilhamento de rede e escolha **Colar Assets** no menu de contexto do aplicativo de desktop [!DNL Experience Manager]. Dessa forma, o aplicativo de desktop [!DNL Experience Manager] inicia o upload dos ativos colados de forma semelhante à opção **Pasta de Carregamento**, disponível na interface da Web do [!DNL Experience Manager].

>[!MORELIKETHIS]
>
>* [Solução de problemas [!DNL Experience Manager] aplicativo de desktop](troubleshoot-app-v1.md)
