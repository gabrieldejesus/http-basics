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
**Cliente** (navegador como Chrome ou Firefox) -> **HTTP (protocolo)** -> **Servidor** (usando PHP, JAVA ou NET entre outros)

---

## 💡 Vamos Além

### 🧭 Uma visão geral do HTTP

✔️ Na internet sempre existe um cliente e um servidor

✔️ Deve haver regras de comunicação entre o cliente e o servidor

✔️ As regras são definidas dentro de um protocolo

✔️ HTTP é o protocolo mais importante da internet

---

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

---

### 🌐 Endereços em seu domínio

✔️ URL são os endereços da web

✔️ Um URL começa com o protocolo (por exemplo https: //) seguido pelo domínio (https://github.com)

✔️ Depois que o domínio pode vir a porta, se não estiver definida, a porta padrão deste protocolo é usada

✔️ Após o domínio: porta, o caminho para um recurso é especificado (/ devgabrieldejesus / http-basics)

✔️ Um recurso é algo concreto no aplicativo que queremos acessar

---

### 📢 O cliente pergunta e o servidor responde

✔️ O protocolo HTTP segue o modelo Solicitação-Resposta

A comunicação realizada pelo HTTP segue o modelo cliente-servidor, baseando-se nos conceitos de request (pedido) e response (resposta). Um request corresponde a um pedido feito ao servidor. Uma mensagem de requisição do cliente é composta pelos seguintes campos de maneira geral:

- Linha de pedido: formada pelo identificador do método HTTP (GET, POST, PUT, DELETE, etc.), URI do recurso (endereço para o qual será enviado o pedido) e versão do protocolo (geralmente, HTTP 1.1 e HTTP 2);

- Cabeçalho: contém meta-informações sobre a requisição, como a identificação do cliente que está fazendo o pedido;

- Corpo: contém os dados da requisição.

Já o response corresponde à resposta que é enviada pelo servidor. Geralmente, ele é composto dos seguintes componentes:

- Linha de status: contém informações como a versão do protocolo utilizado no servidor, código numérico do status da resposta e o texto associado ao status;

- Cabeçalho: é bem similar ao cabeçalho do pedido, ou seja, contém meta-informações e informações adicionais sobre o seu pedido e conteúdo de resposta;

- Corpo: conteúdo de resposta para a requisição realizada (no caso de acesso a um site, seria o HTML para que o browser renderize a página, por exemplo).

De fato, essa comunicação baseada nesse modelo cliente/servidor é extremamente rápida e eficiente. Porém, existe um problema grande: toda essa comunicação que ocorre através do protocolo HTTP é baseada em texto puro, o que é completamente inseguro. E aqui entra o HTTPS.

✔️ Sempre é o cliente que inicia a comunicação

✔️ Um pedido deve ter todas as informações para o servidor gerar a resposta

✔️ HTTP não tem estado, não guarda informações entre as solicitações

Cada página visitada gera um novo par de requisição/resposta), duas estratégias podem ser usadas, já que o HTTP por si só, não permite guardar o estado das requisições e respostas:

- Você possui um cadastro no site e um programa escrito no servidor é responsável por armazenar suas informações ; ou

- Um programa escrito em linguagem cliente (como JavaScript), gerencia essas informações através dos cookies e de bancos de dados que os próprios navegadores disponibilizam para as aplicações, para armazenamento temporário dessas informações.

---

### 🛠 Depurando a solicitação HTPP

✔️ Cabeçalho de resposta

- Os cabeçalhos HTTP permitem que o cliente e o servidor passem informações adicionais com uma solicitação ou resposta HTTP. Um cabeçalho HTTP consiste em seu nome que não diferencia maiúsculas de minúsculas, seguido por dois pontos (:) e, a seguir, por seu valor. O espaço em branco antes do valor é ignorado.

✔️ Códigos de resposta (código de status)

- Os códigos de status das respostas HTTP indicam se uma requisição HTTP foi corretamente concluída. As respostas são agrupadas em cinco classes:

1. Respostas de informação (100-199),
2. Respostas de sucesso (200-299),
3. Redirecionamentos (300-399)
4. Erros do cliente (400-499)
5. Erros do servidor (500-599).

---

### 🧱 Parâmetros de solicitação

Usado para definir os detalhes da pesquisa ou enviar dados do formulário

