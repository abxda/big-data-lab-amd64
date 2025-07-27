 # -*- mode: ruby -*-
 # vi: set ft=ruby :

 Vagrant.configure("2") do |config|
   config.vm.box = "abxda/big-data-lab"

   config.vm.network "forwarded_port", guest: 8888, host: 8888 # Jupyter Lab
   config.vm.network "forwarded_port", guest: 9870, host: 9870 # Hadoop HDFS UI
   config.vm.network "forwarded_port", guest: 9200, host: 9200 # Elasticsearch API

   config.vm.provider "virtualbox" do |vb|
     vb.memory = "4096"
     vb.cpus = 4
   end
 end
