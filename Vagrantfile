# -*- mode: ruby -*-
# vi: set ft=ruby :
HERE = File.dirname(__FILE__)

Vagrant::Config.run do |config|
  config.vm.box     = "precise64"
  config.vm.box_url = "http://files.vagrantup.com/precise64.box"
  
  config.vm.define :dev do |config|
    chef.cookbooks_path = ["#{HERE}/cookbooks"]
    chef.add_recipe("chef-workstation")
 end

end
