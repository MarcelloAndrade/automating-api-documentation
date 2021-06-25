https://github.com/Tufin/oasdiff

## run public 
docker run --rm -t tufin/oasdiff -format text -base https://raw.githubusercontent.com/Tufin/oasdiff/main/data/openapi-test1.yaml -revision https://raw.githubusercontent.com/Tufin/oasdiff/main/data/openapi-test3.yaml

## run local
docker run --rm -t -v $(pwd)/data:/data:ro tufin/oasdiff -format text -base /data/pet-store-v1.0.0.yaml -revision /data/pet-store-v1.0.1.yaml

docker run --rm -t -v $(pwd)/data:/data:ro tufin/oasdiff -format html -base /data/pet-store-v1.0.0.yaml -revision /data/pet-store-v1.0.1.yaml

## pesquisa
api compare response with specification

https://github.com/OpenAPITools/openapi-diff

https://medium.com/condorlabs-engineering/automating-api-documentation-c8f48f2bc30e