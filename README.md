# Swarmpracticecmds
yum install docker -y && systemctl start docker

    2  docker swarm init

    3  docker node ls

    4  docker service create --name flm --publish 1111:80 shaikmustafa/dm

    5  docker service ls

    6  docker service ps flm

    7  docker ps

    8  docker service rm flm

    9  docker service create --name leeshma --replicas 6 --publish 2222:80 shaikmustafa/cycle

   10  docker service ls

   11  docker service ps leeshma

   12  docker ps

   13  docker inspect leeshma.1.t1luzubplndki883ttfiz7pzt

   14  docker inspect leeshma.1.t1luzubplndki883ttfiz7pzt | grep -i "port"

   15  docker inspect leeshma.1.t1luzubplndki883ttfiz7pzt | grep -i "hostport"

   16  docker service ps leeshma

   17  docker service ls
   #scale

   18  docker service scale leeshma=10

   19  docker service ps leeshma
#descale
   20  docker service scale leeshma=3

   21  docker service ps leeshma
#update service
   22  docker service update --image shaikmustafa/dm leeshma

   23  docker service update --image shaikmustafa/mygame leeshma

   24  docker service ps leeshma
#rollback to prevoius service only 1 time will be rollback
   25  docker service rollback leeshma

   26  docker service ps leeshma

   27  docker service update --image shaikmustafa/cycle leeshma

   28  docker service ls

   29  docker service inspect leeshma

   30  docker service logs leeshma
   31  docker service

   32  docker swarm join-token worker

   33  docker node ls

   34   docker node ls

   35  docker service ls

   36  docker node ls

   37  docker node rm bsk7t6f1ypq9roas7a5r92njx

   38  docker node ls

   39  docker node rm bsk7t6f1ypq9roas7a5r92njx

   40  docker node ls

   41  docker node rm y8nm36xbd688cfvljz5a8ojnw

   42  docker node ls

   43  docker node rm qw2h6rghottttextvc2h4cnpy

   44  docker node ls

   45  docker swarm join-token manager

   46  docker node ls

   47  history
