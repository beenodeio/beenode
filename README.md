# beenode
<div align="center">
<img src="https://github.com/beenodeio/beenode/blob/main/Imagens/Logo-beenode.io-1.png" width="400px" />
</div>

## O que é ?

Beenode é uma plataforma para aplicações em internet das coisas ou indústria 4.0 que busca ajudar empresas, integradores e entusiastas a integrar seus dispositivos a nuvem de forma simples.
A beenode possui um Broker MQTT integrado que pode ser facilmente configurado e utilizado pelos usuários.
Com a beenode é possível monitorar e controlar seus dispositivos pela internet onde quer que você esteja.

## Task lists

- [x] Plataforma
- [x] KPIs internos
- [x] Broker MQTT
- [x] Instancia Node-Red
- [ ] Alarmes e eventos
- [ ] Integração Telegram
- [ ] Integração dados Node-Red + beenode
- [ ] Integração Google Sheets
- [ ] Criação instancia privativa (VPS)
- [ ] Bando de dados
- [ ] Integração Grafana
- [ ] Coletor de dados (OPC-UA, OPC-DA, MySQL, Oracle)

## Como utilizar ?

Após o cadastro na pagina da [Beenode](http://beenode.io/Login), o usuário deverá abrir a aba do MQTT e fazer no cadastro no Broker.
O usuário receberá as informações basicas para conexão em TCP.

<div align="center">
<img src="https://github.com/beenodeio/beenode/blob/main/Imagens/MQTT_Beenode_V1.png" width="300px" />
</div>

Cada usuário receberá um tópico esclusivo na qual poderá publicar e subescrever as informações e tambem criar subtópicos.
**Rescrições** não é possivel publicar ou subescrever em um toíco diferente do cadastrado. Os limites de taxa de envio estão limitadas ao processamento do servidor e a utilização dos demais clientes. **OBS**: Usuários da conta gratuita irão compartilhar do mesmo Broker e poderá no futuro sofrer limitações na taxa de envio.

## Como funciona ?

A plataforma pode receber informações de coletores de dados enviados via MQTT para o Broker da beenode, onde é posivel trabalhar de duas formas.
Utilizando os KPIs internos da beenode para monitorar e controlar os devices, ou utilizando a instancia do Node-Red criada no momento da criação de cadastro do usuário para criação de logicas e Dashboards.

<div align="center">
<img src="https://github.com/beenodeio/beenode/blob/main/Imagens/PLC_Sensor_DB_MQTT_Senario.png" width="800px" />
</div>

