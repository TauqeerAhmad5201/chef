# chef - Configuration Management Tool 

All about learnings of chef 

1. Make a workstation 
2. chef generate cookbook lamp_stack 
3. cd lamp_stack 
4. chef generate recipe lamp_recipe 
5. cd .. 
6. vi apache-cookbook/recipes/apache-recipe.rb 

---- Added code to run ----

7. chef exec ruby -c apache-cookbook/recipes/apache-recipe.rb
8. sudo chef-client -zr "recipe[apache-cookbook::server-recipe]" 

![Cookbook](https://github.com/TauqeerAhmad5201/chef/assets/68806440/be9cebb7-1956-43b2-b585-f99e65c0c35f)



Chef-attribute 
It is like props in react.js. 

Priority of Chef Attribute 

1. default 
2. force-default 
3. normal
4. override 
5. force-override 
6. automatic

Error: Connection time out 
Connection can't be established. 


Language used to script : Ruby for writing configuration

![image](https://github.com/TauqeerAhmad5201/chef/assets/68806440/5abe2c1a-f724-41c2-b548-7af4f9ee6bc3)

## Steps to reproduce: 

Hit with the following command 
sudo knife bootstrap 172.31.2.183 -U ec2-user --sudo -i node1.pem -N node1

## Definition
Chef is broken down into three main components: the workstation, the server, and the nodes. 

The workstation is the system where the admin sits. The system creates the code for configuring and managing the infrastructure, and that code (which is written in Ruby) is called a recipe. Multiple recipes in a collection are called cookbooks. The cookbooks are uploaded to the server by means of the Knife command line.

The Chef server is accessed primarily by nodes that are under management by Chef, as the chef-client runs occur. It is also accessed by individuals who maintain cookbooks and policy that is stored on the Chef server, typically from a workstation. And also by individual users with credentials to Chef server components, such as the Chef management console.

## Load Balancer

Nginx is an open-source HTTP and reverse proxy server that is used as the front-end load balancer for the Chef server. All requests to the Chef server API are routed through Nginx.

## Chef Key metrics 

- Chef supports multiple platforms like AIX, RHEL/CentOS, FreeBSD, OS X, Solaris, Microsoft Windows and Ubuntu. Additional client platforms include Arch Linux, Debian and Fedora.
