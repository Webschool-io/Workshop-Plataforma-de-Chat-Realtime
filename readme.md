# Workshop sobre Realtime, Desktop e Bots com Node.js

Nesse workshop modular iremos aprender a criar uma plataforma de chat, com bots, chamadas de vídeo e áudio, e rodando no desktop além da web!

Esse workshop será dividido em 4 módulos:

- Socket.io - 5 horas
- Bots - 10 horas
- Electron - 5 horas
- WebRTC - 10 horas

## A Ideia

Você não irá aprender a criar apenas um sisteminha de chat básico, irá aprender a construir uma plataforma de chat com diversas funcionalidades que ainda não encontramos nos sistemas mais usados como: WhatsApp, Telegram, etc.

Uma das funcionalidades que acredito ser mais interessante é a possibilidade de fazer video/audio chamadas, além disso poder gravar localmente essa chamada.

Outra funcionalidade que acho maravilhosa é poder receber 1 áudio e em vez de ouvi-lo que o sistema converta em texto, caso eu não deseje ouvir e sim apenas ler. Além disso será integrado um sistema de tradução.

*ps: esse sistema será utilizado no nosso EAD.*

Primeiramente vamos definir as ações possíveis na plataforma:

- adicionar amigo via nick/username do github;
- criar chat privado com qualquer um;
- criar chats públicos e privados;
    + todos possuindo uma rota única para poder ser acessado
- criar canal de notícias onde é apenas para leitura;
- criar video/audioconferência particular;
- criar video/audioconferência em grupo;
- gravar as chamadas de video/audio;
- compartilhar arquivos;
- compartilhar desktop;
- criar, executar e gerenciar bots;
- transcrição de áudio para texto;
    + e posterior tradução;
- utilizar o sistema tanto web como desktop e quem sabe mobile também.

## Aulas

> **As aulas serão feitas ao vivo!**

Utilizaremos o Hangouts para as aulas, logo cada turma poderá ter **no máximo 9 alunos**, pois ele só aceita até 10 usuários para que seja fechado.

Teremos duas formas de turmas:

- dia de semana
- final de semana

### Aulas de dia de semana

As aulas serão de Segunda a Sexta-feira sendo de 1 a 2 horas por dia, dependendo da turma.

O horário de início será as 22 horas, mas poderá ser modificado mediante pedido da turma.

### Aulas de final de semana

As aulas serão Sábado e Domingo sendo 5 horas máximas, por dia.

O horário de início será as 14 horas, mas poderá ser modificado mediante pedido da turma.


## Custo

Eu gostaria muitooooo de fazer todo esse workshop free, mas infelizmente estou criando todo esse conteúdo **único como workshop** para que eu consiga pagar minhas contas atrasadas e atuais, para que aí sim eu possa liberar TODO esse conteúdo FREE!

> O custo será de R$100 por cada 5 horas de workshop independente do módulo escolhido!

Creio que R$20 por hora, de um workshop inédito e que ainda irá contribuir com quem não tem como pagar, é bem razoável.

Como o módulo de WebRTC não serei eu que farei, contarei como meta apenas os outros módulos, preciso alcançar um montante de R$8000. Após alcançar essa meta todos os vídeos gravados durante as aulas serão liberados no nosso [canal do Youtube]().

Espero que me entendam por eu estar cobrando por esse workshop, pois infelizmente se eu só der aulas de graça não consigo pagar minhas contas atuais, logo não tenho nem cabeça de criar mais materiais gratuitos.

Essa é uma forma dos alunos que já me ajudam doando para o [Be MEAN]() que possam agora direcionar suas doações para esse workshop que por tabela estará me ajudando e muitooooooo!


## Realtime

Esse módulo engloba 2 sub-módulos:

- Socket.io
- WebRTC

Iniciando com o módulo de Socket.io para criamos a plataforma de chat utilizando Express.

Com o Socket.io iremos criar o chat, grupos e a interação entre os usuários.

### Socket.io - 5 horas

As funcionalidades a serem desenvolvidas nesse módulo são:

- criação de grupos com várias pessoas
- criação de chat individual
- envio de mensagem para algumas pessoas escolhidas
- mostrar quando a pessoa estiver digitando
- mostrar ícone de envio de mensagem
- mostrar ícone de recebimento de mensagem
- mostrar ícone de leitura de mensagem

### WebRTC

Funcionalidades:

- criar video/audioconferência particular;
- criar video/audioconferência em grupo;
- gravar as chamadas de video/audio;
- compartilhar arquivos;
- compartilhar desktop;
- desenho colaborativvo;
    + propósitos educacionais;
- transcrição de áudio para texto;
    + e posterior tradução;
- barra de UserMedia personalizada.


Mais links: 

- Desenho em canvas: https://github.com/muaz-khan/Canvas-Designer
- Compartilhar desktop: https://www.webrtc-experiment.com/RTCMultiConnection/screen-sharing.html
- barra de UserMedia personalizada: https://www.webrtc-experiment.com/navigator.customGetUserMediaBar/
- Tradução de fala e texto: https://github.com/muaz-khan/Translator
- Gravação: https://github.com/muaz-khan/RecordRTC
    + https://github.com/muaz-khan/Ffmpeg.js
    + https://4dbefa02675a4cdb7fc25d009516b060a84a3b4b.googledrive.com/host/0B6GWd_dUUTT8WjhzNlloZmZtdzA/ffmpeg_asm.js
- Compartilhamento de arquivos: https://github.com/muaz-khan/RTCMultiConnection/blob/master/demos/file-sharing.html
    + https://www.webrtc-experiment.com/RTCMultiConnection/audio-conferencing-data-sharing.html
- Com Socket.io: https://github.com/muaz-khan/RTCMultiConnection/blob/master/v2.2.2/demos/socketio-auto-open-join-room.html


- https://www.webrtc-experiment.com/RTCMultiConnection/
- https://www.webrtc-experiment.com/Conversationjs/


## Bots - 10 horas

Nesse módulo não aprenderemos apenas a criar apenas um bot, mas sim criar uma plataforma que execute bots assim como o Telegram, Slack e cia fazem. Porém para isso iremos inicialmente criar 1 bot para o Telegram para entendermos o que e como 1 bot deve se comportar para depois aplicarmos as mesmas funcionalidades na nossa plataforma.


### Eventos

#### API

Para criar nossa API de eventos para nossos bots iremos nos basear na do [Slack](https://api.slack.com/events/api) e Telegram.


- channel_created
- channel_deleted
- channel_joined
- group_close
- group_open
- im_close
- im_created
- im_open
- message.channels
- message.groups
- message.im
- message.mpim

Funcionalidades para o projeto final:

- reaction_added
- reaction_removed
- subteam_created
- team_domain_change
- team_join
- team_rename