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
useradd juliet  # adds the user 'juliet' 
passwd juliet  # let's you create a PW for the newly created user 
chmod WhoWhatWhich file|directory  # u,g,o,a (user, group, other, all) | +,-,= (add, remove, set exactly) | r,w,x (read, write execute) 
chmod go-rw file1 
chmod a+x file2 
chmod ### file|directory  # ### = octal code. -w---x--- = 010|001|000 = 2|1|0. rwxrw-r-- = 111|110|100 = 7|6|4. etc
chmod 664 samplefile 
chmod 750 sampledirectory 
chown student test_file  # changes the owner of 'test_file' to student 
chown -R student test_directory  # changes the owner of 'test_directory' and all subfiles & subfolders to students 
chown visitor:guests test_file  # changes the owner of 'test_file' to user 'visitor' and to group 'guests' 
chown :guests test_file  # changes the owner of 'test_file' to group 'guests' 
chgr guests test_file  # changes the owner of 'test_file' to group 'guests' 
top  # places a watcher on running processes which consume the most resources at the given moment. Exit with 'q' 
ps aux  # lists all running processes 
ps lax  # lists all running processes 
ps -ef  # lists all running processes 
ps j  # lists all running processes 
watch <valid linux command>  # places a watch stream on a linux command 
```
