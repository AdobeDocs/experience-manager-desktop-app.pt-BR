---
title: Instalar e configurar o aplicativo de desktop
description: Instale e configure o aplicativo de desktop  [!DNL Adobe Experience Manager]  para funcionar com  [!DNL Adobe Experience Manager Assets]  servidores e baixe os ativos no sistema de arquivos local.
feature: Desktop App,Release Information
exl-id: 422e51c1-c456-4151-bb43-4b3d29a58187
source-git-commit: 1c7437786a50eeafa884ce92b745f3438b2d2b88
workflow-type: tm+mt
source-wordcount: '1449'
ht-degree: 0%

---

# Instalar o aplicativo de desktop [!DNL Adobe Experience Manager] {#install-app-v2}

Usando o aplicativo de desktop [!DNL Adobe Experience Manager], os ativos do [!DNL Experience Manager] ficam facilmente disponíveis no desktop local e podem ser usados em qualquer aplicativo de desktop nativo. O Assets pode ser visualizado e aberto em aplicativos de desktop. Eles podem ser revelados no Finder ou no Explorer para uso em documentos e editados localmente. As alterações são salvas novamente em [!DNL Experience Manager], criando uma nova versão após o upload.

Essa integração permite que várias funções na organização:

* Gerenciar os ativos de forma centralizada em [!DNL Experience Manager Assets].

* Acesse os ativos em qualquer aplicativo de desktop nativo, incluindo aplicativos de terceiros e no Adobe Creative Cloud. Ao fazer isso, os usuários podem facilmente aderir aos vários padrões, incluindo a marca.

Para usar o aplicativo de desktop [!DNL Experience Manager]:

* Verifique se a sua versão [!DNL Experience Manager] é compatível com o aplicativo de desktop [!DNL Experience Manager].

