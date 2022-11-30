
# Description | 內容
The zombies have grown stronger, now they are able to heal their injuries by standing still without receiving any damage.

* [Video | 影片展示](https://youtu.be/nlPU6Xz0xWQ)

* Image | 圖示
	* Idea comes from [Counter Strike Online Zombie Regeneration](https://cso.fandom.com/wiki/Zombie_2:_Mutation#Regeneration)
        > 靈感來自CSO 殭屍模式
	    <br/>![l4d_cso_zombie_Regeneration_1](image/l4d_cso_zombie_Regeneration_1.jpg)

* Apply to | 適用於
```
L4D1
L4D2
```

* <details><summary>Changelog | 版本日誌</summary>

	* v1.3 (2022-7-17)
        * Game mode check

	* v1.2 (2022-6-10)
        * Fixed entity error when no map is running

	* v1.1 (2022-2-11)
        * Add Tank hp check in l4d1 versus mode

	* v1.0 (2021-8-29)
        * [Initial release](https://forums.alliedmods.net/showthread.php?t=334089)
</details>

* Require | 必要安裝
<br/>None

* <details><summary>ConVar | 指令</summary>

	* cfg\sourcemod\l4d_cso_zombie_regeneration.cfg
		```php
        // 0=Plugin off, 1=Plugin on.
        l4d_cso_zombie_regeneration_allow "1"

        // Boomer recover hp per second. (0=off)
        l4d_cso_zombie_regeneration_boomer_hp "10"

        // Charger recover hp per second. (0=off)
        l4d_cso_zombie_regeneration_charger_hp "80"

        // Hunter recover hp per second. (0=off)
        l4d_cso_zombie_regeneration_hunter_hp "40"

        // Jockey recover hp per second. (0=off)
        l4d_cso_zombie_regeneration_jockey_hp "50"

        // Turn off the plugin in these maps, separate by commas (no spaces). (0=All maps, Empty = none).
        l4d_cso_zombie_regeneration_map_off ""

        // Turn on the plugin in these game modes, separate by commas (no spaces). (Empty = all).
        l4d_cso_zombie_regeneration_modes ""

        // Turn off the plugin in these game modes, separate by commas (no spaces). (Empty = none).
        l4d_cso_zombie_regeneration_modes_off ""

        // Turn on the plugin in these game modes. 0=All, 1=Coop, 2=Survival, 4=Versus, 8=Scavenge. Add numbers together.
        l4d_cso_zombie_regeneration_modes_tog "0"

        // Smoker recover hp per second. (0=off)
        l4d_cso_zombie_regeneration_smoker_hp "10"

        // CSO Zombie Regeneration - Self Healing file (relative to to sound/, empty=disable)
        l4d_cso_zombie_regeneration_soundfile "ui/beep07.wav"

        // Spitter recover hp per second. (0=off)
        l4d_cso_zombie_regeneration_spitter_hp "5"

        // Tank recover hp per second. (0=off)
        l4d_cso_zombie_regeneration_tank_hp "200"

        // Seconds needed to stand still before health recovering.
        l4d_cso_zombie_regeneration_wait_time "4"
		```
</details>

* <details><summary>Command | 命令</summary>

	None
</details>

- - - -
# 中文說明
殭屍變得更強大，他們只要站著不動便可以自癒傷勢　(仿CSO惡靈降世 殭屍技能)

* 原理
    1. 只要特感不動三秒鐘之後，便能每秒回復自身血量，一旦走動或受到傷害便會停止自癒
    2. 靈感來自CSO 殭屍模式，在這款遊戲中殭屍可以自癒傷勢

* 功能
    * 可調整每個種類的特感回復血量
    * 可調整自癒音效