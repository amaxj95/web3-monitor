# web3-monitor

  Experimental only.

The server is built using containers. For setup, a postgres container, a redis container, and el;astisearch container were built and attached to a docker network. 
  > docker run --network web3-monitor --name web3-postgres -p 5432:5432 -e POSTGRES_USER=admin -e POSTGRES_PASSWORD=web3Password -e POSTGRES_DB=web3_mon -d postgres:15.2-alpine
  > docker run --network web3-monitor --name web3-redis -d -p 6379:6379 redis:7.0.8-alpine3.17
  > docker run --network web3-monitor --name web3-elastic -d -p 92__:92__ -p 93__:93__ -e "discoversy.type=single-node" elasticsearch:8.6.2
