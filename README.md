PHP-and-WebSocket-demo
======================
前言：由于公司要做网页交互的广告类的小游戏，所以顺便学习一下以前看的webSocket

======================
+ 客户端
//create a new WebSocket object.
websocket = new WebSocket("ws://localhost:9000/daemon.php"); 
websocket.onopen = function(evt) { /* do stuff */ }; //on open event
websocket.onclose = function(evt) { /* do stuff */ }; //on close event
websocket.onmessage = function(evt) { /* do stuff */ }; //on message event
websocket.onerror = function(evt) { /* do stuff */ }; //on error event
websocket.send(message); //send method
websocket.close(); //close method

+服务端
//Create TCP/IP sream socket and return the socket resource
$socket = socket_create(AF_INET, SOCK_STREAM, SOL_TCP);

// Bind the source address
socket_bind($socket, 'localhost');

// Bind the source address
socket_bind($socket, 'localhost');

PHP 和 websocket 演示样品
