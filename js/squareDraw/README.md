正方形抽奖转盘组件
=========

参数说明：

- id_dom：元素ID
- prize_arr：奖品的数组（从左上角开始，顺时针一圈）
- round_count：旋转圈数
- normal_speed：默认旋转速度
- up_speed：中途加速
- start_point：加速点
- end_point：减速点 【最好要小于-（奖品个数*圈数的大小）】


----------



    //首先new一个抽奖类
       var lottery=new squareDraw({
           "id_dom":"lottery_gift",
           "prize_arr":['a','b','c','d','e','f','g','h','i','j','k','l','m','n','o','p','q','r','s','t'],
           "round_count":2,
           "normal_speed":400,
           "up_speed":100,
           "start_point":6,
           "end_point":38,
           "show_result":function(prize_name){
                console.log("恭喜你中了"+prize_name);
           }
       })


    //调用抽奖类的-转动方法
    lottery.set_prize(prize);