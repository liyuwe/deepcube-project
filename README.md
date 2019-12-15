# deepcube-project
高级软工大作业，包括前端、后端和deepcube模型。


# 模型环境配置
1)系统依赖库安装：\
apt-get update && apt-get install -y --no-install-recommends "build-essential=12.4ubuntu1" "libboost-all-dev=1.65.1.0ubuntu1"  "libboost-dev=1.65.1.0ubuntu1" && rm -rf /var/lib/apt/lists/*

2)开发平台(安装了 conda)：\
conda install --yes python==2.7.5 tensorflow-gpu==1.8.0 && conda clean --yes --all

3)平台依赖库：\
pip install --upgrade dm-sonnet==1.10 matplotlib==2.2.3


# 载入容器并进行端口映射，使得能够在虚拟机外部通过浏览器访问 :  docker run -idt -d 8000:8000  bash
# 注意，win 进入容器的命令:winpty docker exec -it 容器名 bash 
# 系统依赖django安装命令：pip install django
# django为python2
# 进入django项目目录，启动django: python manage.py runserver 0.0.0.0:8000
# 浏览器中访问的是运行容器的虚拟机的ip:8000

