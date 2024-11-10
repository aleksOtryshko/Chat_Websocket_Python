# Chat_Websocket_Python

Чат-приложение
Это простое чат-приложение, использующее WebSockets для обмена сообщениями в реальном времени между несколькими клиентами. Приложение состоит из двух файлов:

server.py — серверный скрипт на Python, который управляет подключениями клиентов и транслирует сообщения.
client.html — клиентская веб-страница на HTML и JavaScript, которая позволяет пользователю отправлять и получать сообщения через WebSocket.
Описание работы приложения
Сервер
Серверный скрипт server.py запускает WebSocket сервер на локальной машине (localhost) и слушает порт 8765. Когда клиент подключается, сервер добавляет его в список активных подключений. Затем он передаёт все полученные сообщения от одного клиента остальным подключённым клиентам. Таким образом, каждое сообщение транслируется всем пользователям, кроме отправителя.

Клиент
client.html представляет собой веб-страницу с текстовым полем для ввода сообщений и кнопкой для отправки. Когда пользователь вводит сообщение и нажимает кнопку, оно отправляется на сервер через WebSocket. Все полученные сообщения отображаются на странице в реальном времени. Каждый клиент, подключённый к серверу, может отправлять и получать сообщения.

Запуск приложения
Скачайте или клонируйте проект.
Убедитесь, что у вас установлен Python 3.7 или выше.
Установите пакет websockets с помощью команды:
pip install websockets
Запустите сервер, выполнив команду:
python server.py
Откройте файл client.html в вашем веб-браузере. Вы можете открыть несколько вкладок с этим файлом, чтобы создать несколько клиентов.
Начните общение — вводите сообщения и отправляйте их. Все подключённые клиенты будут получать сообщения.





Chat Application
This is a simple real-time chat application using WebSockets for message exchange between multiple clients. The application consists of two files:

server.py — a Python server script that handles client connections and broadcasts messages.
client.html — a client-side webpage using HTML and JavaScript that allows users to send and receive messages via WebSocket.
How the Application Works
Server
The server script server.py runs a WebSocket server on the local machine (localhost) and listens on port 8765. When a client connects, the server adds it to the list of active connections. It then forwards any messages received from one client to the other connected clients. Thus, every message is broadcast to all users except the sender.

Client
The client.html file is a webpage with a text input field for entering messages and a button to send them. When the user types a message and presses the button, it is sent to the server via WebSocket. All received messages are displayed on the page in real-time. Each client connected to the server can send and receive messages.

Running the Application
Download or clone the project.
Ensure you have Python 3.7 or later installed.
Install the websockets package using the following command:
pip install websockets
Run the server by executing:
python server.py
Open the client.html file in your web browser. You can open multiple tabs with this file to simulate multiple clients.
Start chatting — type messages and send them. All connected clients will receive the messages.

