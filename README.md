
== GeoExplorer on OpenShift ==

To deploy this example of GeoExplorer on OpenShift:

1. Create a new gear
  $ rhc app-create -s geoexplorer jbossews-2.0
2. Pull down this repo and push it to your new gear
  $ cd geoexplorer
  $ git remote add github -m master https://github.com/jason-callaway/geoexplorer-on-openshift.git
  $ git pull -s recursive -X theirs github master
  $ git rm pom.xml
  $ git commit -am 'initial commit'
  $ git push origin
