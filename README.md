# CS3219 OTOT
> Source:
> - [A1.1_3](https://github.com/CS3219-AY2223S1/OTOT-A1)
> - [A2 & 3](https://github.com/CS3219-AY2223S1/OTOT-A2-A3)

## A1.1 - Dockerize node app in `app` folder

In the `app/index.html` file, search for "TODO" and fill in the blanks.

Follow these guide to Dockerize the sample node app.
- [https://nodejs.org/en/docs/guides/nodejs-docker-webapp/](https://nodejs.org/en/docs/guides/nodejs-docker-webapp/)

Extra: Learning how to render HTML file using express.js
- [https://expressjs.com/en/starter/hello-world.html](https://expressjs.com/en/starter/hello-world.html)
- [https://codeforgeek.com/render-html-file-expressjs/](https://codeforgeek.com/render-html-file-expressjs/)

## A1.2 - Dockerize NGINX reverse proxy in `nginx-sample` folder

In the `nginx-sample/index.html` file, search for "TODO" and fill in the blanks.

Follow these guide to dockerise the sample NGINX reverse proxy to serve the static HTML in `nginx/index.html`.
- [https://docs.nginx.com/nginx/admin-guide/web-server/serving-static-content/](https://docs.nginx.com/nginx/admin-guide/web-server/serving-static-content/)
- [https://docs.nginx.com/nginx/admin-guide/web-server/reverse-proxy/](https://docs.nginx.com/nginx/admin-guide/web-server/reverse-proxy/)
- [https://www.nginx.com/blog/deploying-nginx-nginx-plus-docker/](https://www.nginx.com/blog/deploying-nginx-nginx-plus-docker/)

## A1.3 - Use NGINX to serve the node app using `docker-compose`

Create a new NGINX conf file and Dockerfile in `nginx` folder. Run the application stack in `app` and `nginx` using `docker-compose`.

Follow this guide to use NGINX to act as a reverse proxy such that when a browser makes a HTTP request, the request first goes to the reverse proxy and then sends the request to the appropriate web server. Your final task, you have to server the node app in `app` folder. Use a separate config file from A1.2.
- [https://ashwin9798.medium.com/nginx-with-docker-and-node-js-a-beginners-guide-434fe1216b6b](https://ashwin9798.medium.com/nginx-with-docker-and-node-js-a-beginners-guide-434fe1216b6b)

## A2 - Introduction to Kubernetes

This assignment has three parts:
* A2.1 Deploy a local k8s cluster
* A2.2 Deploy your A1 Docker image as Deployment in A2.1 cluster
* A2.3 Deploy Ingress to expose A2.2 Deployment to your localhost

Follow the guide in demo/a2/ to complete the tasks.
Place your manifests in k8s/manifests/ and commands used in k8s/a2_setup.sh.

## A3 - Scalability and Availability

This assignment has two parts:
* A3.1 Deploy HorizontalPodAutoscaler that makes A2.2 Deployments scale up under load.
* A3.2 Modify your A2.2 Deployment to be distributed equally in each zone


Follow the guide in demo/a3/ to complete the tasks.
Place your manifests in k8s/manifests/ and commands used in k8s/a3_setup.sh.