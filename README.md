# Configuração do InfluxDB no JMeter usando o Backend Listener

Para trabalhar com o InfluxDB na versão 2.0 ou superior, precisará adicionar o plugin ***“jmeter-plugins-influxdb2-listener”*** em: ***“apache-jmeter-5.5\lib\ext”***. Segue o link para baixar o plugin na versão 2.5:  
https://github.com/mderevyankoaqa/jmeter-influxdb2-listener-plugin/releases/download/v2.5/jmeter-plugins-influxdb2-listener-2.5.jar

1- Após adiconar o plugin (conforme orientação acima), abra o ***Apache JMeter*** e carregue algum script de sua preferenci.

[SCRIPT_JPetStore_BackendListener_InfluxDB2.zip](https://github.com/leandrogf1980/config_InfluxDB_in_JMeter_using_BackendListener/files/11133465/SCRIPT_JPetStore_BackendListener_InfluxDB2.zip)

2- Clique com o direito do mouse em: ***Test Plan > Listener > Backend Listener***.

![image](https://user-images.githubusercontent.com/126198206/221881066-a7c9a1f8-033a-44ab-b78b-ac3337b9d659.png)

3- Configurar o ***Backend Listener*** para que o JMeter se comunique com o InfluxDB.  
Realize a configuração conforme a imagem abaixo:

![image](https://user-images.githubusercontent.com/126198206/221884326-eb2a9d13-19c9-4397-b580-00bbcc44d84a.png)

3.1- No campo ***influxDBHost*** deverá ser informado o ***IP da máquina*** onde o InfluxDB está sendo executado, se estiver local informe ***“localhost”***.  
3.2- No campo ***influxDBPort*** deverá ser informado a porta que foi definida na instalação do InfluxDB, por padrão é a porta 8086.  
3.3- No campo ***influxDBToken*** deverá ser informado o Token gerado no influxDB.  
3.4- Nos campos ***influxDBOrganization*** e ***influxDBBucket*** deverão serem informados o ***Nome da Organização*** e o ***Bucket*** definidos no primeiro acesso ao influxDB.
