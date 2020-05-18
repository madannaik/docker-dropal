# My docker project
# ABOUT DOCKER
Developing apps today requires so much more than writing code. Multiple languages, frameworks, architectures, and discontinuous interfaces between tools for each lifecycle stage creates enormous complexity. Docker simplifies and accelerates your workflow, while giving developers the freedom to innovate with their choice of tools, application stacks, and deployment environments for each project.

# ABOUT DROPAL
Drupal is a free and open-source content-management framework written in PHP and distributed under the GNU General Public License. It is used as a back-end framework for at least 2.1% of all Web sites worldwide ranging from personal blogs to corporate, political, and government sites including WhiteHouse.gov and data.gov.uk. It is also used for knowledge management and business collaboration.

# Inorder to provide the storage for drupal image i chosed mysql docker image

#  Steps to configure drupal
1)copy the above docker-compose.yml file in a system that has pre-setup docker in it 

2)go the folder where you copied the above file and run "docker-compose up -d" command.It will launch drupal and mysql containers

3)go to web browser type "htttp://localhost:8081".It will take you to drupal configuration page

4)select a language for your use(eg. english).click next

5)give your site name,login id and password for further excess!!then click next

7)in database configuration option:select mysql
    
    - Database name/username/password: <details for accessing your MySQL instance> (MYSQL_USER, MYSQL_PASSWORD, MYSQL_DATABASE; see          environment variables in the description in docker-compose file for mysql)
    - ADVANCED OPTIONS - Database host: database (Containers on the same docker-network are routable by their container-name)
    
8)then finish the installation
  
# Now you are ready for using drupal!!!!
create a article or blog without having to worry about the server or storage just login and use!!! 
