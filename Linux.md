### 杀进程

- kill -9 pid

### 权限





### 解压文件

*.tar 用 tar –xvf 解压
*.gz 用 gzip -d或者gunzip 解压
*.tar.gz和.tgz 用 tar –xzf 解压
*.bz2 用 bzip2 -d或者用bunzip2 解压
*.tar.bz2用tar –xjf 解压
*.Z 用 uncompress 解压
*.tar.Z 用tar –xZf 解压
*.rar 用 unrar e解压

*.zip 用 unzip 解压

### 查看当前目录

```bash
pwd
```

### 查看当前目录所有文件

```bash
ls -a
```

### 返回上级目录

```bash
cd ..
```

### 新建目录

```bash
mkdir 目录名
```

### 删除目录

```bash
rmdir 目录名
```

### 复制目录或文件

```bash
cp 目录路径1 目录路径2
```

### 删除文件

```bash
rm 目录或文件名
```

我们常说的删库跑路就是下面这个命令， -f 就是强制删除，-r 就是递归删除

```bash
rm -rf 目录或文件名
```

删库跑路可是要负刑事责任的！小心哈

### 移动目录或文件

```bash
mv 目录路径1 目录路径2
```

### 打开文件

vi 和 vim 如果在 Linux 系统上没有的话需要单独安装， 依次运行这两个命令：`apt-get update` ，`apt-get install vim`

```bash
vi 文件名
vim 文件名
```

### 查看磁盘大小

```bash
df -h
### 显示下面的内容，这台机器是 50G 的硬盘
Filesystem      Size  Used Avail Use% Mounted on
devtmpfs        908M     0  908M   0% /dev
tmpfs           920M   24K  919M   1% /dev/shm
tmpfs           920M  504K  919M   1% /run
tmpfs           920M     0  920M   0% /sys/fs/cgroup
/dev/vda1        50G  3.3G   44G   7% /
tmpfs           184M     0  184M   0% /run/user/0
```

### 把本地文件发送到远程服务器

```bash
scp -r local_dir username@servername:remote_dir
# 如 scp -r test user@192.168.0.101:/home/data
```

