# Yoru para Windows

Anime e séries, ao teu ritmo. O Yoru reúne descoberta, biblioteca, episódios e reprodução numa interface local.

Este repositório é o canal de instaladores e atualizações. A versão 0.6.0 está em revisão privada; ainda não existe uma release pública.

## Instalação

1. Descarrega `Yoru-Setup-0.6.0.exe` na release aprovada e abre o ficheiro no Windows 10/11 de 64 bits.
2. Escolhe pastas vazias e separadas para a aplicação e os teus dados.
3. Abre o atalho Yoru e segue a preparação inicial. Cria a tua conta local e liga as tuas próprias contas, se quiseres.

O instalador inclui Jellyfin/FFmpeg, MPV, MPC-HC, qBittorrent e o runtime necessário. Não precisas de instalar codecs, Node ou players à parte. Não inclui vídeos, contas ou bibliotecas de outra pessoa. Os dados ficam na pasta que escolheste.

A bandeja permite abrir o Yoru, ativar o início com Windows ou encerrar os serviços desta instalação. Iniciar com Windows é opcional. A obtenção automática de episódios começa desativada.

## Atualizações

O Yoru verifica novas versões automaticamente. Descarregar e instalar exige confirmação na aplicação; uma sessão de reprodução impede a atualização. O atualizador verifica a assinatura e os ficheiros e recupera a versão anterior se a nova falhar na validação.

Nesta primeira versão, o atualizador cobre o Yoru, o seu runtime e os players. Jellyfin e qBittorrent permanecem na versão base da instalação. O feed só funciona depois de existir uma release publicada e acessível.

## Ver na TV

O PC funciona como servidor e tem de estar ligado durante a reprodução. O primeiro percurso usa a aplicação Jellyfin da TV, ligada ao servidor pela rede de casa. Existem [clientes oficiais para Android TV/Fire TV e LG webOS](https://jellyfin.org/downloads/clients/all/); a compatibilidade depende do modelo. A validação numa TV física ainda está pendente.

## Sobre o beta

A obtenção de todos os episódios confirma primeiro quais foram emitidos, as duplicações e o espaço estimado. A aplicação procura depois uma edição adequada por episódio, respeitando os limites de armazenamento e simultaneidade.

O AniList pode ficar indisponível: a biblioteca e os detalhes guardados continuam visíveis, mas dados antigos não autorizam novos episódios. O envio automático do progresso do player para AniList e a obtenção de séries ainda não estão incluídos.

As atualizações têm assinatura Ed25519. Este instalador beta ainda não tem assinatura de editor Windows (Authenticode). As licenças e os avisos dos componentes incluídos acompanham o pacote.
