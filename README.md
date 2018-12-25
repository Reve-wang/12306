#### 12306抢票代码

- python版本支持
  - 2.7.10 - 2.7.15
- 依赖库
  - 依赖若快 若快注册地址：http://www.ruokuai.com/client/index?6726 推荐用若快，打码兔平台已经关闭
  - 项目依赖包 requirements.txt
  - 安装方法 pip install -i https://pypi.tuna.tsinghua.edu.cn/simple -r requirements.txt

- 项目使用说明
  - 需要配置邮箱，可以配置可以不配置，配置邮箱的格式在yaml里面可以看到ex
  - 提交订单验证码哪里依赖打码兔，所以如果是订票遇到验证码的时候，没有打码兔是过不了的，不推荐手动，手动太慢
  - 配置yaml文件的时候，需注意空格和遵循yaml语法格式

- 项目开始
  - 服务器启动:
      - 修改config/ticket_config.yaml文件，按照提示更改自己想要的信息
      - 运行根目录run.py，即可开始
  - 如果你的服务器安装了docker，那么就可以docker启动
      - 1、docker build -t dockerticket .
      - 2、docker run dockerticket && python run.py 


- 目录对应说明
  - agency - cdn代理
  - config - 项目配置
  - damatuCode - 打码兔接口
  - init - 项目主运行目录
  - myException - 异常
  - myUrllib - urllib库

- 思路图
     ![image](https://github.com/testerSunshine/12306/blob/master/uml/uml.png)

- 项目声明：
  - 本软件只供学习交流使用，务作为商业用途
  - 能为你抢到一张回家的票，是我最大的心愿
