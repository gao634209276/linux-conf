# config-single
This is my personal Ubuntu commonly used profile
The README.md let you know how to design:

    mkdir ~/.git-config && git init

## also, you can make a branch like:

    git checkout -b single

## move all your single mode common profile or config, and ln -s it

    # mv ~/.bashrc ~/.git-config/.basrc && ln -s ~/.git-config/.bashrc ~/.bashrc
    mv $HADOOP_HOME/etc/hadoop ~/.git-config/hadoop-conf && ln -s ~/.git-config/hadoop-conf $HADOOP_HOME/etc/hadoop

## so,let's commit all files.

    cd ~/.git-config && git add ./*conf
    git commit -m "single mode config init"
    git remote add origin git@github.com:username/config-single.git
    git config -l
    git push -u origin single

## also, you can make a branch like:

    git checkout -b distribute

delete all file of Dir ~/.git-config. Ant then, move your distribute mode common profile or config, and ln -s it
when you want to change the env,just use a cmd:

    cd ~/.git-config
    git checkout single

or

    git checkout distribute

