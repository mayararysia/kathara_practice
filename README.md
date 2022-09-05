# kathara_practice

Network Operating Systems classes at IFAL 2022.1

## Requirements

- [x] Docker

## Start

- If you are on windows, start docker first
- Open your terminal

## Examples

### Start a device

````
    kathara vstart -n pc1
````

- In pc1:

````
    ifconfig
````

### Deleting devices

````
    kathara vclean -n pc1
````

### Stopped scenarios

````
    kathara lclean
````

### Enable internet access

````
    kathara vstart --bridged -n pc1
````

### Start custom instance

- e.g.:

````
    kathara vstart -i ubuntu -n pc1
````

### Connect 2 devices on the same local network

````
    kathara vstart --eth 0:a --bridged -i ubuntu -n pc1

    kathara vstart --eth 0:a --bridged -i ubuntu -n pc2
````

### If I want to connect a third PC that belongs to an additional LAN and is shared only with PC1:


````
    kathara vclean -n pc1

    kathara vstart --eth 0:a 1:b --bridged -i ubuntu -n pc1

    kathara vstart --eth 0:b --bridged -i ubuntu -n pc3
````


