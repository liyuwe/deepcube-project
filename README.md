# deepcube-project
高级软工大作业，包括前端、后端和deepcube模型。


# 模型环境配置
1)系统依赖库安装：\
apt-get update && apt-get install -y --no-install-recommends "build-essential=12.4ubuntu1" "libboost-all-dev=1.65.1.0ubuntu1"  "libboost-dev=1.65.1.0ubuntu1" && rm -rf /var/lib/apt/lists/*

2)开发平台(安装了 conda)：\
conda install --yes python==2.7.5 tensorflow-gpu==1.8.0 && conda clean --yes --all

3)平台依赖库：\
pip install --upgrade dm-sonnet==1.10 matplotlib==2.2.3


# 整个项目启动使用命令
# 1）生成docker 容器 docker run -idt -p 8000:8000 project /bin/bash
# 2）进入prodectPy27目录，运行 python manage.py runserver 0.0.0.0:8000，启动django框架
# 或者以后台运行方式  nohup  python manage.py runserver 0.0.0.0:8000  &
# 环境配置中如果有需要，请安装django：pip install django
