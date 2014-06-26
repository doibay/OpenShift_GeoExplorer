GeoExplorer on OpenShift
========================

To deploy this example of GeoExplorer on OpenShift:

1.  Create a new gear

    ```rhc app-create -s geoexplorer jbossews-2.0```

2.  Pull down this repo

    ```cd geoexplorer

    git remote add github -m master https://github.com/jason-callaway/geoexplorer-on-openshift.git

    git pull -s recursive -X theirs github master```

3.  We don't need to build anything, so remove pom.xml

    ```git rm pom.xml```

4.  Now commit and push

    ```git commit -am 'initial commit'

    git push origin```
