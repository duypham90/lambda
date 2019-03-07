# PHP run on Lambda
## https://aws.amazon.com/vi/blogs/apn/aws-lambda-custom-runtime-for-php-a-practical-example/
`js`
./configure --prefix=/home/ec2-user/php-7-bin/ --with-openssl=/usr/local/ssl --with-curl --with-zlib --enable-mbstring --enable-json 

copy file from EC2 to local: scp -i testLambdaPHP.pem ec2-user@ec2-52-205-142-31.compute-1.amazonaws.com:/home/ec2-user/php-7-bin/bin/php ~/Desktop/
