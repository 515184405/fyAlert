# [fyAlert](http://www.yu313.cn/unit/item/461)

多动画，多特效弹框 兼容IE8浏览器 [官网](http://www.yu313.cn/unit/item/461)


# 参数介绍

    title    :'提示', //标题
    icon     : '',
    content  : '',    //内容
    skin     : '',    //皮肤
    position : 'fixed',//定位方式
    closeBtn : true,   //是否显示关闭按钮
    type     : 1,      //type=2 为iframe
    drag     : false,   //是否开启拖动
    time     : 2000,   //当无头或无底部按钮时自动关闭时间
    shadow   : [0.3,'#000'], //遮罩
    shadowClose : true,  //是否点击遮罩关闭
    animateType : 0, // 0为默认动画 1为底部弹出 2为顶部弹出 3为左部弹出 4为右部弹出
    aniExtend: '',   //例 css动画名 opacity
    area     : ['auto','auto'], //设置宽高
    minmax   : false,
    direction: ['center','center'], //方向 key1:right left center  key2: top bottom center
    btns     : {                   //按钮组
       /* '确定' : function(){},*/
    },
    success  : function(){},  //弹出后回调
    end      : function(){}   //关闭后回调
    
 # msg调用方法

    //信息提示弹出层（图标）
    fyAlert.msg("下方弹出弹框",{icon:1,animateType:1};
    fyAlert.msg("上方弹出弹框",{icon:2,animateType:2};
    fyAlert.msg("左方弹出弹框",{icon:3,animateType:3};
    fyAlert.msg("右方弹出弹框",{icon:4,animateType:4};
    fyAlert.msg("右方弹出弹框",{icon:5,animateType:4};
    
 # alert调用方法
 
     fyAlert.alert({
        title:'文本提示框',
        content: '您觉得这个这个弹框动画怎么样',
        btns    : {                  //按钮组
              '很好' : function(obj){
                  obj.destory();   //在页面上
              },
              '不好' : function(obj){
                  obj.destory(); //销毁
              }
          },
      }) 
