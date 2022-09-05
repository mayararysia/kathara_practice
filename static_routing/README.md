# **Configuração manual**

````
ifconfig
````

"O comando ifconfig é um comando pertencente ao pacote **net-utils** que tem por objetivo possibilitar a recuperação das informações das interfaces de rede e a configuração das redes."

- [x] Endereço IP: apresentado após as palavras **inet addr**;
- [x] Endereço MAC: apresentado após a palavra **HWaddr**.

## Para configurar o endereçamento de modo manual

````
ifconfig interface endereco ip netmask mascara
````
    =

````
ifconfig eth0 192.168.0.1/24
````

````
ip a
````

````
ifconfig -a
````