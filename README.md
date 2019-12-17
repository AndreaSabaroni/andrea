# Api Mutante
Acceso a Api en kubernetes: http://35.232.238.121/mutant

Para ejecutar local:
http://localhost:8080/mutant

HTTP STATUS como RESPUESTA:
400 BAD_REQUEST: En caso de cadena de adn incorrecta 
200 OK:Cadena de ADN correcta y corresponde a un humano mutante
403 FORBIDDEN: Cadena de ADN correcta y corresponde a un humano no mutante
