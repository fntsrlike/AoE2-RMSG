#### 1.2.3. <ELEVATION_GENERATION>
海拔是一塊柔和且可步行的山丘（相較於峭壁）。此地形會避開玩家的起始區域。

##### Commands
```
create_elevation N(1-7)  { ... }
```

建立一或多個最高為 N 的隨機高度的山丘。一般來說，有比較大的基底的山丘容易達到更高的高度。

##### Attributes
```
base_terrain TYPE
```
山丘會生成在這個地形上。預設值是草地 `GRASS`。

```
number_of_tiles N
```
所有山丘所佔有基底的面積，預設是 100。（至少作者如此認為

```
number_of_clumps N
```
最多建立幾座明顯的山丘。預設值是一座。

```
set_scale_by_size
```
所有基礎面積受到地圖面積調整。沒有調整的值是參照 100x100 的地圖

```
set_scale_by_groups
```
山丘數量受到地圖面積調整。沒有調整的值是參照 100x100 的地圖

```
Spacing N
```
指定每一層高度之間會有多少空間。預設值是 1。數字越大所產生的山丘在每一層會有更多得平坦面積。這可以用來增加建地以及預防長斜坡的產生。