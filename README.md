# config-single
This is my personal Ubuntu commonly used profile
The README.md let you know how to design:

    mkdir ~/.git && git init

    # mv ~/.bashrc ~/.git/.basrc && ln -s ~/.git/.bashrc ~/.bashrc

    mv $HADOOP_HOME/etc/hadoop ~/.git/hadoop-conf && ln -s ~/.git/hadoop-conf $HADOOP_HOME/etc/hadoop

to move all your common profile or config, and ln -s it
## so,let's commit all files.

    cd ~/.git && git add ./*

    git commit -m "single mode config init"

    git remote add origin git@github.com:username/config.git

    git config -l

    git push -u origin master

## also, you can make a branch like:

    git checkout -b single
