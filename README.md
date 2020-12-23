<h1> nudge_ci: nudge pipelines for continuous integration </h1>
<h2>The full path where all repositry cloned in github runner  is :</h2>
<h5>==> /home/runner/work/nudge_ci/nudge_ci/</h5>

<h2>The  pipeline Github Actions used is here : </h2>
<h5>==> .github/workflows/build-nudge-server.yml</h5>

<h2> The pipeline clone all those repository to generate jar/war files :</h2>
<h5>==> nudge-dockerfiles | nudge-parent  | nudge-legacy-dependencies  |nudge-buffer-cassandra| nudge-buffer-probe | nudge-apm-server</h5>

<h2> Dockerfile and all config files used are cloned from this path of  nudge-dockerfiles repository  :</h2>
<h5>==> nudge-dockerfiles/nudge-apm/server </h5>
<h5> EX: COPY nudge-dockerfiles/nudge-apm/server/conf/nudge-server.properties $NUDGE_CONFIG/nudge-server.properties</h5>

<h2> Nudge-server war genereted from this repository nudge-apm-server in this path : </h2>
<h5>==>  nudge-apm-server/nudge-war/ </h5>
<h5> EX: COPY  nudge-apm-server/nudge-war/target/*.war  /usr/local/tomcat/webapps/ROOT.war </h5>

<h2> After generating the war file and cloning Dockerfile  and necessary configuration files we have to: </h2>
<h5> Build nudge image docker  | Loging to the registry with secrets token | push image to the registry . </h5>

<h2> We ended our pipeline with Logout from the docker registry and remove nudge the image after we pushed, and delete all repositories cloned.  </h2>
