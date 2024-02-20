## ssh into Racoon web-api 
`gcloud compute ssh --project racoon-staging-ab15d --zone europe-west2-c user@web-api-001`
`journalctl -flu web-api`

## Allocate 4GB of heap memory to node
 `export NODE_OPTIONS=--max-old-space-size=4096`


## Library to run secuity audit on node.js apps
Install
`npm i -g snyk`
Test
`snyk test` 
Open wizard that will walk you through patching vunerabilities
`snyk wizard`

## Start redis server locally
`sudo systemctl start redis-server`

## Isaac reference number school adminissions
846-2024-09-E-114067

## Restart Netowrk 
sudo service NetworkManager stop
sudo rm /etc/NetworkManager/system-connections/*
sudo service NetworkManager start
sudo ifdown th0 && sudo ifup eth0
