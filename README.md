# helm-chart
A personal helm repo chart

<br>

### Add this repo
	helm repo add jpradoar https://jpradoar.github.io/helm-chart/

### Optional update repo
	helm repo update

### To see all charts
	helm search repo jpradoar		


<br>

### Create new Helms  (helm-chart)
	helm create demo
	helm package demo/
	mv demo-x.y.tgz charts/
	helm repo index .
