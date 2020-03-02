# wishlist
Sample wishlist application to demo microservices with containers running in Kubernetes.

docker build -t pervonrosen/wishlist:1.0 -f Dockerfile.list .

docker build -t pervonrosen/wishlist-auth:1.0 -f Dockerfile.auth .

docker build -t pervonrosen/wishlist-catalog:1.0 -f Dockerfile.catalog .

docker push pervonrosen/wishlist-catalog:1.0

docker push pervonrosen/wishlist-auth:1.0

docker push pervonrosen/wishlist:1.0
