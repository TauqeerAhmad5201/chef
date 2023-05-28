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

