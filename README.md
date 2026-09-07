# Yoru para Windows

[Descarregar Yoru para Windows](https://github.com/afonsohbamorim/yoru-releases/releases)

## No PC Windows

1. Descarrega **Yoru-Setup-0.6.7.exe** na [página de downloads](https://github.com/afonsohbamorim/yoru-releases/releases).
2. Abre e carrega em **Instalar**. As pastas sugeridas servem; podes alterá-las. A primeira abertura precisa de Internet e prepara automaticamente os leitores e serviços.
3. O Yoru abre no browser. Escolhe onde guardar os vídeos e cria o perfil de reprodução. Liga o AniList se quiseres trazer a tua lista.

O ícone Yoru junto ao relógio indica que o serviço está aberto. Podes abrir a interface, escolher **Iniciar com Windows** ou **Sair**. Fechar a página do browser mantém o serviço aberto.

O botão de sol/lua no canto superior direito alterna o tema claro e escuro. A escolha fica guardada nesse browser.

Não precisas de instalar Node, codecs, MPV, MPC-HC, Jellyfin ou qBittorrent à mão. Cada pessoa tem as suas próprias contas e ficheiros. O programa fica na pasta da aplicação; os vídeos podem ficar noutro disco escolhido no Yoru.

Na escolha do armazenamento, seleciona o primeiro disco e usa **Adicionar disco** para acrescentar os restantes discos detetados. As setas definem a ordem de tentativa; cada destino tem a sua própria pasta. Usa **Escolher pasta** para navegar nas pastas do PC; o caminho manual fica nas opções avançadas. Guardar esta ordem não move nem apaga vídeos existentes.

## Na TV

No PC, abre **Definições → Dispositivos → Preparar ligação à TV** e aceita o pedido do Windows. Instala a app **Jellyfin** na loja da TV. Android/Google TV e LG webOS têm clientes nativos; a disponibilidade depende do modelo e da loja.

Dentro da app Jellyfin, introduz o endereço que o Yoru mostra. É a ligação inicial ao servidor do PC; a app guarda-o. No login, escolhe **Quick Connect** e escreve no Yoru o código apresentado na TV. Também podes entrar com o perfil de reprodução criado no PC.

Depois, abres a app da TV e escolhes os vídeos. O PC tem de estar ligado, com sessão Windows iniciada e o Yoru aberto. Ambos os dispositivos têm de estar na mesma rede de casa. Se o router mudar o endereço do PC, atualiza o servidor guardado na TV.

Em **Definições → Dispositivos → Verificar biblioteca e imagem**, confirma as pastas ligadas e os vídeos indexados. Se houver pastas em falta, usa **Ligar pastas em falta e atualizar**. Durante um episódio na TV, verifica novamente para saber se o servidor entrega vídeo original ou convertido.

## No MacBook

Não instales o servidor no Mac. No PC, abre **Definições → Dispositivos**, ativa o acesso pelo browser e gera um código de emparelhamento. No Safari do Mac, abre o endereço **Yoru** apresentado nessa secção e introduz o código. Usa **Disponíveis** para ver a mesma coleção e continuar os episódios.

O endereço Yoru é diferente do endereço Jellyfin da TV. `localhost` no Mac aponta para o Mac, por isso deves usar o endereço do PC. Chrome não é obrigatório. A reprodução e eventual conversão dependem do formato do vídeo e do Mac.

Depois de ligado, o dispositivo fica autorizado até revogares o acesso. Não precisas de renovar semanalmente. Se apagares os dados do browser ou usares navegação privada, poderás precisar de o ligar novamente. Os dispositivos autorizados numa versão antiga têm a opção **Manter autorizado** no PC.

## Obter episódios e atualizar

Na ficha de um anime, escolhe o áudio e o que queres guardar. **Descarregar episódios disponíveis** permite rever todos os emitidos ou os não vistos, confirmar o espaço e iniciar o lote. Os episódios só aparecem em **Disponíveis** depois de concluídos e verificados. Um lote pode esperar por uma edição que cumpra o perfil; a espera tem um motivo visível.

Nas instalações novas, a aquisição automática de planos começa desligada. Ativa-a em **Episódios** para acompanhar a fila. A qualidade, o espaço e a identificação do episódio são sempre verificados antes de iniciar uma transferência.

As transferências ficam agrupadas por anime em **Em curso**, **Pausas e problemas** e **Histórico**. Abre um grupo para ver os episódios. Depois de confirmar o vídeo concluído, o Yoru retira o seu torrent do qBittorrent e preserva o ficheiro na coleção. Torrents pessoais e transferências incompletas não são removidos.

Podes escolher entre 1 e 16 transferências simultâneas. Um limite maior permite mais transferências, mas não cria versões compatíveis quando elas não existem.

Se apagares um vídeo num disco ligado, o Yoru volta a reconhecer que falta. Se mudares o áudio de um anime, verifica as faixas declaradas dos ficheiros existentes e pode procurar uma edição adequada à nova preferência. Não apaga a edição anterior. Um idioma não declarado continua a aparecer como desconhecido e não conta como DUB inglês confirmado.

## Pesquisa, progresso e legendas

A pesquisa nativa funciona sem configuração adicional. O Yoru prepara Sonarr e Prowlarr em segundo plano quando o serviço de downloads está pronto. Não precisas de entrar nos painéis dessas aplicações. Em **Definições → Avançado → Pesquisa de episódios**, podes consultar o estado e abrir detalhes se houver um problema.

Para usar a pesquisa Sonarr num título cuja identidade não pôde ser confirmada automaticamente, abre **Rever a identificação de um anime**, procura o título e revê a numeração dos episódios. A pesquisa nativa continua disponível sem esta associação. Packs de temporadas e aquisição geral de séries TV ainda não estão incluídos nesta ponte.

Com AniList ligado, o progresso visto no perfil Jellyfin preparado nesta instalação é sincronizado automaticamente com o Yoru e o AniList. O PC e o Yoru têm de estar ligados. São contados episódios consecutivos confirmados; notas, estados e progresso superior são preservados. Outras alterações manuais à lista continuam disponíveis para revisão na página da conta.

No leitor do browser, as faixas ASS compatíveis oferecem **Estilo original ASS**, que preserva a apresentação da edição, e **Texto personalizável**, para escolher a tua apresentação. Se a renderização original falhar, o leitor regressa ao texto. Na televisão, os controlos de legendas são os da app Jellyfin.

## Atualizações

**Se tens 0.6.1–0.6.5:** descarrega **Yoru-Setup-0.6.7.exe** na [página de downloads](https://github.com/afonsohbamorim/yoru-releases/releases), abre-o e escolhe atualizar. Esta passagem precisa do instalador novo para renovar o sistema de arranque e recuperação. Não desinstales: as tuas contas, definições e vídeos ficam guardados.

Se tinhas escolhido outra pasta para o programa, usa **Alterar pastas** e seleciona essa mesma pasta da instalação anterior.

Em **Definições → Atualizações**, o Yoru avisa quando existe uma versão e trata do download e instalação após a tua escolha. Os leitores e serviços da primeira instalação mantêm as versões fixadas; esta versão ainda não atualiza esses componentes automaticamente.

## Desinstalar

O Yoru aparece nas **Aplicações instaladas** do Windows e no Painel de Controlo. Por omissão, a desinstalação preserva dados e vídeos. Podes escolher apagar os dados do Yoru e, separadamente, os vídeos geridos na pasta de dados. Vídeos externos ou desconhecidos são preservados. A janela mostra o âmbito antes de confirmar.

Este é um beta sem certificado Authenticode; o Windows pode mostrar um aviso de editor desconhecido. As atualizações são verificadas com assinatura Ed25519. A TV física e o Safari do destinatário precisam do primeiro teste no respetivo dispositivo.

Referências: [clientes Jellyfin](https://jellyfin.org/downloads/clients/all/), [Quick Connect](https://jellyfin.org/docs/general/server/quick-connect/), [compatibilidade de formatos](https://jellyfin.org/docs/general/clients/codec-support/).
