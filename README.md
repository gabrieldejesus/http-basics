![](images/cover.png)

## O que é HTTP?

Quando se trata de HTTP, o primeiro pensamento que vem à mente é sobre como usar internet, é o cenário onde realmente vemos o uso do HTTP na prática. Nós acessamos sites onde seus endereços começam com http: // e, portanto, precisamos saber o que realmente está acontecendo ao fazer isso.

No momento em que você acessou este repositório, entre o navegador e o GitHub aconteceu uma comunicação, e essa comunicação tem duas partes bem conhecidas que chamamos
*client-server* ou em Português *Cliente-Servidor*.

Toda a internet é baseada nesta arquitetura onde há um cliente que solicita e um servidor que responde.

### Exemplo:
**Cliente** (navegador como Chrome ou Firefox) -> **Internet** -> **Servidor** (usando PHP, JAVA ou NET entre outros)

Como em qualquer comunicação. devesse haver algumas regras para que as duas partes possam se entender com sucesso. 
Pensando na comunicação do seu navegador com o Git ou algum outro site este conjunto de regras é basicamente um protocolo, onde neste cenário é HTTP.

Os protocolos são definidos, especificados e disponibilizados para implementação em ambas as partes, para consultar a especificação HTTP, você pode usar o seguinte
endereço: https://tools.ietf.org/html/rfc2616

### Exemplo:
**Cliente** (navegador como Chrome ou Firefox) -> **Regras de comunicação?** -> **Servidor** (usando PHP, JAVA ou NET entre outros)

### Resumindo:
HTTP é um protocolo que define as regras de comunicação entre cliente e servidor na internet.

### Exemplo:
**Cliente** (navegador como Chrome ou Firefox) -> **HTTP (protocolo)** -> **Servidor** (usando PHP, JAVA ou NET entre outros) *

***

## 💡 Vamos Além

### 🧭 Uma visão geral do HTTP

✔️ Na internet sempre existe um cliente e um servidor

✔️ Deve haver regras de comunicação entre o cliente e o servidor

✔️ As regras são definidas dentro de um protocolo

✔️ HTTP é o protocolo mais importante da internet


### 🔐 A web segura - HTTPS

✔️ Por padrão, os dados são trafegados como texto simples na web.

✔️ Somente com HTTPS a web é segura

✔️ O protocolo HTTPS nada mais é do que o protocolo HTTP mais uma camada adicional de segurança, **TLS / SSL**

✔️ O tipo de criptografia de chave pública / chave privada

- A criptografia de chaves pública e privada utiliza duas chaves distintas, uma para codificar e outra para decodificar mensagens. Neste método cada pessoa ou entidade mantém duas chaves: uma pública, que pode ser divulgada livremente, e outra privada, que deve ser mantida em segredo pelo seu dono. As mensagens codificadas com a chave pública só podem ser decodificadas com a chave privada correspondente. 

✔️ O que são certificados digitais?

- O SSL é a abreviação de “Secure Sockets Layer” e os certificados SSL são utilizados para proteger as comunicações entre um site, host ou servidor e os usuários finais que estão se conectando a ele (ou entre duas máquinas em um relacionamento cliente-servidor).

✔️ Os certificados têm identidade e validade

✔️ As chaves públicas estão no certificado, a chave privada está apenas no servidor

- A criptografia de chaves pública e privada utiliza duas chaves distintas, uma para codificar e outra para decodificar mensagens. Neste método cada pessoa ou entidade mantém duas chaves: uma pública, que pode ser divulgada livremente, e outra privada, que deve ser mantida em segredo pelo seu dono. As mensagens codificadas com a chave pública só podem ser decodificadas com a chave privada correspondente.

✔️ O que é uma autoridade de certificação?

A autoridade de certificação (CA), também conhecido como um Autoridade de Certificação, é uma empresa ou organização que atua para validar as identidades de entidades (como sites, endereços de email, empresas ou pessoas físicas) e vinculá-las a chaves criptográficas através da emissão de documentos eletrônicos conhecidos como certificados digitais. Um certificado digital fornece:

- Autenticação, servindo como credencial para validar a identidade da entidade para a qual é emitida.

- Criptografia, para comunicação segura em redes inseguras, como a Internet.

- Integridade de documentos assinado com o certificado para que não possam ser alterados por terceiros em trânsito.


⏳ O navegador usa a chave pública para criptografar os dados?
> (explicação em breve)


### 🌐 Endereços em seu domínio

✔️ URL são os endereços da web

