---
title: Instalar e configurar o aplicativo de desktop v1.10
description: Instale e configure o  [!DNL Experience Manager] aplicativo de desktop versão 1.10 para funcionar com  [!DNL Assets] servidores e mapeie os ativos a serem montados como uma unidade no desktop.
exl-id: 7f3bdfb1-d345-4e48-b020-6e06531f46f2
source-git-commit: 1c7437786a50eeafa884ce92b745f3438b2d2b88
workflow-type: tm+mt
source-wordcount: '884'
ht-degree: 0%

---

# Instalar e configurar o aplicativo de desktop do [!DNL Experience Manager] v1.10 {#install-and-configure-aem-desktop-app}

Usando o aplicativo de desktop [!DNL Experience Manager], os ativos do [!DNL Experience Manager] são facilmente acessíveis no desktop local e podem ser usados em qualquer aplicativo de desktop. O Assets pode ser revelado no Mac Finder ou no Windows Explorer, editado em aplicativos de desktop, e as alterações são salvas novamente em [!DNL Experience Manager], criando uma nova versão após o carregamento.

Essa integração permite que diferentes funções gerenciem ativos de forma central na organização na Assets, acessem-nos no Creative Cloud e em outros aplicativos e cumpram facilmente com vários padrões, inclusive de marca.

Para usar o aplicativo de desktop [!DNL Experience Manager],

