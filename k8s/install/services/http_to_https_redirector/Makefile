deploy:
	kubectl create namespace redirector
	kubectl -n redirector create configmap redirector-config --from-file=redirector-config=redirector.conf
	kubectl -n redirector create -f ./deployment.yaml
	kubectl -n redirector create -f service.yaml
