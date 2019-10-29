# PHP run on Lambda

https://aws.amazon.com/vi/blogs/apn/aws-lambda-custom-runtime-for-php-a-practical-example/

## PHP release
https://github.com/php/php-src/releases?after=php-7.1.28

## Note
Disable OPcache in php: 
```
--disable-opcache
```

```
./configure --prefix=/home/ec2-user/php-7-bin/ --with-openssl=/usr/local/ssl --with-curl --with-zlib --enable-mbstring --enable-json --disable-opcache

copy file from EC2 to local: scp -i testLambdaPHP.pem ec2-user@ec2-52-205-142-31.compute-1.amazonaws.com:/home/ec2-user/php-7-bin/bin/php ~/Desktop/

serverless deploy function -f getdata && serverless invoke -f getdata -l
```

https://articles.microservices.com/monolithic-vs-microservices-architecture-5c4848858f59

https://viblo.asia/p/doi-net-ve-microservice-architecture-va-monolithic-architecture-XL6lAAvrlek
