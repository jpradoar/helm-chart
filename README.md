# helm-chart
A personal helm repo chart

<br>

### Add this repo
	helm repo add jpradoar https://jpradoar.github.io/helm-chart/

### Optional update repo
	helm repo update

### To see all charts
	helm search repo jpradoar		

### Install a demo deployment
	helm upgrade -i -n superdemo --create-namespace superdemo jpradoar/demo
 	helm upgrade -i -n default --create-namespace demoapp jpradoar/domoticz \
  		--set general.name=democlient \
    		--set general.tz=America/Argentina/Buenos_Aires \
      		--set service.loadBalancer=None


### Delete demo depoyment
	helm -n superdemo delete superdemo


<br>

### Create new Helms  (helm-chart)
	helm create demo
	helm package demo/
	mv demo-x.y.tgz charts/
	helm repo index .
