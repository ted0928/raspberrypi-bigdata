# raspberrypi-bigdata
bigdata frameworks on raspberrypi


docker pull docker pull ted0928/raspberry_presto

git clone https://github.com/ted0928/raspberrypi-presto.git

sudo docker run -d -v ~/raspberrypi-presto/presto/cluster/coordinator_etc:/root/presto/etc -v /var/presto:/var/presto -p 8080:8080 ted0928/raspberry_presto:0.187

sudo docker run -d -v ~/raspberrypi-presto/presto/cluster/works_etc:/root/presto/etc -v /var/presto:/var/presto -p 8080:8080  --add-host=master:192.168.0.183 ted0928/raspberry_presto:0.187 
