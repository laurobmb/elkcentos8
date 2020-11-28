# Install ELK on Centos 8 usando ANSIBLE 

## Install cluster of Elasticsearch

O servidor do Elasticsearch é instalado em cluster, logo são necessários no minimo dois servidores para iniciar o projeto.

> Alterar endereços IP no [inventory.txt](https://github.com/laurobmb/elkcentos8/blob/main/inventory.txt) com os endereços do elasticsearch master end slave 

> Alterar também os endereços IP do elasticsearch master end slave no all.yml

## Install Kibana

A role do Kibana instala também um Nginx para sevir como PROXY de acesso ao KIBANA. 

> Alterar o usuário e senha no arquivo kibana.yml

> Alterar o arquivo all.yml para informar o dominio do PROXY NGINX e ainda informar os usuarios e senhas iniciais do acesso.

## Install Logstash

Informar o endereço IP o Logstach no inventory.txt

>Em aberto 

## Install client

Informar o endereço IP dos clientes no inventory.txt

#### install metricbeats
#### install auditbeat
#### install filebeat

# Comandos 

* ansible-playbook -i inventory.txt project.yml --tags "elasticsearch"
* ansible-playbook -i inventory.txt project.yml --tags "monitoring_clients"
* ansible-playbook -i inventory.txt project.yml --tags "kibana"
* ansible-playbook -i inventory.txt project.yml --tags="logstash"


# Referencia
