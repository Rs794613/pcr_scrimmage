# pcr大乱斗
一个基于hoshino_bot的小游戏，玩法类似大富翁<br>
目前有两个版本，一个是贵族决斗版 pcr_scrimmage_duel ，一个普通版 pcr_scrimmage<br>
贵族版决出胜利者后可按排名获得贵族决斗游戏的金币<br>
**该项目随时都有可能更新或修复bug，详情查看commits**

## 安装
将 pcr_scrimmage 这个文件夹直接丢到hoshino里的moudle里，然后在__bot__.py里的MODULES_ON加上"pcr_scrimmage"即可<br>
如要安装贵族版，则将 pcr_scrimmage_duel 里的两个文件放到 pcr_scrimmage 文件夹里覆盖即可。<br>
**关于贵族版的问题，需要加上贵族决斗作者魔改的猜头像附带的daylimiter，详情请看[这里](https://github.com/Rs794613/PcrDuel/releases)的Games.add.gold.zip**

## 规则概括
1. 和大富翁类似，一个正方形环形跑道，跑道上有多个事件，通过丢色子走到特定的位置触发事件
2. 可多个玩家同时玩，最多4个，最少2个。每个玩家可选择一个pcr里的角色，不同的角色有不同的属性、技能
3. 角色有tp值，每次投掷色子，所有玩家都会增加tp值，tp达到技能的要求可释放技能
4. 需要选择目标的技能释放范围有距离限制，以角色属性的攻击距离为准
5. 避免游戏时长过长，每4回合增加一次攻击力和攻击距离
6. 活到最后获胜（吃鸡？）

## 指令表
### 基础命令：
1. #### 大乱斗规则<br>
	可查看大乱斗相关规则<br>
2. #### 大乱斗角色<br>
	可查看所有可用角色<br>
3. #### 角色详情 （角色名）<br>
	如：**角色详情 黑猫**<br>
	可查看角色的基础属性和技能<br>
4. #### 结束大乱斗<br>
	可以强制结束正在进行的大乱斗游戏<br>
	（该命令只有管理员和房主可用）<br>
### 创建阶段：
1. #### 创建大乱斗<br>
2. #### 加入大乱斗<br>
3. #### 开始大乱斗<br>
### 选择角色阶段：
1. #### （角色名）<br>
	如：**凯露 / 黑猫**<br>
	（名字和外号都行）<br>
### 对战阶段：
1. #### 丢色子<br>
2. #### （技能编号） @xxx<br>
	如：**1 @xxx**<br>
	发送技能编号并@目标，如果这个技能不需要指定目标，直接发送技能编号即可<br>
3. #### 查看属性<br>
	可查看自己当前角色详细属性<br>
4. #### 投降 / 认输<br>

## 自定义
游戏内的跑道事件、角色、技能效果都可自定义，详情看 runway_case.py 和 role.py 的顶部注释<br>

## 其它
代码写得很烂，要伤害一下各位的眼睛了orz<br>
测试得比较少，可能存在非常多的bug<br>
目前已有角色不多，且数值不平衡<br>
（十分渴望优化建议或提出bug orz ）

## 感谢
十分感谢hoshino bot的创造者和各位做bot开发的老前辈们<br>
[HoshinoBot](https://github.com/Ice-Cirno/HoshinoBot)<br>
[HoshinoBot 作品索引](https://github.com/pcrbot/HoshinoBot-plugins-index)
