# Install ELK on Centos 8 usando ANSIBLE 

## Install cluster of Elasticsearch

O servidor do Elasticsearch é instalado em cluster, logo são necessários no minimo dois servidores para iniciar o projeto.

> Alterar endereços IP no [inventory.txt](https://github.com/laurobmb/elkcentos8/blob/main/inventory.txt) com os endereços do elasticsearch master end slave 

> Alterar também os endereços IP do elasticsearch master end slave no [all.yml](https://github.com/laurobmb/elkcentos8/blob/main/all.yml)

## Install Kibana

A role do Kibana instala também um Nginx para sevir como PROXY de acesso ao KIBANA. 


> Alterar o arquivo [all.yml](https://github.com/laurobmb/elkcentos8/blob/main/all.yml) para informar o [domínio](https://github.com/laurobmb/elkcentos8/blob/main/all.yml) do PROXY NGINX e ainda informar os usuários e senhas iniciais do acesso.

## Install Logstash

Informar o endereço IP o Logstach no [inventory.txt](https://github.com/laurobmb/elkcentos8/blob/main/inventory.txt)

>Em aberto 

## Install client

Informar o endereço IP dos clientes no [inventory.txt](https://github.com/laurobmb/elkcentos8/blob/main/inventory.txt)

#### install metricbeats
#### install auditbeat
#### install filebeat

# Comandos 

* ansible-playbook -i inventory.txt project.yml --tags "elasticsearch"
* ansible-playbook -i inventory.txt project.yml --tags "monitoring_clients"
* ansible-playbook -i inventory.txt project.yml --tags "kibana"
* ansible-playbook -i inventory.txt project.yml --tags="logstash"


# Referencia
