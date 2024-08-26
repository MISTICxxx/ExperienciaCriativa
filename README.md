# ExperienciaCriativa
inicializei os servos em 80 para ficar visualmente mais bonito, o servo 1 vai de 80 a 130 para ser os 50 graus pedidos no exercicio, ja o servo 2 vai de 80 a 180, pois ele nao vai ate 260.
em todo caso, o codigo funciona basicamente com as conexoes no mqtt e no wifi do proprio wokwi, tem a declaracao dos pinos e dos pwm para fazer algumas coisas funcionarem como o servo motor e o buzzer da esp2
caso a temperatura suba para acima de 60 graus, ele liga determinado servo motor e abre a comporta, se os dois estiverem acima de 60, abre os dois.
caso a umidade de qualquer um dos dois caia para menos de 20%, envia uma mensagem a esp2
a esp2 esta o tempo todo lendo as mensagens enviadas, e caso leia que a umidade esta baixa, pisca o led a cada 1 segundo e liga o buzzer ate que a umidade suba novamente ou liguemos o switch da esp2 para parar o alarme
caso liguemos o switch da esp1, os servo motores voltam a posicao original e para de enviar mensagens a esp2.

vale ressaltar que ficou um pouco confuso essa parte na explicacao da atividade, portanto, fiz com que a esp2 ao receber a mensagem de parada pelo switch, tambem parasse de soar o alarme
pois com a explicacao dada em sala faria mais sentido parar, ja que seria alarme falso.
