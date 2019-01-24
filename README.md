# ecommerce app


#first create network ecom
docker network create ecom


#in each folder of microservices

#produit
docker build . -t produit-image
docker run -t -p 9001:9001 --network="ecom" --name produit-container produit-image

#commande
docker build . -t commande-image
docker run -t -p 9001:9001 --network="ecom" --name commande-container commande-image

#paiment
docker build . -t paiment-image
docker run -t -p 9001:9001 --network="ecom" --name paiment-container paiment-image
