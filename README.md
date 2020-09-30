O que é o HTTP?

Quando se fala em HTTP, o primeiro pensamento que vem a nossa mente é sobre a utilização da 
internet, é o cenário onde vemos realmente na prática a utilização do HTTP. Nós acessamos 
sites em que seus endereços iniciam com http:// e por isso precisamos conhecer o que realmente 
está acontecendo ao fazer isso.
No momento em que acessou este curso, esta aula, entre o navegador e a Alura aconteceu 
uma comunicação, e esta comunicação tem duas partes bem conhecidas que chamamos de 
Client-Server ou em português Cliente-Servidor. Este é um modelo arquitetural, ou seja, a 
internet inteira é baseada nesta arquitetura onde há um cliente que solicita e um servidor que responde.

Cliente(Navegador como Chrome ou Firefox) -> Internet -> Servidor(Usando PHP, JAVA ou NET entre outros)

Em qualquer comunicação é preciso existir algumas regras para que as duas partes consigam se 
entender com sucesso. Pensando na comunicação do seu navegador entre a Alura ou algum outro 
site esse conjunto de regras é basicamente um protocolo, onde neste cenário é o HTTP.

Os protocolos são definidos, especificados e disponibilizados para implementação em 
ambas as partes, para consultar a especificação do HTTP, você pode utilizar o seguinte 
endereço: https://tools.ietf.org/html/rfc2616

Cliente(Navegador como Chrome ou Firefox) -> Regras de comunicação? -> Servidor(Usando PHP, JAVA ou NET entre outros)

`Resumindo:`
O HTTP é um protocolo que define as regras de comunicação entre cliente e servidor na internet.

`Exemplo:`
Cliente(Navegador como Chrome ou Firefox) -> HTTP(protocolo) -> Servidor(Usando PHP, JAVA ou NET entre outros)


01. O que é HTTP?
O que eu aprendi desse modulo:
- Na internet sempre tem um cliente e um servidor
- Entre o cliente e o servidor precisam haver regras de comunicação
- As regras são definidas dentro de um protocolo
- HTTP é o protocolo mais importante na internet

02. A Web segura - HTTPS
O que eu aprendi desse modulo:
- Por padrão, os dados são trafegados como texto puro na web.
- Apenas com HTTPS a Web é segura
- O protocolo HTTPS nada mais é do que o protocolo HTTP mais uma camada adicional de segurança, a TLS/SSL
- O tipo de criptografia de chave pública/chave privada
- O que são os certificados digitais
- Certificados possuem identidade e validade
- As chaves públicas estão no certificado, a chave privada fica apenas no servidor
- O que é uma autoridade certificadora
- O navegador utiliza a chave pública para criptografar os dados


03. Endereços sob seu domínio
O que eu aprendi desse modulo:
- URL são os endereços da Web
- Uma URL começa com o protocolo (por exemplo https://) seguido pelo domínio (www.alura.com.br)
- Depois do domínio pode vir a porta, se não for definida é utilizada a porta padrão desse protocolo
- Após o domínio:porta, é especificado o caminho para um recurso (/course/introducao-html-css)
- Um recurso é algo concreto na aplicação que queremos acessar


04. O cliente pede e o servidor responde
O que eu aprendi desse modulo:
- O protocolo HTTP segue o modelo Requisição-Resposta
- Sempre o cliente inicia a comunicação
- Uma requisição precisa ter todas as informações para o servidor gerar a resposta
- HTTP é stateless, não mantém informações entre requisições
- As plataformas de desenvolvimento usam sessões para guardar informações entre requisições