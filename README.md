# WebSocket Chat App

Este é um projeto de exemplo que demonstra como criar um aplicativo de chat em tempo real usando Spring WebSocket.

## Visão Geral

Este projeto implementa um aplicativo de chat usando o protocolo WebSocket e o framework Spring. Ele permite que os usuários se conectem a uma sala de chat em tempo real, enviem mensagens, entrem e saiam da sala.

## Pré-requisitos

- Java JDK 17 ou superior.
- Maven para construção e gerenciamento de dependências.

## Configuração

- Clone o repositório:
```sh
git clone https://github.com/luckraw/websocket-chat.git
```
- Configure as Dependências:

O arquivo pom.xml contém as dependências do projeto, incluindo o Spring Boot, Spring WebSocket e Lombok.
Execute o aplicativo:


## Uso

- Acesse o aplicativo em seu navegador: `http://localhost:8080`.
- Insira um nome de usuário para entrar na sala de chat.
- Envie mensagens para a sala de chat.

## Estrutura do Projeto

`ChatMessage.java` : Classe de modelo que representa uma mensagem de chat.

`ChatController.java` : Controlador que gerencia o envio de mensagens e adição de usuários.

`MessageType.java` : Enumeração que define os tipos de mensagem.

`WebSocketConfig.java` : Configuração do WebSocket.

`WebSocketEventListener.java` : Ouvinte de eventos WebSocket para tratar desconexões.

## Rotas
O projeto utiliza as seguintes rotas:

`/ws` : O ponto de extremidade WebSocket para comunicação em tempo real.

`/app/chat.sendMessage` : Rota para enviar mensagens de chat.

`/app/chat.addUser` : Rota para adicionar um usuário à sala de chat.

`/topic/public` : Canal de tópico para enviar mensagens para todos os usuários na sala.

### Contribuição

Se você quiser contribuir para este projeto, siga estas etapas:

- Faça um fork do projeto.
- Crie uma branch para sua feature `(git checkout -b feature/SuaFeature)`.
- Faça commit das suas mudanças `(git commit -m 'Adicionar alguma funcionalidade')`.
- Envie para o branch (git push origin feature/SuaFeature).
- Crie um novo Pull Request.
