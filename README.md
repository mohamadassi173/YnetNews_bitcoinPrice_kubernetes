### Ynet News And Bitcoin Price With kubernetes

#### Kubernetes project that shows price of BitCoin and displays the latest news from Ynet:    
● Presents the Current BitCoin Price, And the Average Price for the last 10 minutes and stores the price in a Redis Database.  
● Reads the “Breaking News” from YNet news service.  
  

## ⚡Run With Minikube:

Clone the project

```bash
  git clone https://github.com/mohamadassi173/YnetNews_bitcoinPrice_kubernetes.git
```

Go to the project directory

```bash
  cd YnetNews_bitcoinPrice_kubernetes
```

Start minikube

```bash
  minikube start
```

Enable ingress addon

```bash
  minikube addons enable ingress
```
Apply Deployment

```bash
  kubectl apply -f .
```

Start minikube tunnel

```bash
  minikube tunnel
```

Access from browser:  
● http://localhost/bitcoin
● http://localhost/ynet  

## ⚡Run the apps with Docker

Run BitCoin image from DockerHub

```bash
  docker pull mohamadassi173/bitcoin-flask
  docker run -d -p 8000:5000 mohamadassi173/bitcoin-flask:latest
```
<img width="932" alt="image" src="https://user-images.githubusercontent.com/57872327/177643708-e471383c-7a00-4601-9f9b-4986d45e87ad.png">

  
Run Ynet image from DockerHub

```bash
  docker pull mohamadassi173/ynet
  docker run -d -p 8000:5000 mohamadassi173/ynet:latest
```
<img width="919" alt="image" src="https://user-images.githubusercontent.com/57872327/180656827-beb39b46-b3b9-4d8c-9f39-88885457f50f.png">

## Author

- [@Mohamad Assi](https://github.com/mohamadassi173)