* Baixe e instale o aplicativo. Consulte [instalar aplicativo de desktop](#install-v2) abaixo.

* Teste a conexão usando alguns ativos. Consulte [como procurar e pesquisar ativos](using.md#browse-search-preview-assets).

## Requisitos do sistema, pré-requisitos e links de download {#tech-specs-v2}

Para obter informações detalhadas, consulte as [[!DNL Experience Manager] notas de versão do aplicativo de desktop](release-notes.md).

## Atualizar de uma versão anterior {#upgrade-from-previous-version}

Se você for um usuário da v1.x do aplicativo de desktop, entenda as diferenças e semelhanças entre a versão anterior e a mais recente do aplicativo. Consulte [novidades no aplicativo de desktop](introduction.md#whats-new-v2) e [como o aplicativo funciona](release-notes.md#how-app-works).

>[!NOTE]
>
>Duas versões de um aplicativo de desktop não podem coexistir em um computador. Antes de instalar uma versão, desinstale a outra versão.

Para atualizar de uma versão anterior do aplicativo, siga estas instruções:

1. Antes de atualizar, sincronize todos os ativos e carregue as alterações no [!DNL Experience Manager]. Isso evita que você perca edições ao desinstalar o aplicativo.

1. Desinstale a versão anterior do aplicativo. Ao desinstalar, selecione a opção para limpar o cache.

1. Reinicie o computador.

1. [Baixe](release-notes.md) e [instale](#install-v2) o aplicativo mais recente. Siga as instruções abaixo.

## Instalar {#install-v2}

Para instalar o aplicativo de desktop, siga estas etapas. Desinstale qualquer aplicativo de desktop Adobe [!DNL Experience Manager] existente v1.x antes de instalar o aplicativo mais recente. Para obter mais informações, consulte acima.

1. Baixe o instalador mais recente da página [notas de versão](release-notes.md).

1. Mantenha a URL e as credenciais da sua implantação do [!DNL Experience Manager] acessíveis.

1. Se você estiver atualizando de outra versão do aplicativo, consulte [atualizar aplicativo de desktop](#upgrade-from-previous-version).

1. Pule esta etapa se estiver usando o [!DNL Experience Manager] como um [!DNL Cloud Service], [!DNL Experience Manager] 6.4.4 ou posterior, ou [!DNL Experience Manager] 6.5.0 ou posterior. Verifique se a instalação do [!DNL Experience Manager] atende aos requisitos de compatibilidade mencionados nas [notas de versão](release-notes.md). Se necessário, baixe o [pacote de compatibilidade](https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/cq640/featurepack/adobe-asset-link-support) aplicável e instale-o usando o Gerenciador de Pacotes [!DNL Experience Manager] como administrador [!DNL Experience Manager]. Para instalar um pacote, consulte [Como trabalhar com pacotes](https://experienceleague.adobe.com/en/docs/experience-manager-65/content/sites/administering/contentmanagement/package-manager).

1. Execute o binário do instalador e siga as instruções na tela para instalar o.

1. No Windows, o instalador pode solicitar a instalação de `Visual Studio C++ Redistributable 2015`. Siga as instruções na tela para instalá-lo. Se a instalação falhar, instale-a manualmente. Baixe o instalador de [aqui](https://www.microsoft.com/en-us/download/details.aspx?id=52685) e instale os arquivos `vc_redist.x64.exe` e `vc_redist.x86.exe`. Execute novamente o instalador do aplicativo de desktop [!DNL Experience Manager].

1. Reinicie o computador conforme solicitado. Inicie e configure o aplicativo de desktop.

1. Para conectar o aplicativo com um repositório [!DNL Experience Manager], clique no ícone do aplicativo na bandeja e inicie o aplicativo. Forneça o endereço do servidor [!DNL Experience Manager] no formato `https://[aem_server]:[port]/`.

   Clique em **[!UICONTROL Connect]** e forneça as credenciais.

   ![Tela de conexão do aplicativo de desktop para o endereço do servidor de entrada](assets/connect_da2.png)

   *Figura: tela de conexão para endereço do servidor de entrada.*

   Selecione **[!UICONTROL Remember Connection]** para evitar inserir os detalhes da conexão sempre que você fizer logon no aplicativo de desktop.

   >[!CAUTION]
   >
   >Verifique se não há espaços à esquerda ou à direita antes ou depois do endereço do servidor [!DNL Experience Manager]. Caso contrário, o aplicativo não poderá se conectar ao servidor [!DNL Experience Manager].

1. [Opcional] Clique em **[!UICONTROL I want to connect a different way]** e em **[!UICONTROL Adobe login]** para fazer logon no servidor Experience Manager Assets usando o Adobe Identity Management Service (IMS). O logon IMS permite que o aplicativo de desktop execute a atualização do token de acesso automaticamente, permitindo que o usuário permaneça conectado por até 14 dias. Clique em **[!UICONTROL Direct login]** para executar o logon padrão no servidor [!DNL Experience Manager] usando as credenciais do usuário.

   ![Logon de Adobe](assets/adobe-login.png)

1. Após a conexão bem-sucedida, você pode visualizar a lista de pastas e ativos disponíveis na pasta raiz do DAM [!DNL Experience Manager]. Você pode navegar pelas pastas de dentro do aplicativo.

   ![No logon, o aplicativo exibe o conteúdo do DAM](assets/firstview_da2.png)

   *Figura: o aplicativo exibe o conteúdo do DAM após o logon*

1. ([!DNL Experience Manager] 6.5.1 ou posterior) Se você estiver usando o aplicativo de desktop com [!DNL Experience Manager] 6.5.1 ou posterior, atualize o conector S3 ou Azure para a versão 1.10.4 ou posterior. Consulte [conector do Azure](https://experienceleague.adobe.com/en/docs/experience-manager-65/content/implementing/deploying/deploying/data-store-config#azure-data-store) ou [conector S3](https://experienceleague.adobe.com/en/docs/experience-manager-65/content/implementing/deploying/deploying/data-store-config#amazon-s-data-store).

   Se você for um cliente do Adobe Managed Services (AMS), entre em contato com o Suporte ao cliente do Adobe.

## Definir preferências {#set-preferences}

Para alterar as preferências, clique em ![Ícone de mais opções](assets/do-not-localize/more_options_da2.png) e **[!UICONTROL Preference]** ![Ícone de preferências](assets/do-not-localize/preferences_icon_da2.png). Na janela **[!UICONTROL Preferences]**, ajuste os valores do seguinte:

* [!UICONTROL Launch the application on logon].

* [!UICONTROL Show a window when the application starts].

* **[!UICONTROL Cache Directory]**: Local do cache local do aplicativo (contém os ativos baixados localmente).

* **[!UICONTROL Network Drive Letter]**: A letra da unidade usada para mapear para o DAM [!DNL Experience Manager]. Não altere esta letra de unidade de rede se não tiver certeza. O aplicativo pode mapear para qualquer letra de unidade no Windows. Se dois usuários colocarem ativos de letras de unidade diferentes, eles não poderão ver os ativos colocados um pelo outro. O caminho dos ativos muda. Os ativos permanecem colocados no arquivo binário (digamos INDD) e não são removidos. O aplicativo lista todas as letras de unidade disponíveis e, por padrão, usa a última letra disponível que normalmente é `Z`.

* **[!UICONTROL Maximum Cache Size]**: cache permitido no disco rígido em GB usado para armazenar ativos baixados localmente.

* **[!UICONTROL Current cache size]**: tamanho de armazenamento dos ativos baixados localmente. As informações são exibidas somente após o download dos ativos usando o aplicativo.

* **[!UICONTROL Automatically download linked assets]**: ao baixar o arquivo original, os ativos colocados em aplicativos Creative Cloud nativos com suporte são buscados automaticamente.

* **[!UICONTROL Maximum number of downloads]**: ![ícone de cuidado](assets/do-not-localize/caution-icon.png). Altere com cuidado. Ao baixar ativos pela primeira vez (por meio da opção Revelar, Abrir, Editar, Baixar ou semelhante), os ativos serão baixados somente se o lote contiver menos que esse número. O valor padrão é 50. Não altere se não tiver certeza. Aumentar o valor pode resultar em tempos de espera mais longos, enquanto reduzi-lo pode impedir que você baixe todos os ativos ou pastas necessários em uma única tentativa.

* **[!UICONTROL Use legacy conventions when creating nodes for assets and folders]**: ![ícone de cuidado](assets/do-not-localize/caution-icon.png). Altere com cuidado. Esta configuração permite que o aplicativo emule o comportamento do aplicativo v1.10 ao carregar pastas. Na v1.10, os nomes de nó criados no repositório respeitam os espaços e a capitalização dos nomes de pasta fornecidos pelo usuário. No entanto, na v2.1 do aplicativo, os espaços extras nos nomes de pasta são convertidos em traços. Por exemplo, carregar `New Folder` ou `new   folder` criará o mesmo nó no repositório se a opção não estiver selecionada e o comportamento padrão na v2.1 for retido. Se essa opção estiver selecionada, nós diferentes serão criados no repositório para as duas pastas acima e ele corresponderá ao comportamento do aplicativo v1.10.

  O comportamento padrão da v2.1 permanece inalterado: ele substitui vários espaços em nomes de pastas por traços no nome do nó do repositório e converte os nomes dos nós em minúsculas.

* **[!UICONTROL Upload Acceleration]**: ![ícone de cuidado](assets/do-not-localize/caution-icon.png). Altere com cuidado. Ao fazer upload de ativos, o aplicativo pode usar uploads simultâneos para melhorar a velocidade de upload. Você pode aumentar a simultaneidade do upload movendo o controle deslizante para a direita. O controle deslizante no lado esquerdo distante significa que não há simultaneidade (upload de segmento único), a posição intermediária corresponde a dez threads simultâneos e o limite máximo no lado direito distante corresponde a 20 threads simultâneos. Um limite de simultaneidade mais alto consome mais recursos.

Para atualizar as preferências indisponíveis, faça logoff do servidor [!DNL Experience Manager] e, em seguida, atualize. Depois de atualizar as preferências, clique em ![Salvar preferências](assets/do-not-localize/save_preferences_da2.png).

![Preferências e configurações do aplicativo de desktop](assets/preferences_da2.png)

*Figura: Preferências do aplicativo de desktop.*

### Suporte de proxy {#proxy-support}

O aplicativo de desktop [!DNL Experience Manager] usa o proxy predefinido do sistema para se conectar à Internet via HTTPS. O aplicativo só pode se conectar usando um proxy de rede que não exija autenticação extra.

Se você definir ou modificar as configurações de servidor proxy para o Windows (Opções da Internet > Configurações da LAN), reinicie o aplicativo de desktop [!DNL Experience Manager] para que as alterações entrem em vigor. A configuração de proxy se aplica ao iniciar o aplicativo de desktop. Feche e reinicie o aplicativo para que as alterações entrem em vigor.

Se o proxy exigir autenticação, a equipe de TI poderá permitir que a URL [!DNL Experience Manager Assets] nas configurações do servidor proxy permita a passagem do tráfego do aplicativo.

## Desinstalar o aplicativo {#uninstall-the-app}

Para desinstalar o aplicativo no Windows, siga estas etapas:

1. Carregue todas as alterações no [!DNL Experience Manager] para evitar a perda de edições. Consulte [Editar ativos e carregar ativos atualizados para [!DNL Experience Manager]](using.md#edit-assets-upload-updated-assets). Faça logoff e [!UICONTROL Exit] o aplicativo.

1. Remova o aplicativo como removeria qualquer outro aplicativo do sistema operacional. Desinstale-o em Adicionar e remover programas no Windows.

1. Para remover o cache e os logs, marque a caixa de seleção necessária.

   ![Caixa de diálogo de desinstalação para remover logs e cache](assets/uninstall_da2.png)

1. Siga as instruções na tela. Quando terminar, reinicie o computador.

Para desinstalar o aplicativo no Mac, siga estas etapas:

1. Carregue todas as alterações no [!DNL Experience Manager] para evitar a perda de edições. Consulte [Editar ativos e carregar ativos atualizados para [!DNL Experience Manager]](using.md#edit-assets-upload-updated-assets). Faça logoff e [!UICONTROL Exit] o aplicativo.

1. Remova o `Adobe Experience Manager Desktop.app` de `/Applications`.

Como alternativa, para limpar os caches de aplicativos internos no Mac e desinstalar o aplicativo, você pode executar o seguinte comando no terminal:

```shell
/Applications/Adobe Experience Manager Desktop/Contents/Resources/uninstall-osx/uninstall.sh
```
