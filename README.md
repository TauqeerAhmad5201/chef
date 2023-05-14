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
