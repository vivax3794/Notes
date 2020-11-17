# COMMAND BLOCK FLOODFILL

```
execute as @e[name="floodfill"] at @s run execute if block ~ ~-1 ~ diamond_block run summon armor_stand ~1 ~ ~ {NoGravity:1, CustomName:"\"floodfill\""}
execute as @e[name="floodfill"] at @s run execute if block ~ ~-1 ~ diamond_block run summon armor_stand ~-1 ~ ~ {NoGravity:1, CustomName:"\"floodfill\""}
execute as @e[name="floodfill"] at @s run execute if block ~ ~-1 ~ diamond_block run summon armor_stand ~ ~ ~1 {NoGravity:1, CustomName:"\"floodfill\""}
execute as @e[name="floodfill"] at @s run execute if block ~ ~-1 ~ diamond_block run summon armor_stand ~ ~ ~-1 {NoGravity:1, CustomName:"\"floodfill\""}
execute as @e[name="floodfill"] at @s run execute if block ~ ~-1 ~ diamond_block run setblock ~ ~-1 ~ gold_block
execute as @e[name="floodfill"] at @s run execute if block ~ ~-1 ~ gold_block run kill @s
```

# Things to Learn
I need to learn some more stuff

## Python frameworks

 - [ ] Numpy
 - [ ] Arcade


  
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTUwNzU2MTQwMl19
-->