✔️ Um URL começa com o protocolo (por exemplo https: //) seguido pelo domínio (https://github.com)

✔️ Depois que o domínio pode vir a porta, se não estiver definida, a porta padrão deste protocolo é usada

✔️ Após o domínio: porta, o caminho para um recurso é especificado (/ devgabrieldejesus / http-basics)

✔️ Um recurso é algo concreto no aplicativo que queremos acessar


### 📢 O cliente pergunta e o servidor responde

⏳ O protocolo HTTP segue o modelo Solicitação-Resposta
> (explicação em breve)

✔️ Sempre é o cliente inicia a comunicação

✔️ Um pedido deve ter todas as informações para o servidor gerar a resposta

⏳ HTTP não tem estado, não guarda informações entre as solicitações
> (explicação em breve)

⏳ As plataformas de desenvolvimento usam sessões para armazenar informações entre as solicitações
> (explicação em breve)

### 🛠 Depurando a solicitação HTPP

⏳ Console de depuração
> (explicação em breve)

⏳ Método HTTP GET
> (explicação em breve)

⏳ Cabeçalho de resposta
> (explicação em breve)

⏳ Códigos de resposta (código de status)
> (explicação em breve)

### 🧱 Parâmetros de solicitação

✔️ Usado para definir os detalhes da pesquisa ou enviar dados do formulário

⏳ GET: os parâmetros são enviados na própria URL (usando [?] E concatenando com [&])
> (explicação em breve)

⏳ POST: os parâmetros são enviados no corpo da solicitação
> (explicação em breve)

⏳ HTTP️ Existem outros métodos HTTP como POST, DELETE, PUT
> (explicação em breve)

Resumo

⏳ OBTER: Receber dados (Parâmetros na URL)
> (explicação em breve)
 
⏳ POST: Enviar dados (parâmetros no corpo da solicitação)
> (explicação em breve)

⏳ DELETE: Remover um recurso
> (explicação em breve)
 
⏳ PUT / PATCH: Atualizar um recurso
> (explicação em breve)

### 07. Serviços da Web com REST

⏳ REST é um padrão arquitetônico para comunicações entre aplicativos
> (explicação em breve)

⏳ Aproveita a estrutura HTTP
> (explicação em breve)

⏳ Os recursos são definidos via URI
> (explicação em breve)

⏳ Operações com métodos HTTP (GET / POST / PUT / DELETE)
> (explicação em breve)

⏳ Cabeçalhos (Aceitar / Tipo de Conteúdo) são usados para especificar representações (JSON, XML, ...)
> (explicação em breve)

### 💡 Para saber mais: tipos de dados

Em alguns cabeçalhos HTTP, devemos especificar algum formato. Os formatos são chamados na documentação dos tipos MIME. E na definição do cabeçalho usamos a seguinte estrutura: tipo / subtipo. Os tipos conhecidos são:

`texto, imagem, aplicativo, áudio e vídeo`

E alguns subtipos:

`text -> text / plain, text / html, text / css, text / javascript`

ʻImagem -> imagem / gif, imagem / png, imagem / jpeg`

ʻAudio -> audio / midi, audio / mpeg, audio / webm, audio / ogg, audio / wav`

`video -> video / mp4`

ʻApplication -> application / xml, application / pdf`

ʻOutros formatos aceitos: https: // developer.mozilla.org / en-US / docs / Web / HTTP / Basics_of_HTTP / MIME_types`

### 🔑 HTTP2 - Para uma web mais eficiente

HTTP / 2 (originalmente chamado de HTTP / 2.0) é uma revisão importante do protocolo de rede HTTP usado pela World Wide Web. Ele foi derivado do protocolo SPDY experimental anterior, originalmente desenvolvido pelo Google.
HTTP / 2 foi desenvolvido pelo Grupo de Trabalho HTTP (também chamado de httpbis, onde "bis" significa "segundo") da Força-Tarefa de Engenharia da Internet.
HTTP / 2 é a primeira nova versão de HTTP desde HTTP 1.1, padronizado no RFC 2068 em 1997.
O Grupo de Trabalho submeteu HTTP / 2 ao IESG para consideração como um padrão proposto em dezembro de 2014, e o IESG aprovou a publicação como um padrão proposto em 17 de fevereiro de 2015.
A especificação HTTP / 2 foi publicada como RFC 7540 em 14 de maio de 2015.

### 💡 Um pouco sobre HTTP2

↪️ Atua sobre o que já se conhece de HTTP

↪️ Cabeçalhos binários e de tablet (HPACK)

↪️ GZIP padrão em resposta

↪️ Multiplexação (solicitação e respostas são paralelas)

↪️ Cabeçalhos úteis (apenas enviamos cabeçalhos que mudam)

↪️ Serve-Push (ato do servidor enviar dados sem que o navegador tenha solicitado)
