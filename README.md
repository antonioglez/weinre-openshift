# weinre-openshift

An instance of Weinre served over Openshift.

Pay attention to the package.json file, set the proper weinre dependencies.

The application will work only if it binds to "$OPENSHIFT_INTERNAL_IP:8080". Therefore, make sure to set the proper script in package.json:

"weinre --httpPort 8080 --boundHost $OPENSHIFT_INTERNAL_IP"