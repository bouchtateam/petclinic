# petclinic
<<<<<<< HEAD
test12234
=======

testtt22
>>>>>>> 3dc1f7dad3346631000c0b35b1b9ae1269851b83
TEST2
test avec sam 
<h1> nudge_ci: nudge pipelines for continuous integration </h1>
The full path where all repositry cloned in github runner  is : /home/runner/work/nudge_ci/nudge_ci/

<h2>The  pipeline Github Actions used is here : </h2>
 .github/workflows/build-nudge-server.yml

<h2> The pipeline clone all those repository :</h2>
 nudge-dockerfiles | nudge-parent  | nudge-legacy-dependencies  |nudge-buffer-cassandra| nudge-buffer-probe | nudge-apm-server
<h2> Dockerfile and all config files used are cloned from this path of repository nudge-dockerfiles :</h2>
nudge-dockerfiles/nudge-apm/server
ex:
<h3> COPY nudge-dockerfiles/nudge-apm/server/conf/nudge-server.properties $NUDGE_CONFIG/nudge-server.properties </h3>
<h2> Nudge-server war genereted from this repoitory nudge-apm-server: </h2>
COPY  nudge-apm-server/nudge-war/target/*.war  /usr/local/tomcat/webapps/ROOT.war
