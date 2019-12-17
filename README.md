# Api Mutante
Determina si la cadena de Adn pasado como requestBody (json) corresponde a un humano mutante. 
Se debe ejecutar un POST con body del tipo json en el cual se debe informar la cadena a validar.
El HttpsStatus del response determina:

400 BAD_REQUEST: En caso de cadena de adn incorrecta (no cumple con las condiciones del ejercicio, por ej no es nxn o tiene algún caracter incorrecto.

200 OK:Cadena de ADN correcta y corresponde a un humano mutante

403 FORBIDDEN: Cadena de ADN correcta y corresponde a un humano no mutante

ACCESOS:
Api pública (google cloud): 
http://35.232.238.121/mutant

Para ejecutar en entorno local, bajar el repo y ejecutar comando gradle bootRun (dentro del task application):
levanta en http://localhost:8080/mutant

Para determinar si el servicio se encuentra levantado ejecutar un GET a URL_BASE/actuator/health, cuando se encuentra levantado responde OK (HTTPSTATUS 200 ) y  cuerpo 
{
	"status": "UP"
}
