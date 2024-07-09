---
title: Notas de versão do aplicativo de desktop v1.10
description: Detalhes da versão, melhorias, novos recursos, compatibilidade e links de download para o aplicativo para desktop AEM versão 1.10.
exl-id: 886864e0-016a-4a17-b3ba-4b18a514214a
source-git-commit: 23719d2f5d92f6031687df18036acdbc04722402
workflow-type: tm+mt
source-wordcount: '3989'
ht-degree: 0%

---

# [!DNL Adobe Experience Manager] notas de versão do aplicativo de desktop v1.10 {#aem-desktop-app-release-notes}

Para a versão v1.x do aplicativo de desktop, veja a seguir os links de download e as informações de compatibilidade do AEM.

| Produtos | Aplicativo de desktop do [!DNL Adobe Experience Manager] |
|--- |--- |
| Versão | 1.10 (1.10.0.6 no Mac e 1.10.0.3 no Windows) |
| Tipo | Versão secundária |
| Data | 1.10.0.6 (Mac): 15 de abril de 2020; 1.10.0.3 (Win): 31 de agosto de 2018 |
| URLs para download | [macOS X 64 bits](https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/adobe/aem-desktop-app/aem-desktop-osx-1.10.0.6.dmg); [Windows de 32 bits](https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/adobe/aem-desktop-app/aem-desktop-win32-1.10.0.3.exe); [Windows de 64 bits](https://experience.adobe.com/#/downloads/content/software-distribution/en/aem.html?package=/content/software-distribution/en/details.html/content/dam/aem/public/adobe/packages/adobe/aem-desktop-app/aem-desktop-win64-1.10.0.3.exe) |
| Compatibilidade | AEM 6.5.x; AEM 6.4.x; AEM 6.3 SP2; AEM AEM 6.2 SP1 CFP2+; 6.1 SP2 CFP7+ |

>[!NOTE]
>
>O limite de tamanho do cache não é aplicado. Quando o aplicativo de desktop é iniciado, o tamanho do cache é calculado uma vez e uma notificação é exibida se o tamanho estiver próximo do limite predefinido.

## Requisitos e pré-requisitos do sistema {#system-requirements-and-prerequisites}

[!DNL Adobe Experience Manager] o aplicativo de desktop é compatível com os seguintes sistemas operacionais:

* macOS X 10.10 ou mais recente, com as correções de erros mais recentes.

* Windows 10 com os service packs e correções de erros mais recentes.

A Adobe recomenda o uso da versão mais recente do aplicativo de desktop AEM para garantir que você esteja usando as funcionalidades mais recentes, as correções de erros mais recentes e o melhor desempenho possível.

A versão do aplicativo para desktop AEM que você pretende instalar no computador local requer uma versão específica do servidor AEM/componentes adicionais do servidor (service packs, hot fixes ou pacotes de recursos). Verifique se o servidor AEM está configurado corretamente antes de se conectar a ele pela primeira vez. Se precisar de ajuda, entre em contato com o administrador do AEM.

Consulte a [matriz de compatibilidade detalhada](#compatibilitymatrix) no final deste documento para avaliar os pré-requisitos da sua configuração.

## Novidades no aplicativo de desktop v1.10 {#what-s-new-in-aem-desktop-app}

O aplicativo para desktop AEM 1.10 tem como objetivo melhorar a experiência do usuário com uploads grandes, informações sobre as operações em segundo plano e experiência otimizada ao abrir ativos com arquivos vinculados (como o InDesign).

>[!NOTE]
>
>Se você estiver usando o macOS 10.15.4 ou mais recente, use a versão 1.10.0.6 do aplicativo. Esta versão de patch está em conformidade com [Requisitos de autenticação do Apple](https://developer.apple.com/news/?id=04102019a).

**Edição local / Check-out**: os uploads automáticos de alterações salvas em ativos podem ser desativados na janela de status. Dessa forma, o usuário pode continuar trabalhando nos arquivos e salvando as alterações e, quando estiverem prontos, decidir fazer upload de todas as alterações.

**Janela Status do ativo simplificado**. A janela de status foi simplificada. A variável [!UICONTROL Uploads] A guia agora mostra ativos individuais e carregamentos em pasta ou em massa. A guia anterior de uploads em massa foi removida.

**Ícone de aplicativo para indicar uploads em massa**. O ícone do aplicativo indica que um upload em massa está em andamento ao mostrar uma sobreposição de &quot;transferência&quot;.

**Notificações para Conflitos de Atualização**. Quando o aplicativo detecta um conflito durante uma atualização de ativo, ele exibe uma notificação, permitindo que o usuário o revise sem monitorar a janela de status. Na inicialização, o aplicativo verifica todos os conflitos, permitindo que o usuário os resolva.

**Melhor tratamento das perdas de conexão**. Os uploads em massa são pausados em caso de perda de conexão e o usuário pode retomar o processo posteriormente. A [!UICONTROL Retry] A opção está disponível para tentar novamente um upload com falha de um arquivo individual.

## Instruções de instalação {#installation-instructions}

Para obter instruções detalhadas, consulte [Instalar e configurar o aplicativo de desktop AEM](install-configure-app-v1.md).

## Melhorias nas versões anteriores {#enhancements-in-the-previous-versions}

Esta versão estende e substitui as versões anteriores da [!DNL Experience Manager] aplicativo de desktop da, que forneceu as seguintes melhorias principais:

* **Versão 1.9 / 1.9.1**: uploads retomáveis, janela de status aprimorada, ícones de aplicativo que indicam o status do aplicativo/conexão, pré-busca de ativos vinculados para arquivos do InDesign.

* **Versão 1.8**: melhor controle do tamanho do cache para o usuário, experiência de logon aprimorada para SAML/SSO no Windows, suporte `.pac` proxy de rede no Mac e problemas relatados pelo cliente.

* **Versão 1.7**: melhorias na estabilidade e na lógica de cache, melhor suporte para proxy de rede e capacidade de limpar arquivos internos após a desinstalação.

* **Versão 1.6**: melhorias no processo de logon para várias configurações de segurança AEM e estabilidade e desempenho do aplicativo.

* **Versão 1.5**: estabilidade e resiliência de aplicativos contra vários problemas de rede, melhor capacidade de suporte.

* **Versão 1.4**: a capacidade de fazer upload de pastas hierárquicas em segundo plano com o monitoramento do progresso.

* **Versão 1.3**: aprimoramentos de desempenho e estabilidade de acesso a arquivos e salvamento de alterações no AEM, especialmente em aplicativos de desktop Creative Cloud, como InDesign, Illustrator ou Photoshop. O objetivo era proporcionar aos usuários uma experiência mais semelhante à de um desktop local ao trabalhar com arquivos, enquanto manipulava simultaneamente operações de transferência de dados em rede em segundo plano.

### Melhorias disponíveis desde o aplicativo de desktop AEM 1.9 {#Enhancements-Available-Since-AEM-Desktop-App-19x}

[!DNL Adobe Experience Manager] A versão 1.9.1 do aplicativo de desktop do foi uma versão de patch. Ele foi projetado para solucionar os principais problemas do cliente com a finalização de ativos. E endereçar copiando arquivos de um compartilhamento de rede para um diretório local.

* O Assets desmarcado por um usuário não deve estar disponível para modificação para outros usuários (CQ-4246009)

* Cópia compatível de uma pasta mapeada para uma pasta local quando a pasta do usuário estiver em uma partição de disco separada (CQ-4243978)

O aplicativo para desktop AEM 1.9 tem como objetivo melhorar a experiência do usuário com uploads grandes, informações sobre as operações em segundo plano e experiência otimizada ao abrir ativos com arquivos vinculados (como o InDesign).

**Uploads retomáveis**
Para uploads, especialmente em arquivos grandes, há uma opção para pausá-los/retomá-los na nova janela Status do ativo.

**Janela Status do ativo aprimorada**
Uma janela de Status do ativo aprimorada fornece as seguintes informações sobre os ativos.

[!UICONTROL Changes]

* Exibe as alterações atualmente na fila.

* Exibe uploads em andamento com uma barra de progresso, taxa de transferência, tamanho total do arquivo e a quantidade transferida até o momento.

* Uploads concluídos mostrados com o total transferido e a taxa final.

* Os uploads com falha são exibidos junto com uma mensagem de erro e informações de transferência, se disponíveis.

* Carregamentos que falharam três vezes mostram uma mensagem de erro.

* Os arquivos conflitantes são exibidos com um ícone no qual o usuário pode clicar. Clicar no ícone mostra uma caixa de diálogo com uma explicação e duas opções:

   * [!UICONTROL Keep Mine] faz o upload do arquivo imediatamente no servidor.

   * [!UICONTROL Overwrite Mine] O exclui imediatamente o arquivo local e baixa uma nova cópia do servidor.

[!UICONTROL Downloads]

* Exibe downloads em andamento, incluindo uma taxa de transferência e o tamanho transferido até o momento.

* Os downloads concluídos são exibidos com o total transferido, a taxa final e um ícone que abre o arquivo ao clicar (disponível somente para arquivos únicos).

* Downloads malsucedidos exibidos com uma mensagem de erro e informações de transferência, se disponíveis.

* O rodapé mostra o número total de arquivos baixados e a taxa média de transferência.

* Se um usuário optar por abrir ou editar vários arquivos no [!DNL Experience Manager Assets] Web, elas são agrupadas. Por exemplo, myasset.jpeg e mais 4 arquivos.

* Ao baixar documentos do InDesign com ativos vinculados do AEM Assets, o aplicativo de desktop primeiro baixa todos os ativos vinculados antes de abrir o documento e indicar o status do download. Por exemplo, 5 de 24.

[!UICONTROL Bulk Uploads]

Fazer upload de grandes hierarquias de pastas por meio de [!UICONTROL Create] > [!UICONTROL Upload Folder] na interface da Web do AEM aciona essa caixa de diálogo. O mesmo ocorre ao copiar e selecionar &quot;Colar Assets&quot; no Finder ou Explorer no menu de contexto do aplicativo de desktop.

* Exibe uploads em andamento, incluindo uma barra de progresso e o nome do arquivo que está sendo transferido.

* Os uploads em andamento incluem um ícone que cancela o upload quando clicado. A transferência é interrompida depois que o arquivo atualmente em transferência é concluído.

* Os processos de transferência com falha são exibidos com uma mensagem de erro (somente se toda a transferência falhar).

* Se um arquivo individual não for transferido, ele será exibido na guia como um erro. Caso contrário, os arquivos individuais não serão exibidos na guia * apenas uma única entrada para todo o upload.

**Ícones para Indicar o Status das Operações em Segundo Plano**

O ícone do aplicativo indica o estado das operações em segundo plano para fornecer uma dica visual melhor aos usuários. Por exemplo, quando o aplicativo não está conectado ao AEM, o ícone fica esmaecido. Quando há um upload ativo, ele mostra uma sobreposição de &quot;sincronização&quot; e assim por diante.

**Pré-busca do Assets vinculado**

Para aprimorar a experiência do usuário com documentos do InDesign que contêm ativos vinculados armazenados no AEM, o aplicativo de desktop busca previamente esses arquivos vinculados no cache local. Esse fluxo ocorre antes de baixar e abrir o documento do InDesign. Dessa forma, o usuário tem os arquivos vinculados disponíveis localmente e não precisa aguardar mais ao acessar ativos no InDesign (no painel Links ).
A busca prévia só funciona se o AEM reconhecer os links no lado do servidor. Um ativo com links reconhecidos tem uma lista de &quot;Referências&quot; listadas na visualização Propriedades do ativo do InDesign.

### Melhorias disponíveis desde o aplicativo de desktop AEM 1.8.x {#enhancements-available-since-aem-desktop-app-18x}

A versão de acompanhamento rápido do aplicativo de desktop AEM 1.8.1 adicionou melhorias ao abrir vários arquivos de uma só vez da interface AEM para a versão 1.8 (CQ-4237747, CQ-4238780). As melhorias no aplicativo para desktop AEM 1.8 são:

* Armazenamento em cache: nova interface para gerenciar o cache do aplicativo de desktop AEM (CQ-4208690), incluindo,

   * exibir tamanho atual do cache

   * definir o tamanho máximo do cache antes do envio de uma notificação

   * O tamanho do cache é verificado somente na inicialização do aplicativo de desktop, e uma notificação é exibida se estiver atingindo o limite configurado

   * o botão limpar cache agora está disponível na nova interface do usuário

* Logon: (Win) correção do logon na instância do AEM configurada para usar SAML e SSL (CQ-4216353)

* Rede:

   * quando uma sessão de AEM expira, o usuário agora é notificado e pode clicar na notificação para fazer logon novamente (CQ-4202028).

   * (Mac) Adicionar suporte para conexão com AEM por meio do uso do `.pac` configuração de proxy (CQ-4233430).

   * (Win) corrija problemas com a caixa de diálogo Avançado - URL de logon (CQ-4236061).

* Correções de erros:

   * Caixa de diálogo Mais informações do ativo: às vezes, a barra de ação não estava visível (CQ-4208540).

   * (Win) O arquivo agora pode ser sincronizado após reverter para uma versão anterior da interface do usuário do AEM Assets (CQ-4216411).

### Melhorias disponíveis desde o aplicativo de desktop AEM 1.7 {#Enhancements-Available-Since-AEM-Desktop-App-17}

* Estabilidade:

   * Estabilidade aprimorada quando o aplicativo de desktop AEM se conecta a um servidor AEM sobrecarregado (CQ-4224803).

   * Estabilidade aprimorada quando muitos arquivos são solicitados (CQ-4224212).

   * Atualização de ativos aprimorada com verificação adicional (CQ-4228291).

* Armazenamento em cache:

   * Correção de erros de disco e problemas de abertura ao abrir arquivos no Photoshop, InDesign, Finder (CQ-4223993, CQ-4217603, CQ-4223717).

   * Armazenamento em cache aprimorado para evitar binários de tamanho zero (CQ-4216599).

* Logon: permitir a conexão com strictSSL desabilitado para configurações especiais (como certificados emitidos localmente) (CQ-4223949).

* Rede: suporte aprimorado para conexão via proxy de rede (CQ-4223477, CQ-4221280, CQ-4206854).

* Instalação e desinstalação:

   * (Win) Desinstalação do limpador (CQ-4220906).

   * [Windows de 32 bits] Falha do instalador ao tentar instalar o Microsoft .NET Framework v. 4.5 (CQ-4218084).

   * (Mac) Script manual para remover completamente os arquivos de aplicativo de desktop (CQ-4216489).

>[!NOTE]
>
>Problemas encontrados nas cargas beta do aplicativo para desktop AEM 1.7 que estavam ausentes na versão 1.6 são omitidos das notas de versão.

### Melhorias disponíveis desde o aplicativo de desktop AEM 1.6 {#Enhancements-Available-Since-AEM-Desktop-App-16}

* Documentação: nova [Práticas recomendadas para o aplicativo v1.x](/help/using/best-practices-for-v1.md) documentação.

* Processo de logon aprimorado para AEM:

   * Melhorar o manuseio de SAML * regras de atenuação (CQ-4202781).

   * Adicione a capacidade de configurar um URL de logon separado em Preferências (CQ-4214052, CQ-4214051).

* Usabilidade: notifique o usuário quando um ativo ainda estiver sendo baixado para ativos maiores (CQ-4216284).

* Rede:

   * Armazenamento em cache DNS (CQ-4210176).

   * Conexão de suporte via proxy no Windows (CQ-4206854).

* Armazenamento em cache e acesso ao compartilhamento de rede no Finder/Explorer:

   * O ícone de bloqueio agora está visível para ativos com check-out no Windows 10 (CQ-90957).

   * O conteúdo da pasta pode desaparecer/reaparecer no compartilhamento de rede (CQ-4209160, CQ-4210180).

   * Erro no upload do arquivo devido a um conflito relatado no Status da fila de upload (CQ-4215727).

   * Ao abrir vários arquivos da pasta de aplicativos de desktop no PS, mensagens truncadas ou incompletas de arquivos podem ser exibidas (CQ-4216276).

* Correções na estabilidade e no desempenho:

   * Desempenho aprimorado ao navegar pelas pastas com muitos ativos (CQ-4214933).

   * O aplicativo de desktop 1.5 pode desacelerar uma máquina de desktop ao longo do tempo (CQ-4209159).

   * O recurso Mostrar status da fila funciona somente para o usuário que instalou o aplicativo (CQ-4212199).

   * (Windows) Verifique se o instalador de 32 bits não contém o código de 64 bits (CQ-4217406).

* Problemas selecionados encontrados e corrigidos em 1.6 Beta:

   * Alto uso da CPU (CQ-4218070).

   * Arraste e solte arquivos que geram erros ao fazer upload para o AEM (CQ-4217006).

### Melhorias disponíveis desde o aplicativo de desktop AEM 1.5 {#Enhancements-Available-Since-AEM-Desktop-App-15}

**Versão 1.5.1.5 para macOS X:** A versão 1.5.1.5 oferece os seguintes benefícios:

* Novos recursos e melhorias: adicione a funcionalidade Copiar/Colar à integração do Finder para permitir a transferência direta do desktop para o AEM (CQ-4208158).

* Correções de erros:

   * Correção do problema 43 que ocorria às vezes durante a renomeação de ativos (CQ-4207900).

   * Reverter para uma versão mais antiga da linha do tempo no AEM não atualiza o ativo no Localizador (CQ-4205194).

   * O aplicativo de desktop trava ao navegar em diretórios aninhados grandes (CQ-4208539).

   * O ponto de montagem do aplicativo de desktop agora é /Volumes/DAM, portanto, é consistente para todos os usuários (CQ-4208159).

   * Colocar um arquivo no InDesign pela primeira vez inicia um aviso de atualização (CQ-4207454).

Observação sobre avisos de link: os aplicativos Creative Cloud (como o InDesign) fazem um &quot;instantâneo&quot; da hora da última modificação do item no momento em que ele é colocado. Se essa data for alterada posteriormente, o aplicativo Adobe Creative Cloud relata que os links estão desatualizados. Essas informações são relatadas de duas maneiras:

* Quando o aplicativo Adobe Creative Cloud é iniciado, ele exibe uma caixa de diálogo informando ao usuário que os ativos vinculados estão desatualizados e solicita que o usuário tome uma ação.

* Se o aplicativo Adobe Creative Cloud já estiver em execução, ele mostrará um ícone de aviso de triângulo amarelo no ativo vinculado.

Esse comportamento é o mesmo para ativos no disco local e ativos em um diretório montado em um desktop AEM, com as seguintes exceções:

* Se um usuário diferente editar um ativo inserido, o ícone de aviso será exibido na primeira vez que outros usuários abrirem um documento contendo o ativo inserido. Esse aviso só acontece se o ativo inserido já tiver sido armazenado em cache localmente.

* Se um usuário modificar um ativo inserido por meio do diretório montado do desktop AEM e, em seguida, limpar o cache local, o ativo inserido será relatado como desatualizado.

Ambos os casos são esperados e são efeitos colaterais da arquitetura de &quot;sincronização atrasada&quot; do desktop AEM.

**Versão 1.5.0.x para macOS X e Windows:** Essa versão do aplicativo para desktop AEM oferece os seguintes benefícios:

* Maior estabilidade e resiliência contra problemas de rede.

   * Mapeamento mais estável de pastas do AEM Assets (CQ-103276, CQ-4204669, CQ-4203957).

   * Melhor tratamento dos arquivos em cache (CQ-4204336, CQ-4206263).

   * Manuseio aprimorado de download/upload de arquivos grandes com mais de 2 GB (CQ-4206438).

   * Correção do &quot;Erro 36&quot; ao mover ou renomear um número maior de arquivos no Finder (CQ-4204640).

* Otimizações na comunicação de rede com o servidor AEM (CQ-4204974, CQ-100903).

* Aprimoramento da confiabilidade de abrir, colocar e salvar ativos do AEM em aplicativos Creative Cloud (CQ-4203968, CQ-4205511, CQ-103543, CQ-4207141, CQ-90980).

* Melhor capacidade de suporte: opção para limpar o cache (CQ-4202541), acesso fácil a registros (CQ-4202340, CQ-4204673).

* Outras correções:
   * Melhor suporte para ativos e pastas que têm caracteres japoneses nas configurações de nome/idioma diferentes do inglês (CQ-4195433, CQ-4205793, CQ-4199446).

   * Melhor tratamento de logon com SSL (CQ-4200217).

   * Montagem de compartilhamento mais confiável (CQ-4200793).

   * Várias melhorias na estabilidade (CQ-4207539, CQ-4200378).

   * Melhor manipulação do URL do AEM Assets em Preferências (CQ-97388).

### Melhorias disponíveis desde o aplicativo de desktop AEM 1.4 {#Enhancements-Available-Since-AEM-Desktop-App-14}

* Upload simplificado de pastas hierárquicas por meio da nova ação Criar > Fazer upload da pasta na interface para toque.
   * Esta ação inicia uma operação de carregamento de pasta realizada pelo aplicativo de desktop.
   * O aplicativo de desktop atravessa a hierarquia de pastas fornecida no desktop em segundo plano e faz upload dos arquivos para o AEM Assets.
   * O usuário pode monitorar o progresso na nova janela Fazer upload do status da fila para operações em andamento.
   * O Status da fila de uploads também fornece melhores informações de solução de problemas (por exemplo, sem conexão com o servidor).
* Nova ação Editar na interface para toque que combina operações de Check-out e Abrir em uma única.
* Agrupamento otimizado de ações relacionadas ao desktop na interface para toque (AEM 6.3).
* Maior compatibilidade com as versões mais recentes do sistema operacional.
* O cliente relatou correções.

### Melhorias disponíveis desde o aplicativo de desktop AEM 1.3 {#Enhancements-Available-Since-AEM-Desktop-App-13}

* Maior eficiência. Os usuários gastam menos tempo aguardando a conclusão das operações de rede.
* Aprimoramento da integração do Localizador, que fornece mais estabilidade e acesso a recursos, como miniaturas.
* Armazenamento em cache e melhorias de desempenho.
* Melhor suporte para salvar diretamente de aplicativos de desktop (PS, ID, AI e assim por diante).
* Melhor integração com o macOS (protocolo de unidade de rede local alterado de WebDAV para SMB1 mais estável).
* O aplicativo de desktop se conecta com o servidor AEM usando o protocolo RESTful HTTP nativo AEM.
* Primeiro, os arquivos são salvos localmente e depois carregados de volta no AEM em segundo plano após um tempo predefinido (30 segundos). Esse fluxo de trabalho reduz o tempo de salvamento de arquivos.
* Melhor manuseio de aplicativos de desktop que usam operações de arquivo intermediárias para salvar um arquivo (salvamentos parciais e arquivos temporários), o que permite que a linha do tempo do ativo AEM exiba as informações corretas de versão e upload de ativos.
* Uma caixa de diálogo é fornecida para rastrear o status das tarefas de upload em segundo plano.

## Lista de alterações {#list-of-changes}

### Ponto de montagem no Mac {#mount-point-on-mac}

Desde o macOS 10.12 (Sierra), a Apple alterou as permissões na pasta /Volumes usadas para montar unidades de rede e dispositivos para serem mais restritivos. A criação de um novo ponto de montagem nesse local exigia direitos administrativos. Este problema foi corrigido no macOS 10.12.5.

O ponto de montagem do aplicativo de desktop AEM foi alterado nas versões 1.4 e 1.5. No macOS, ele foi alterado para uma subpasta DAM na pasta local do usuário, compatível com usuários não administradores (CQ-104183).

Como a variável `/Volumes` A pasta do não requer mais direitos administrativos. esta alteração foi revertida na 1.5.1. Essa alteração também possibilita o compartilhamento de documentos do InDesign que colocaram ativos do AEM entre usuários do macOS.

### Alteração de protocolo (desde a v1.3) {#protocol-change-since}

* macOS X:
   * O protocolo de unidade de rede local para integração de desktop do OS X foi alterado para SMB1 a partir do WebDAV.
   * O repositório AEM montado com o aplicativo de desktop está visível como um `smb` no Finder, em vez de um drive WebDAV.
* Windows:
   * O protocolo de unidade de rede local para integrações de desktop do Windows permanece; o AEM é montado como um compartilhamento WebDAV.
* Para ambas as plataformas (Windows e Mac):
   * O protocolo para acessar / baixar ativos e fazer upload de alterações no AEM foi alterado para o protocolo AEM nativo, que é um protocolo RESTful baseado em HTTP. Ele oferece maior controle sobre as operações de rede e é mais compatível com a infraestrutura de rede.

>[!NOTE]
>
>No macOS X, a alteração do protocolo de unidade de rede local de WebDAV para SMB1 resulta em um caminho local diferente para o mesmo ativo no repositório. Essa alteração pode afetar links para arquivos colocados em aplicativos do Adobe Creative Cloud por meio do comando &quot;Inserir&quot;. Consulte a [Usar o aplicativo de desktop AEM](use-app-v1.md) para obter mais informações.

### Manuseio de arquivos (desde 1.3) {#file-handling-since}

* As pastas são atualizadas automaticamente após um atraso predefinido (atualmente 30s).
* Os arquivos submetidos a check-out por outros usuários são marcados como somente leitura.
* Os arquivos são salvos em um local de unidade de rede montado por meio do aplicativo de desktop em duas fases.
* Na primeira fase, um arquivo é salvo localmente. Dessa forma, o usuário que salva o arquivo não precisa esperar até que ele seja totalmente transferido para o AEM e pode retomar o trabalho assim que o arquivo for salvo.
* Na segunda fase, o aplicativo de desktop carrega um arquivo atualizado no servidor AEM após um atraso predefinido (por exemplo, trinta segundos). Esta operação ocorre em segundo plano. Use o **Mostrar Status de Sincronização de Arquivos em Segundo Plano** opção para visualizar o status da operação de upload.

## Avisos importantes {#important-notices}

**Carregamento de pasta.** A Adobe recomenda que você use o novo recurso de upload de pastas para fazer upload de pastas maiores e hierárquicas para AEM. Essa abordagem é recomendada em vez de usar uma cópia/arrastar e soltar em um repositório AEM montado no nível Finder/Explorer. Ao usar o recurso de carregamento de pasta, o aplicativo de desktop se comunica diretamente com o AEM e, portanto, tem muito melhor controle sobre o processo geral.

**Mantenha a sessão do AEM disponível.** O aplicativo de desktop AEM depende de uma sessão aberta no servidor do AEM Assets para garantir a operação adequada. Os usuários diários devem desmontar o AEM Assets ao final do dia para fazer logoff e remontar pela manhã para garantir a funcionalidade de logon e compartilhamento de rede.

**Desative &quot;Visualização de ícone&quot; no Localizador.** Para a navegação eficiente de pastas grandes com o Finder, especialmente com baixa conectividade de rede, verifique se o &quot;Ícone&quot; e a &quot;Visualização de ícone&quot; estão desativados. Caso contrário, o Localizador inicia o download de cada ativo em uma pasta para gerar uma pequena visualização, o que pode levar a baixo desempenho e alta utilização de largura de banda (CQ-4219779)

* No localizador, vá para a pasta de rede compartilhada da AEM Assets
* Clique com o botão direito do mouse no ponto de montagem do DAM
* Selecione Mostrar opções de exibição
* Desmarque &quot;Mostrar visualização do ícone&quot;
* Clique em &quot;Usar como padrão&quot;

**Limpe o cache ao conectar-se a um novo servidor AEM.** Se o aplicativo de desktop se conectar a outro servidor AEM com o mesmo URL, o cache não será limpo automaticamente. Limpe o cache manualmente para garantir as operações adequadas. Observe que esse processo normalmente ocorreria em testes, quando instalações de AEM podem ser substituídas enquanto são executadas no mesmo URL (CQ-4216982)

**Usar certificados SSL assinados pela CA.** O aplicativo de desktop AEM não é compatível com certificados SSL autoassinados ao se conectar ao AEM por meio de uma conexão segura HTTPS. É necessário um certificado assinado pela CA no servidor para essas conexões. (CQ-87941)

## Problemas conhecidos {#known-issues}

* Geral:
   * Os URLs do servidor são necessários para apontar para o servidor sem um caminho (por exemplo, `http://server`, `https://server`, `http://server:port`ou `https://server:port`). Não há suporte para caminhos e subpastas de contexto diferentes de /content/dam (CQ-89343, CQ-87272)
* Nomes/localização de arquivos:
   * Nomes de arquivos e pastas com caracteres reservados não são manipulados corretamente. Use nomes de arquivos e pastas que atendam aos requisitos do AEM. (CQ-93361, CQ-93308, CQ-89276, CQ-4217183)
   * Alguns aplicativos, como o Adobe Illustrator, podem criar arquivos com nomes não compatíveis com AEM. Por exemplo, adicionar `Converted` após converter um arquivo, o que impede que ele seja carregado. (CQ-4216985)
   * O Assets com nomes internacionais pode aparecer e desaparecer a cada poucos segundos.
* Fazer check-in e check-out:
   * Um ativo retirado por um usuário não pode ser aberto por outro usuário, seja pela ação Abrir da interface do usuário de toque, ou diretamente no desktop. Alguns aplicativos podem relatá-lo como bloqueado, mas também corrompido ou até mesmo travar ao tentar abrir o. (CQ-4199234)
   * A alteração de arquivos simultaneamente por vários usuários pode causar a perda de algumas modificações. A solução alternativa é usar a funcionalidade de check-in e check-out para impedir que vários usuários alterem o mesmo arquivo. (CQ-97035)
   * Determinados aplicativos não oferecem suporte adequado ao sinalizador somente leitura, que permite que um usuário salve um arquivo do qual outro usuário fez check-out. O arquivo modificado não é transferido até que o outro usuário faça check-in do arquivo. Ambas as modificações estão disponíveis no AEM como versões diferentes do ativo. (CQ-89551, CQ-87572, CQ-89615)
   * Os status de check-out e somente leitura são relatados de forma independente no Localizador. Essa abordagem resulta em dois ícones de bloqueio quando um usuário faz o check-out de um ativo. (CQ-89507)
* Integração do localizador:
   * Ao arrastar e soltar arquivos grandes, o Localizador pode atingir o tempo limite enquanto os arquivos estão sendo transferidos em segundo plano. Esse atraso resulta em uma `Error - 36`. A solução alternativa é arrastar e soltar ou abrir o ativo novamente. (CQ-4219628)
   * O recarregamento manual da pasta nem sempre funciona. Solução alternativa: aguarde trinta segundos para que a pasta seja atualizada automaticamente. (CQ-97389)
   * Mais informações do ativo... estão limitadas a seleções de arquivos únicos. (CQ-89542, CQ-87656)
   * Abrir no AEM Assets... é limitado a seleções de arquivos e pastas únicos. (CQ-83382)
   * Erro ao renomear ativos sem extensão. (CQ-4218971)
* Funcionalidade Copiar/Colar: a opção Colar está disponível quando nenhum ativo foi copiado para a área de transferência.
* Windows:
   * Arquivos com Fluxos de Dados Alternativos (ADS) só são totalmente compatíveis com o NTFS. Ao copiar arquivos para o compartilhamento WebDAV por meio do aplicativo de desktop, uma caixa de diálogo de cuidado avisa que algumas propriedades de arquivos não podem ser transferidas para o novo local. Este aviso geralmente é correto porque as propriedades são relevantes apenas para um aplicativo específico na área de trabalho do usuário e não têm nada a ver com o conteúdo real do arquivo. (CQ-103770) (Win)
   * O usuário que está usando o aplicativo de desktop no Windows precisa ser o usuário que irá instalá-lo. (CQ-4216389) (Win)
   * O aplicativo pode falhar ao selecionar o [!UICONTROL Retry] em um upload com falha. Essa falha pode ocorrer em determinadas circunstâncias depois de ter retomado o upload de lote quando desconectado. (CQ-4251884) (Win)

## Recursos úteis {#helpful-resources}

* [Documentação do AEM](https://experienceleague.adobe.com/en/docs)
* [Usar o aplicativo para desktop AEM v1.x](use-app-v1.md)
* [Práticas recomendadas do aplicativo para desktop AEM v1.x](best-practices-for-v1.md)

## Matriz de compatibilidade e pré-requisitos {#compatibilitymatrix}

O aplicativo de desktop AEM funciona com várias versões do AEM. Consulte a matriz de compatibilidade para obter as versões compatíveis.

| Versão | Revisão | Data de lançamento | Compatibilidade |
|--- |--- |--- |--- |
| 1,10 | 1.10.0.3 (Mac e Win) | sábado, 31 de agosto de 2018 | AEM 6.5; AEM 6.4 SP1; AEM 6.3 SP2; AEM AEM 6.2 SP1 CFP2+; 6.1 SP2 CFP7+ |
| 1,9 | 1.9.1.1 (Mac e Win) | 21 de junho de 2018 | AEM 6.4; AEM 6.3 SP1; AEM AEM 6.2 SP1 CFP2+; 6.1 SP2 CFP7+ |
| 1.8 | 1.8.1.0 (Mac e Win) | quinta-feira, 28 de março de 2018 | AEM 6.4; AEM 6.3 SP1; AEM AEM 6.2 SP1 CFP2+; 6.1 SP2 CFP7+ |
| 1,7 | 1.7.0.3 (Mac e Win) | quinta-feira, 10 de janeiro de 2018 | AEM 6.3 SP1; AEM 6.2 SP1 CFP2+; AEM 6.1 SP2 CFP7+ |
