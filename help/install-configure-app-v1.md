---
title: Instalar e configurar o aplicativo de desktop v1.10
description: Instale e configure os servidores [!DNL Experience Manager] desktop app version 1.10 to work with [!DNL Assets] e mapeie os ativos para montar como uma unidade no seu desktop.
translation-type: tm+mt
source-git-commit: cc4ce762ad1d7f4c5a54ab6bac9d1a872e3d18c9
workflow-type: tm+mt
source-wordcount: '901'
ht-degree: 0%

---


# Instalar e configurar [!DNL Experience Manager] aplicativo desktop v1.10 {#install-and-configure-aem-desktop-app}

Usando o [!DNL Experience Manager] aplicativo de desktop, os ativos em [!DNL Experience Manager] são facilmente acessíveis em seu desktop local e podem ser usados em qualquer aplicativo de desktop. Os ativos podem ser facilmente revelados no Mac Finder ou no Windows Explorer, abertos em aplicativos de desktop e alterados localmente - as alterações são salvas em [!DNL Experience Manager] quando você carrega e uma nova versão é criada no repositório.

Essa integração permite que várias funções na organização gerenciem os ativos centralmente no Assets e os acessem no Creative Cloud e em outros aplicativos, além de facilitar o cumprimento dos vários padrões, inclusive a marca.

Para usar [!DNL Experience Manager] aplicativo de desktop,