✔️ GET: Receber dados (Os parâmetros são enviados na própria URL (usando [?] E concatenando com [&])
- O método GET solicita a representação de um recurso específico. Requisições utilizando o método GET devem retornar apenas dados.
 
✔️ POST: Enviar dados (Parâmetros no corpo da solicitação)
- O método POST é utilizado para submeter uma entidade a um recurso específico, frequentemente causando uma mudança no estado do recurso ou efeitos colaterais no servidor.

✔️ DELETE: Remover um recurso
- O método DELETE remove um recurso específico.

✔️ PUT / PATCH: Atualizar um recurso
- O método PUT substitui todas as atuais representações do recurso de destino pela carga de dados da requisição.

---

### ⚙️ Serviços da Web com REST

✔️ REST é um padrão arquitetônico para comunicações entre aplicativos

- É um conjunto de princípios de arquitetura que atende às necessidades de aplicações mobile e serviços web leves. Como se trata de um grupo de diretrizes, são os desenvolvedores que precisam implementar essas recomendações.

✔️ Os recursos são definidos via URI

- Um URI (Identificador de recursos uniforme) é uma sequência de caracteres utilizados para identificar um recurso lógico ou físico, geralmente, na internet. O URI descreve os mecanismos para acessar um recurso, os computadores nos quais os recursos estão hospedados e os nomes dos recursos em cada computador. 

---

### 💡 Para saber mais: tipos de dados

Em alguns cabeçalhos HTTP, devemos especificar algum formato. Os formatos são chamados na documentação dos tipos MIME. E na definição do cabeçalho usamos a seguinte estrutura: tipo / subtipo. Os tipos conhecidos são:

```sh 
texto, imagem, aplicativo, áudio e vídeo
```

E alguns subtipos:

```sh
text -> text / plain, text / html, text / css, text / javascript
```
```sh
Imagem -> imagem / gif, imagem / png, imagem / jpeg
```
```sh
Audio -> audio / midi, audio / mpeg, audio / webm, audio / ogg, audio / wav
```

```sh
video -> video / mp4
```

```sh
Application -> application / xml, application / pdf
```

```sh
Outros formatos aceitos: https: // developer.mozilla.org / en-US / docs / Web / HTTP / Basics_of_HTTP / MIME_types
```

---

### 🔑 HTTP 2 - Para uma web mais eficiente

HTTP 2 (originalmente chamado de HTTP/2.0) é uma revisão importante do protocolo de rede HTTP usado pela World Wide Web. Ele foi derivado do protocolo SPDY experimental anterior, originalmente desenvolvido pelo Google.

HTTP 2 foi desenvolvido pelo Grupo de Trabalho HTTP (também chamado de httpbis, onde "bis" significa "segundo") da Força-Tarefa de Engenharia da Internet.

HTTP 2 é a primeira nova versão de HTTP desde HTTP 1.1, padronizado no RFC 2068 em 1997.

O Grupo de Trabalho submeteu HTTP 2 ao IESG para consideração como um padrão proposto em dezembro de 2014, e o IESG aprovou a publicação como um padrão proposto em 17 de fevereiro de 2015.

A especificação HTTP 2 foi publicada como RFC 7540 em 14 de maio de 2015.

---

### 💡 Um pouco sobre HTTP2

✔️ Atua sobre o que já se conhece de HTTP

⏳ Cabeçalhos binários e de tablet (HPACK)
> (explicação em breve)

⏳ GZIP padrão em resposta
> (explicação em breve)

⏳ Multiplexação (solicitação e respostas são paralelas)
> (explicação em breve)

⏳ Cabeçalhos úteis (apenas enviamos cabeçalhos que mudam)
> (explicação em breve)

⏳ Serve-Push (ato do servidor enviar dados sem que o navegador tenha solicitado)
> (explicação em breve)

---

## 🗃 Histórico de lançamento

* 0.1.0
    * Estudando a possibilidade de adicionar novos conteúdos

* 0.0.1
    * Trabalho em progresso

## 📝 Meta

Gabriel de Jesus - [Meu Portfólio](https://www.gabrieldesenvolvedor.com/) - oi@gabrieldesenvolvedor.com

Distribuído sob a licença MIT. Veja `LICENSE` para mais informações.

[https://github.com/devgabrieldejesus/http-basics](https://github.com/devgabrieldejesus/)

## 🚀 Contribuição

1. Fork em (<https://github.com/devgabrieldejesus/http-basics/fork>)
2. Crie seu branch de recurso (`git checkout -b feature / fooBar`)
3. Faça commit de suas alterações (`git commit -am 'Add some fooBar'`)
4. Empurre para o branch (`git push origin feature / fooBar`)
5. Crie uma nova solicitação pull
