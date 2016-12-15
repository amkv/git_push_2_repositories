# git_push_2_repositories

This simple script just helps you to push your projects files to 2 git repositories, the script simply changes the config file names

make a copy of your config file in the .git folder
```
cd .git
cp config config_g
```

change the url variable in config_g
```
url =  https://github.com/your_login/project.git
```
go back

```
cd ../
```

and clone 
```
git clone https://github.com/amkv/git_double_push.git
```

move sh_push script to your project folder
```
mv git_double_push/sh_push .
```
change permissions
```
chmode 755 sh_push
```
launch
```
./sh_push
```
or

```
./sh_push "text to commit"
```
