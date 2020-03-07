# python3_flask_demo
## learning in windows

1、mkdir Code <br>
2、django-admin startproject mysite <br>
3、python manage.py runserver <br>

1、cd mysite   <br>
2、python manage.py startapp lib <br>
3、激活模型 python manage.py makemigrations lib <br>
4、查看要执行的sql python manage.py sqlmigrate lib 0001 <br>
5、执行 python manage.py migrate <br>

setup <br>
python manage.py runserver  <br>


### 生成</br>
pip freeze > requirements.txt
### 下载</br>
* #### pip install -r requirements.txt

# Linux
#### 更改pip源码
* ~/.pip/pip.conf  （每一个我都找了都没有，所以我是在这个文件夹中创建的  pip.conf文件）
* ~/.config/pip/pip.conf

#### 修改为阿里镜像</br>
[install]</br>
trusted-host=mirrors.aliyun.com

[global]</br>
index-url=http://mirrors.aliyun.com/pypi/simple/ 

# virtualenv环境运行py项目
* python3 的 pip3</br>
pip3 install virtualenv
* 创建环境ENV</br>
virtualenv ENV
cd ENV
* 启用此环境，后续命令行前面出现（ENV）代表此时环境已切换</br>
source ./bin/activate
* 之后执行pip python3 等指令，相当于是在此环境中执行</br>
pip3 install -r /opt/flask2/requirements.txt
* 此时看到依赖已安装</br>
pip3 list
* 运行</br>
python3 /opt/flask2/flask2.py