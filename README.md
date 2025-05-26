# PPS-IniciacionKubernetes
Siguiendo el vídeo de Pelardo Nard sobre KUBERNETES De NOVATO a PRO!   https://youtu.be/DCoBcpOA7W4


Sigue el vídeo del canal de Pelardo Nard sobre <https://youtu.be/DCoBcpOA7W4>

- Si quieres, puedes clonar el repositorio de peladonerd para poder ver archivos de configuración: 

```bash
git clone https://github.com/pablokbs/peladonerd.git
``` 
- Comprueba si tienes kubectl instalado en tu equipo:

```bash
kubectl version --client=true
``` 

- Instala kubernetes kubectl (si no está instalado)

	- en windows 
		<https://kubernetes.io/es/docs/tasks/tools/included/install-kubectl-windows/>
	- en linux <https://kubernetes.io/es/docs/tasks/tools/included/install-kubectl-linux/> 

- Instalamos también `MiniKube`:
<https://minikube.sigs.k8s.io/docs/start/>

```bash
curl -LO https://storage.googleapis.com/minikube/releases/latest/minikube_latest_amd64.deb
sudo dpkg -i minikube_latest_amd64.deb
``` 

- Iniciamos `MiniKube`
```bash
minikube start
``` 
![](images/image1.png)

 Tendrás la siguiente estructura de archivos:

![](images/image2.png)

- Comprobamos estructura de nodos creados

```bash
kubectl get nodes
``` 
![](images/image3.png)

- Para ver la lista de acciones o comandos posibles:

```bash
kubectl --help
``` 

![](images/image5.png)

- Obtnemos configuración.
```bash
kubectl config get-contexts 
``` 

![](images/image4.png)

(min 20)

- Obtenemos los namespaces

```bash
kubectl get ns
``` 
![](images/image6.png)

- Ver Pods

```bash
kubectl -n kube-system get pods
``` 
![](images/image7.png)
```bash
kubectl -n kube-system get pods -o wide
``` 

(min 24:30)
- Borramos 
- Realiza también los apartados de Verificar la configuración y Plugins y configuraciones adiccionales.

- Instalamos Kind para crear los cluster :   https://kind.sigs.k8s.io/docs/user/quick-start/#installing-with-a-package-manager



```bash

``` 
- Descarga el archivo config.yaml que tienes adjunto. Nos servirá para crear un cluster de 3 nodos.


```bash

``` 

- Crea el cluster con el comando: kind create cluster --config=config.yaml

```bash

``` 

- Iniciamos minikube: minikube start

```bash

``` 
- Creamos cluster de kubernetes con minikube: https://k8s-docs.netlify.app/en/docs/setup/learning-environment/minikube/ (Si tienes problemas para crear el cluster con minikube, puedes utilizar Kind:

```bash

``` 
![](images/image.png)
![](images/image.png)
![](images/image.png)
![](images/image.png)
![](images/image.png)
![](images/image.png)
![](images/image.png)
