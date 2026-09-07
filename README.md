# Yoru para Windows

[**Descarregar Yoru para Windows**](https://github.com/afonsohbamorim/yoru-releases/releases)

Anime e séries, do teu PC à TV.

## No PC Windows

1. Descarrega o ficheiro **Yoru-Setup-…exe** da versão mais recente na [página de downloads](https://github.com/afonsohbamorim/yoru-releases/releases/latest).
2. Abre e carrega em **Instalar**. As pastas sugeridas servem; podes alterá-las. A primeira abertura precisa de Internet e prepara automaticamente os leitores e serviços.
3. O Yoru abre no browser. Escolhe onde guardar os vídeos e cria o perfil de reprodução. Liga o AniList se quiseres trazer a tua lista.

O ícone Yoru junto ao relógio indica que o serviço está aberto. Podes abrir a interface, escolher **Iniciar com Windows** ou **Sair**. Fechar a página do browser mantém o serviço aberto.

Não precisas de instalar Node, codecs, MPV, MPC-HC, Jellyfin ou qBittorrent à mão. Cada pessoa tem as suas próprias contas e ficheiros. O programa fica na pasta da aplicação; os vídeos podem ficar noutro disco escolhido no Yoru.

## Na TV

No PC, abre **Definições → Dispositivos → Preparar ligação à TV** e aceita o pedido do Windows. Instala a app **Jellyfin** na loja da TV. Android/Google TV e LG webOS têm clientes nativos; a disponibilidade depende do modelo e da loja.

Dentro da app Jellyfin, introduz o endereço que o Yoru mostra. É a ligação inicial ao servidor do PC; a app guarda-o. No login, escolhe **Quick Connect** e escreve no Yoru o código apresentado na TV. Também podes entrar com o perfil de reprodução criado no PC.

Depois, abres a app da TV e escolhes os vídeos. O PC tem de estar ligado, com sessão Windows iniciada e o Yoru aberto. Ambos os dispositivos têm de estar na mesma rede de casa. Se o router mudar o endereço do PC, atualiza o servidor guardado na TV.

## No MacBook

Não instales o servidor no Mac. No PC, abre **Definições → Dispositivos**, ativa o acesso pelo browser e gera um código de emparelhamento. No Safari do Mac, abre o endereço **Yoru** apresentado nessa secção e introduz o código. Usa **Disponíveis** para ver a mesma coleção e continuar os episódios.

O endereço Yoru é diferente do endereço Jellyfin da TV. `localhost` no Mac aponta para o Mac, por isso deves usar o endereço do PC. Chrome não é obrigatório. A reprodução e eventual conversão dependem do formato do vídeo e do Mac.

Depois de ligado, o dispositivo fica autorizado até revogares o acesso. Não precisas de renovar semanalmente. Se apagares os dados do browser ou usares navegação privada, poderás precisar de o ligar novamente. Os dispositivos autorizados numa versão antiga têm a opção **Manter autorizado** no PC.

## Obter episódios e atualizar

Na ficha de um anime, escolhe o áudio e o que queres guardar. **Descarregar episódios disponíveis** permite rever todos os emitidos ou os não vistos, confirmar o espaço e iniciar o lote. Os episódios só aparecem em **Disponíveis** depois de concluídos e verificados. Um lote pode esperar por uma edição que cumpra o perfil; a espera tem um motivo visível.

Nas instalações novas, a aquisição automática de planos começa desligada. Ativa-a em **Episódios** para acompanhar a fila. A qualidade, o espaço e a identificação do episódio são sempre verificados antes de iniciar uma transferência.

Podes escolher entre 1 e 16 transferências simultâneas. Um limite maior permite mais transferências, mas não cria versões compatíveis quando elas não existem.

Em **Definições → Atualizações**, o Yoru avisa quando existe uma versão e trata do download e instalação após a tua escolha. Os leitores e serviços da primeira instalação mantêm as versões fixadas; esta versão ainda não atualiza esses componentes automaticamente.

## Desinstalar

O Yoru aparece nas **Aplicações instaladas** do Windows e no Painel de Controlo. Por omissão, a desinstalação preserva dados e vídeos. Podes escolher apagar os dados do Yoru e, separadamente, os vídeos geridos na pasta de dados. Vídeos externos ou desconhecidos são preservados. A janela mostra o âmbito antes de confirmar.

Este é um beta sem certificado Authenticode; o Windows pode mostrar um aviso de editor desconhecido. As atualizações são verificadas com assinatura Ed25519. A TV física e o Safari do destinatário precisam do primeiro teste no respetivo dispositivo.

Referências: [clientes Jellyfin](https://jellyfin.org/downloads/clients/all/), [Quick Connect](https://jellyfin.org/docs/general/server/quick-connect/), [compatibilidade de formatos](https://jellyfin.org/docs/general/clients/codec-support/).
