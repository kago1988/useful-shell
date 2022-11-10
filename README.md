# useful-shell
(Hobby) A few very basic but useful shell commands


```
cd  # switches automatically to /home/user 
cd ..  # switches automatically one file in the hierachy up 
cd folder  # switches automatically into the folder named 'folder' 
cd -  # switches into the last folder 
pwd # print working directory 
ls  # list all visible files and folders 
ls a*  # list all visible files and folders that start with 'a' 
ls ~  # list all visible files and folders from /home/user (even when the shell is somewhere else) 
ls -a  # list all files and folders 
ls -l  # list all visible files and folders in the long format 
ls -r folder  # list all visible files and folders from folder 
ls -al  # list all files and folders in the long format 
mkdir abc  # create a folder 
touch file.txt  # create file.txt
touch file{1..4}{a..d}.txt  # creates 16 files 'file1a.txt', "file1b.txt', ... 
touch file{1{a,b},2,3}.txt  # creates 4 files 'file1a.txt', "file1b.txt', 'file2.txt', 'file3.txt'
CTRL a  # jump to the beginning of the shell command 
CTRL e  # jump to the end of the shell command 
CTRL k  # delete everything in the shell command that comes after the cursor 
cp /music/songs/song_1.mp3 .  # copies the mp3 into the current directory 
cp /music/songs/song_1.mp3 /music/songs/song_2.mp3 .  # copies the two mp3s into the current directory 
mv /music/songs/song_1.mp3 .  # moves the mp3 into the current working directory 
mv /music/songs/* .  # moves the folder songs and all content to current working directory 
mv /music/songs/song_{1,2}.mp3 .  # moves the two mp3s into the current directory 
rmdir folder  # removes a directory if it is empty 
rm -r folder  # removes a folder and all its content 
rm old*  # deletes all files that start with 'old'
passwd  # change current password 
cat (vim / vi / nano / less / head / tail / ...) file.txt  # in order to read the file 
USERNAME=user_1  # sets a variable 
echo $USERNAME  # prints the variable 
echo ${USERNAME}  # prints the variable 
export PORT=8080  # sets environment variable 'PORT' to 8080
env  # shows current environment variables 
date  # prints date + local machine time 
echo The time is $( date )  # prints the line 'The time is <current date + local machine time>'
echo You are $HOME  # prints 'You are /home/user' 
echo You are \$HOME  # prints 'You are $HOME'
su - user82  # switches to another user. Of course PW will be asked if you use this command 
sudo <admissible linux command>  # stands for "super user do" 
```
