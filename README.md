<h1> nudge_ci: nudge pipelines for continuous integration </h1>
<h2>The full path where all repositry cloned in github runner  is :</h2>
==> /home/runner/work/nudge_ci/nudge_ci/ 

<h2>The  pipeline Github Actions used is here : </h2>
==> .github/workflows/build-nudge-server.yml

<h2> The pipeline clone all those repository to generate jar/war files :</h2>
==> nudge-dockerfiles | nudge-parent  | nudge-legacy-dependencies  |nudge-buffer-cassandra| nudge-buffer-probe | nudge-apm-server

<h2> Dockerfile and all config files used are cloned from this path of  nudge-dockerfiles repository  :</h2>
==> nudge-dockerfiles/nudge-apm/server
<h3> EX: COPY nudge-dockerfiles/nudge-apm/server/conf/nudge-server.properties $NUDGE_CONFIG/nudge-server.properties</h3>

<h2> Nudge-server war genereted from this repository nudge-apm-server: </h2>
<h5> EX: COPY  nudge-apm-server/nudge-war/target/*.war  /usr/local/tomcat/webapps/ROOT.war </h5>
