# system_setup

A Developer System Setup

Remcommended Hardware Config
 i5 11Gen 32G RAM 256 SSD 8G Cache
Software
Ubuntu 22.4 distribution

:Shell:
ZSH
Shell plugins:
oh-my-zsh: https://github.com/ohmyzsh/ohmyzsh
zsh-autosuggestions: https://github.com/zsh-users/zsh-autosuggestions
zsh-syntax-highlighting: https://github.com/zsh-users/zsh-syntax-highlighting
powerlevel10k: https://github.com/romkatv/powerlevel10k
tmux:https://github.com/justmeandopensource/dotfiles
1 cat ~/.zshrc
 2 git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
 3 vi ~/.zshrc
 4 ssh
 5 history
 6 git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting
 7 cat ~/.zshrc
 8 /plugin
 9 vi ~/.zshrc
 10 ls
 11 cd Documents/Software
 12 git clone - depth=1 https://github.com/romkatv/powerlevel10k.git ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/themes/powerlevel10k
 13 vi /.zshrc
 14 vi ~/.zshrc
 15 nano ~/.zshrc
 16 vi ~/.zshrc
 17 ls
 18 sudo apt install fonts-font-awesome
 19 ls
 20 git clone - depth=1 https://github.com/romkatv/powerlevel10k.git ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/themes/powerlevel10k
 21 vi ~/.zshrc
 22 sudo vi ~/.zshrc
 23 cd ~/Downloads
 24 cd ~/Documents/Software
 25 git clone https://github.com/justmeandopensource/dotfiles.git
 26 sudo apt install tmux
Install git
Install git ssh shell:
https://www.freecodecamp.org/news/git-ssh-how-to/
Install Docker:
https://www.digitalocean.com/community/tutorials/how-to-install-and-use-docker-on-ubuntu-22-04
Install visual studio:
47  sudo apt install code_1.81.1-1691620686_amd64.deb
   48  sudo dpkg -i code_1.81.1-1691620686_amd64.deb
   49  sudo apt-get install -f
   50  sudo apt install apt-transport-https
   51  sudo apt update
   52  sudo apt install code
Install Jetbrain Toolbox
JetBrains Toolbox App: Manage Your Tools with Ease
Open any of your projects in any of the IDEs with one click.www.jetbrains.com
36 sudo tar -xvzf ~/Downloads/jetbrains-toolbox-2.0.2.16660.tar.gz
 37 sudo mv jetbrains-toolbox-2.0.2.16660 jetbrains
 38 jetbrains/jetbrains-toolbox
 39 sudo jetbrains/jetbrains-toolbox
 40 sudo apt-get install fuse libfuse2\n
 41 sudo apt install libfuse2
 42 sudo kill -9 74565
 43 sudo apt install libfuse2
 44 sudo jetbrains/jetbrains-toolbox
 45 jetbrains/jetbrains-toolbox
Java
sudo apt-get install openjdk-8-jdk
Maven
153 wget https://mirrors.estointernet.in/apache/maven/maven-3/3.6.3/binaries/apache-maven-3.6.3-bin.tar.gz
 154 tar -xvf apache-maven-3.6.3-bin.tar.gz
 155 mv apache-maven-3.6.3 /opt/
 156 sudo mv apache-maven-3.6.3 /opt/
 157 M2_HOME='/opt/apache-maven-3.6.3'
 158 PATH="$M2_HOME/bin:$PATH"
 159 export PATH
Phoenix:
sudo docker run -p 8765:8765 boostport/hbase-phoenix-all-in-one:latest
Neo4j
sudo docker run \ - name neo4j \ -p7474:7474 -p7687:7687 \ -dit \ -v ~/Downloads/neo4j-19-july-2023/neo4j/data:/data \ -v ~/Downloads/neo4j-19-july-2023/neo4j/logs:/logs \ -v ~/Downloads/neo4j-19-july-2023/neo4j/conf:/var/lib/neo4j/conf:rw \ -v ~/Downloads/neo4j-19-july-2023/neo4j/import:/var/lib/neo4j/import \ -v ~/Downloads/neo4j-19-july-2023/neo4j/plugins:/plugins \ - env NEO4J_AUTH=neo4j/test123 \ neo4j:latest
Postgres
sudo docker run - name myPostgresDb -p 5432:5432 -e POSTGRES_USER=postgres -e POSTGRES_PASSWORD=postgres -e POSTGRES_DB=targettingframework -d postgres
Mongo
docker run -p 27017:27017 -d mongo -v IdeaProject/mongo:/data/db
Mysql
docker run -p 3306:3306 -v /tmp:/tmp - name db - detach -e MYSQL_ROOT_PASSWORD="qwe123" -e MYSQL_ROOT_HOST=% -e MYSQL_DATABASE=social -d mysql/mysql-server:5.6 - lower_case_table_names=1 - init-connect='GRANT CREATE USER ON . TO 'root'@'%';FLUSH PRIVILEGES;'
Redis Cluster
sudo docker run -e "IP=0.0.0.0" -p 7000–7005:7000–7005 grokzen/redis-cluster:latest
docker exec -it 4655936da4e9 sh
# redis-cli
Could not connect to Redis at 127.0.0.1:6379: Connection refused
not connected> CONFIG SET protected-mode no
Could not connect to Redis at 127.0.0.1:6379: Connection refused
not connected> 
not connected> exit
# redis-cli localhost:7000
Could not connect to Redis at 127.0.0.1:6379: Connection refused
# redis-cli -h localhost -p 7000
localhost:7000> CONFIG SET protected-mode no
OK
localhost:7000> CONFIG SET requirepass "test123"
OK
Redis UI:
docker run -dit -v redisinsight:/db -p 8001:8001 redislabs/redisinsight:latest
