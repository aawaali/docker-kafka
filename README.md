# docker-kafka
this is a simple docker compose file to run a kafka broker locally in docker container (alongside with zookeeper in seperate container).<br>
both kafka and zookeeper docker images are built from a basic official alpine image, and have nothing insalled except oppenjdk8, kafka or zookeeper.
# prerequisites
to run docker-compose you must have both docker and docker-compose installed.
# start
to start kafka node, grab a terminal and run below commands :<br>
  1- git clone https://github.com/aawaali/docker-kafka.git<br>
  2- cd docker-kafka<br>
  3- docker-compose up -d // this might take a while the first time because it will pull(download) the images in your local repo<br>
  4- add the below line in your /etc/hosts file:<br>
    <pre>127.0.0.1 kafka</pre>
and voila, your kafka node is up and running, and listening in localhost:9092.<br>
  # stop
  you can stop your kafka node by typing the below command from docker-kafka folder
  <pre>docker-compose down -v</pre>
