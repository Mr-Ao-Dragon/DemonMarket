# DemonMarket 
![logo](https://raw.githubusercontent.com/Tining123/DemonMarket/master/src/main/img/logo.png)

#### A market plugin. The optimized power index function and the inverse function are used to converge the selling price. It could solve the problem of server economic imbalance caused by the high production capacity of certain items in industrial servers.
By using a convergence function based on the player's assets, items sold by the player will gradually depreciate. Items depreciate rapidly after reaching the specified baseline, and gradually decrease towards 0 but never reach 0. Using this method, players can begin to adapt to price convergence at the beginning of the entry and effectively curb the further expansion of server oligarch players' assets.

#### To prevent player from trading money by others plugin, DemonMarket will disable every command except /mt pay. 
#### You could turn this off in config.yml.

![GUI操作](https://raw.githubusercontent.com/Tining123/DemonMarket/master/src/main/img/gui_thumb2.gif)

## Usage
#### Players could use /demonmarket or /mt
+ /mt gui - Open the acquire box
+ /mt list - Show the acquire list
+ /mt sell - Sell items in your hand
+ /mt sell all - Sell items in your hand and the same things in your inventory
+ /mt pay - Pay someone money
+ /mt price - Check the price
+ /mt help - Check helps

Also ：dm, dmt, demonmarket

#### Admins could use /demonmarketadmin or /mtadmin
+ /mtadmin set [price] - Set price for the item
+ /mtadmin nbtset [price] - Set price for the nbt item
+ /mtadmin name - Check name info
+ /mtadmin nbt - Check nbt info
+ /mtadmin reload - Reload plugin

Also ：dmadmin, dmtadmin, demonmarketadmin

## Example
![5000w资产效果](https://raw.githubusercontent.com/Tining123/DemonMarket/master/src/main/img/5000w.jpg)
![60w资产效果](https://raw.githubusercontent.com/Tining123/DemonMarket/master/src/main/img/60w.jpg)
![800资产效果](https://raw.githubusercontent.com/Tining123/DemonMarket/master/src/main/img/800.jpg)
Set diamond block with $800.
- You could receive $1.6 if you have only $800
- You could receive $1.6 if you have $600000
- You could receive $1.6 if you have $50000000


## Permission
+ demonmarket.use - Player need this permission node to use demonmarket
+ If you are using Groupmanager, try /mangaddp builder demonmarket.use or /mangaddp default demonmarket.use
+ If you are using luckperm, try /lp editor 
## config.yml
+ lang: Set language manually.
+ TaxRate: Tax rate.
+ OP: The tax beneficiary. If you don't want to use it, just leave it blank.
+ BasicProperty: The average balance of single player in mathematical expectation.
+ Round: Enable and make the numbers approximate(shorter and easier to read)
+ Fitler: For SlimeFun Plugin. Enable this option to block any items with lore being sold. Attention, this might cause the NBT support disable
+ disable-pay: Enable this option to prevent user from paying others by using ess or others plugin.
+ disable-pay-list: Set the paying command you want to block.

## Mathematical Theory
+ TAX=（1 - TaxRate）

![未调优曲线图](https://raw.githubusercontent.com/Tining123/DemonMarket/master/src/main/img/chart.png)
![实际最终公式](https://raw.githubusercontent.com/Tining123/DemonMarket/master/src/main/img/math.png)

## Developing
+ Selling store [-]
+ Acquire list [-]
+ GUI support [✓]
+ NBT Support [✓]
+ Use command to set price [✓]
+ Check item name with command [✓]
## About
+ MIT lisence
+ If you have any suggestion, complain or recommend function, don't be hesitated and contact me via GitHub or spigot.
## Contact
- Github: https://github.com/Tining123/DemonMarket
- Email: tingave201@outlook.com