* Verifique se a versão do servidor [!DNL Experience Manager] é compatível com o aplicativo de desktop [!DNL Experience Manager]. Consulte a [matriz de compatibilidade](release-notes-of-v1.md#compatibilitymatrix).

* Baixe e instale o aplicativo.

* Teste a conexão usando alguns ativos. Consulte [Acessar e abrir ativos na área de trabalho](use-app-v1.md#openondesktop).

## Requisitos do sistema, pré-requisitos e links de download {#system-requirements-prerequisites-and-download-links}

Para obter informações detalhadas, consulte as [[!DNL Experience Manager] notas de versão do aplicativo de desktop](release-notes-of-v1.md).

## Instalar e conectar o aplicativo ao servidor [!DNL Experience Manager] {#install-and-connect-aem-desktop-app-to-aem-server}

Para obter detalhes, consulte [Instalar e conectar [!DNL Experience Manager] aplicativo de desktop ao [!DNL Experience Manager] servidor](use-app-v1.md#installandconnect).

>[!NOTE]
>
>Somente uma instância do aplicativo de desktop [!DNL Experience Manager] pode ser instalada e estar ativa por vez.

## Manuseio de arquivos {#file-handling}

Ao alterar um arquivo de um local de compartilhamento de rede montado pelo aplicativo de desktop, os arquivos são salvos nesse local em duas fases. Na primeira fase, um arquivo é salvo localmente. Um usuário pode salvar o arquivo e continuar trabalhando nele, sem esperar a conclusão da transferência.

Na segunda fase, o aplicativo de desktop carrega o arquivo atualizado no servidor [!DNL Experience Manager] após um atraso predefinido (por exemplo, 30s). Esta operação ocorre em segundo plano. Use a opção Exibir status do ativo para exibir o status da operação de upload.

1. Faça upload de um ativo para o Assets.

1. Clique no ícone do aplicativo de desktop [!DNL Experience Manager], na barra de ferramentas.

1. No menu, selecione a opção Exibir status do ativo.

1. Na caixa de diálogo do, revise o status da operação de upload.

>[!NOTE]
>
>O aplicativo de desktop [!DNL Experience Manager] pode manipular ativos de até 40 GB.

## Conectar-se a uma instância do [!DNL Experience Manager] por trás de um Dispatcher {#connect-to-an-aem-instance-behind-a-dispatcher}

Os métodos de copiar e mover na API do Assets exigem que os seguintes cabeçalhos adicionais sejam passados para [!DNL Experience Manager]:

* Destino X
* Profundidade X
* X-Sobrescrever

A área de trabalho do [!DNL Experience Manager] se conecta ao [!DNL Experience Manager] usando uma URL que inclui a porta padrão. Portanto, a configuração `virtualhosts` na configuração do Dispatcher deve incluir o número de porta padrão. Para obter mais informações sobre a configuração de `virtualhosts`, consulte [identificar hosts virtuais](https://experienceleague.adobe.com/en/docs/experience-manager-dispatcher/using/configuring/dispatcher-configuration#identifying-virtual-hosts-virtualhosts).

Para obter informações adicionais sobre como configurar o Dispatcher para passar por esses cabeçalhos adicionais, consulte [Especificação dos Cabeçalhos HTTP](https://experienceleague.adobe.com/en/docs/experience-manager-dispatcher/using/configuring/dispatcher-configuration#specifying-the-http-headers-to-pass-through-clientheaders).

### Suporte de proxy {#proxy-support}

O aplicativo de desktop [!DNL Experience Manager] usa o proxy predefinido do sistema para se conectar à Internet via HTTPS. O aplicativo só pode se conectar usando um proxy de rede que não exija autenticação extra.

Se você definir ou modificar as configurações de servidor proxy para o Windows (Opções da Internet > Configurações da LAN), reinicie o aplicativo de desktop [!DNL Experience Manager] para que as alterações entrem em vigor.

>[!NOTE]
>
>A configuração de proxy é aplicada somente quando você inicia o aplicativo de desktop. Feche e reinicie o aplicativo para que as alterações entrem em vigor.

Se o proxy exigir autenticação, a equipe de TI poderá permitir que o URL do Experience Manager Assets nas configurações do servidor proxy permita a passagem do tráfego do aplicativo.

## Personalizar a caixa de diálogo Informações do ativo {#customize-the-asset-info-dialog}

Você pode personalizar a caixa de diálogo Informações do ativo sobrepondo um ou ambos os componentes:

* A página da interface do usuário do Granite em `/libs/dam/gui/content/assets/moreinfo`.

* O componente HTL `/css/javascript` em `/libs/dam/gui/components/admin/moreinfo`.

O componente sobreposto depende da natureza da personalização. Para alterar quais componentes são exibidos como parte da caixa de diálogo Informações do ativo, sobreponha a página da interface do usuário do Granite. Para alterar o conteúdo HTML, CSS ou JavaScript da caixa de diálogo, sobreponha o componente HTL.

## Gerenciar cache {#manage-cache}

No Windows, o cache está em `%LOCALAPPDATA%\Adobe\AssetsCompanion\Cache\`, onde é uma versão codificada do host [!DNL Experience Manager] configurado no aplicativo de desktop. Por exemplo, `http://localhost:4502` aparece como `http%3A%2F%2Flocalhost%3A4502%2F`.

No macOS X, um diretório semelhante está em `~/Library/Group Containers/group.com.adobe.aem.desktop/cache`.

### Opção no aplicativo para gerenciar o cache {#in-app-option-to-manage-cache}

Você pode controlar a quantidade de espaço em disco disponibilizada para fins de armazenamento em cache local. Os artefatos do servidor do Assets são armazenados em cache localmente para obter uma experiência mais suave. Você pode alterar os padrões para atender às suas necessidades. Além disso, é possível limpar o cache para buscar todos os ativos novamente. Para definir as opções desejadas, clique no ícone do aplicativo e clique em **[!UICONTROL Advanced]** > **[!UICONTROL Manage Cache]**. **&#x200B;**

>[!NOTE]
>
>Quando você limpa o cache, ele preserva as alterações não salvas. Todos os ativos não verificados no servidor [!DNL Experience Manager] são retidos e não excluídos.

### Alterar local do cache no Windows {#change-location-of-cache-on-windows}

O local padrão do cache para o aplicativo de desktop [!DNL Experience Manager] é o seguinte:

* No Windows, `%LocalAppData%\Adobe\AssetsCompanion\Cache\EncodedAEMEndpoint`.

* No Mac, `~/Library/Group/Containers/group.com.adobe.aem.desktop/cache/EncodedAEMEndpoint`.

O `EncodedAEMEndpoint` é a URL do ponto de extremidade [!DNL Experience Manager] configurada do aplicativo. O valor é uma versão codificada da URL de direcionamento do servidor [!DNL Experience Manager]. Por exemplo, se o aplicativo for direcionado a `http://localhost:4502`, o nome do diretório será `http%3A%2F%2Flocalhost%3A4502`. O caminho do Windows para o diretório de cache neste exemplo é `%LocalAppData%\Adobe\AssetsCompanion\Cache\http%3A%2F%2Flocalhost%3A4502`.

Para direcionar o aplicativo para uma pasta ou unidade diferente, edite o arquivo de configuração do aplicativo.

1. Navegue até o diretório de instalação do aplicativo. O local padrão no Windows é `C:\Program Files (x86)\Adobe\Adobe Experience Manager Desktop`.

1. Edite o arquivo `Adobe Experience Manager Desktop.exe.config` com um editor de texto.

   São necessários privilégios de administrador para salvar as alterações feitas neste arquivo.

1. Procure a sequência &quot;ProxyCacheRoot&quot;. Você pode ver que o valor está definido para o local de cache `%LocalAppData%\Adobe\AssetsCompanion\Cache`. Basta alterar esse valor para qualquer caminho válido.

   >[!NOTE]
   >
   >O aplicativo cria automaticamente um subdiretório *&lt;Endpoint AEM Codificado>*. Esse comportamento não é configurável.

>[!MORELIKETHIS]
>
>* Assista a uma [Introdução ao [!DNL Experience Manager] aplicativo de desktop](https://experienceleague.adobe.com/en/docs/experience-manager-learn/assets/creative-workflows/aem-desktop-app) (5 minutos, 43 segundos).
>* [Usar [!DNL Experience Manager] aplicativo de desktop](use-app-v1.md).
>* [Solução de problemas [!DNL Experience Manager] aplicativo de desktop](troubleshoot-app-v1.md).
