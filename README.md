# Get OCP and ASB up and running

## The broker

Execute the script:
```
./ocp_asb_setup.sh 

```

## The apb CLI

```
alias apb='docker run --rm --privileged -v $PWD:/mnt -v $HOME/.kube:/.kube -v /var/run/docker.sock:/var/run/docker.sock -u $UID docker.io/ansibleplaybookbundle/apb-tools:release-1.1' 

apb list
```

## Some other commands

```

oc project kube-service-catalog

oc get clusterservicebroker template-service-broker -o yaml

svcat get broker
```

