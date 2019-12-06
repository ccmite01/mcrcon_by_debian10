mcrcon compiled by debian10.
# Made way
<pre>
docker run --rm --name testbuster -v /share/Container/container-station-data/application/ccmite/mcrcon_by_debian10:/mnt/mcrcon -it debian:buster /bin/bash
apt --allow-releaseinfo-change update && apt install -y gcc make
cd /mnt/mcrcon
curl -s -k --tlsv1.2 https://codeload.github.com/Tiiffi/mcrcon/tar.gz/v0.6.1 -o mcrcon-src-0.6.1.tgz
tar zxf mcrcon-src-0.6.1.tgz
cd mcrcon-src-0.6.1
make
</pre>