* Certifique-se de que a versão do servidor [!DNL Experience Manager] seja suportada pelo [!DNL Experience Manager] aplicativo de desktop. Consulte a matriz de compatibilidade [a1/>.](release-notes-of-v1.md#compatibilitymatrix)

* Baixe e instale o aplicativo.

* Teste a conexão usando alguns ativos. Consulte [Acessar e abrir ativos na área de trabalho](use-app-v1.md#openondesktop).

## Requisitos do sistema, pré-requisitos e links de download {#system-requirements-prerequisites-and-download-links}

Para obter informações detalhadas, consulte as [[!DNL Experience Manager] notas de versão do aplicativo para desktop](release-notes-of-v1.md).

## Instale e conecte o aplicativo ao servidor [!DNL Experience Manager] {#install-and-connect-aem-desktop-app-to-aem-server}

Para obter detalhes, consulte [Instalar e conectar [!DNL Experience Manager] desktop app to [!DNL Experience Manager] servidor](use-app-v1.md#installandconnect).

>[!NOTE]
>
>Apenas uma instância do aplicativo de desktop [!DNL Experience Manager] pode ser instalada e estar ativa de cada vez.

## Manuseio de arquivos {#file-handling}

Ao alterar um arquivo de um local de compartilhamento de rede montado pelo aplicativo de desktop, os arquivos são salvos nesse local em duas fases. Na primeira fase, um arquivo é salvo localmente. Um usuário pode salvar o arquivo e continuar trabalhando nele, sem esperar a conclusão da transferência.

Na segunda fase, o aplicativo desktop carrega o arquivo atualizado no servidor [!DNL Experience Manager] após um atraso predefinido (por exemplo, 30s). Esta operação ocorre em segundo plano. Use a opção Status do ativo de Visualização para visualização do status da operação de upload.

1. Carregar um ativo para os Ativos.

1. Clique no ícone [!DNL Experience Manager] do aplicativo para desktop na barra de ferramentas.

1. No menu, selecione a opção Status do ativo de Visualização.

1. Na caixa de diálogo, reveja o status da operação de upload.

>[!NOTE]
>
>[!DNL Experience Manager] o aplicativo desktop pode lidar com ativos de até 40 GB.

## Conectar-se a uma instância [!DNL Experience Manager] atrás de um dispatcher {#connect-to-an-aem-instance-behind-a-dispatcher}

Os métodos de cópia e movimentação na API Ativos exigem que os seguintes cabeçalhos adicionais sejam passados para [!DNL Experience Manager]:

* Destino X
* Profundidade X
* X-Overwrite

[!DNL Experience Manager] a área de trabalho se conecta ao  [!DNL Experience Manager] uso de um URL que inclui a porta padrão. Portanto, a configuração `virtualhosts` na configuração do dispatcher deve incluir o número da porta padrão. Para obter mais informações sobre a configuração `virtualhosts`, consulte [identificar hosts virtuais](https://experienceleague.adobe.com/docs/experience-manager-dispatcher/using/configuring/dispatcher-configuration.html#identifying-virtual-hosts-virtualhosts).

Para obter informações adicionais sobre como configurar o dispatcher para passar por esses cabeçalhos adicionais, consulte [Especificação dos cabeçalhos HTTP](https://experienceleague.adobe.com/docs/experience-manager-dispatcher/using/configuring/dispatcher-configuration.html#specifying-the-http-headers-to-pass-through-clientheaders).

### Suporte a proxy {#proxy-support}

[!DNL Experience Manager] o aplicativo desktop usa o proxy predefinido do sistema para se conectar à Internet por HTTPS. O aplicativo só pode se conectar usando um proxy de rede que não exija autenticação extra.

Se você configurar ou modificar as configurações do servidor proxy para Windows (Opções da Internet > Configurações de LAN), reinicie o [!DNL Experience Manager] aplicativo de desktop para que as alterações tenham efeito.

>[!NOTE]
>
>A configuração de proxy só é aplicada quando você start o aplicativo de desktop. Feche e reinicie o aplicativo para que as alterações entrem em vigor.

Se o proxy exigir autenticação, a equipe de TI poderá permitir que o URL dos ativos Experience Manager nas configurações do servidor proxy permita que o tráfego do aplicativo passe.

## Personalizar a caixa de diálogo Informações do ativo {#customize-the-asset-info-dialog}

Você pode personalizar a caixa de diálogo Informações do ativo sobrepondo um ou ambos os componentes:

* A página da interface do usuário do Granite em `/libs/dam/gui/content/assets/moreinfo`.

* O componente HTL `/css/javascript` em `/libs/dam/gui/components/admin/moreinfo`.

O componente sobreposto depende da natureza da personalização. Para alterar quais componentes são exibidos como parte da caixa de diálogo Informações do ativo, sobreponha a página da interface do usuário do Granite. Para alterar o conteúdo HTML, CSS ou JavaScript da caixa de diálogo, sobreponha o componente HTL.

## Gerenciar cache {#manage-cache}

No Windows, o cache está em `%LOCALAPPDATA%\Adobe\AssetsCompanion\Cache\`, onde é uma versão codificada do host [!DNL Experience Manager] configurado no aplicativo de desktop. Por exemplo, `http://localhost:4502` aparece como `http%3A%2F%2Flocalhost%3A4502%2F`.

No Mac OS X, um diretório semelhante fica em `~/Library/Group Containers/group.com.adobe.aem.desktop/cache`.

### Opção no aplicativo para gerenciar o cache {#in-app-option-to-manage-cache}

Você pode controlar a quantidade de espaço em disco disponível para fins de armazenamento em cache local. Os artefatos do servidor Assets são armazenados em cache localmente para proporcionar uma experiência mais suave. Você pode alterar os padrões para atender às suas necessidades. Além disso, você pode limpar o cache para obter todos os ativos novamente. Para definir as opções desejadas, clique no ícone do aplicativo e clique em **[!UICONTROL Advanced]** > **[!UICONTROL Manage Cache]**. ****

>[!NOTE]
>
>Quando você limpa o cache, ele preserva suas alterações não salvas. Todos os ativos não verificados no servidor [!DNL Experience Manager] são retidos e não excluídos.

### Alterar local do cache no Windows {#change-location-of-cache-on-windows}

O local padrão do cache para o aplicativo de desktop [!DNL Experience Manager] é o seguinte:

* No Windows, `%LocalAppData%\Adobe\AssetsCompanion\Cache\EncodedAEMEndpoint`.

* No Mac, `~/Library/Group/Containers/group.com.adobe.aem.desktop/cache/EncodedAEMEndpoint`.

`EncodedAEMEndpoint` é o URL de  [!DNL Experience Manager] ponto de extremidade configurado do aplicativo. O valor é uma versão codificada do URL de definição de metas do servidor [!DNL Experience Manager]. Por exemplo, se o aplicativo estiver direcionando `http://localhost:4502`, o nome do diretório será `http%3A%2F%2Flocalhost%3A4502`. O caminho do Windows para o diretório de cache neste exemplo é `%LocalAppData%\Adobe\AssetsCompanion\Cache\http%3A%2F%2Flocalhost%3A4502`.

Para apontar o aplicativo para uma pasta diferente ou uma unidade diferente, edite o arquivo de configuração do aplicativo.

1. Navegue até o diretório de instalação do aplicativo. O local padrão no Windows é `C:\Program Files (x86)\Adobe\Adobe Experience Manager Desktop`.

1. Edite o arquivo Adobe Experience Manager Desktop.exe.config com um editor de texto.

   São necessários privilégios de administrador para salvar as alterações neste arquivo.

1. Procure a string &quot;ProxyCacheRoot&quot;. Você verá que seu valor está definido para o local do cache `%LocalAppData%\Adobe\AssetsCompanion\Cache`. Basta alterar esse valor para qualquer caminho válido.

   >[!NOTE]
   >
   >O aplicativo cria automaticamente um subdiretório *&lt;Encoded AEM Endpoint>*. Este comportamento não é configurável.

>[!MORELIKETHIS]
* [Introdução  [!DNL Experience Manager] ao aplicativo](https://experienceleague.adobe.com/docs/experience-manager-learn/assets/creative-workflows/aem-desktop-app.html) para desktop.
* [Use  [!DNL Experience Manager] o aplicativo](use-app-v1.md) para desktop.
* [ [!DNL Experience Manager] Solução de problemas do aplicativo](troubleshoot-app-v1.md) para desktop.

