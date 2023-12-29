<h1 align="center">

EF Inventory

</h1>

<h1 align="center"> Previews </h1>

![for github](https://github.com/blastersuraj/ef-inventory/assets/104319683/caf3dff6-700b-42c0-82f4-b5de838326b5)

![SPOILER_image](https://github.com/blastersuraj/ef-inventory/assets/104319683/9df23add-f818-492d-9d7f-ca6734ec599b)
![image](https://github.com/blastersuraj/ef-inventory/assets/104319683/30e11608-5544-4143-90f7-565aea384ee6)

<h1 align="center"> Key Features </h1>

<ul>
  <li>Item Doubling Exploit Fixed</li>
  <li>Right Click To Use Item</li>
  <li>Right Click To Give Item</li>
  <li>Givem Item on Specific Player ID (Optional change in Config.lua)</li>
  <li>Player Stats on Inventory Section (Optional change in Config.lua)</li>
  <li>Server Logo in Inventory Section (Optional change in Config.lua)</li>
  <li>User PC Real Time in Inventory Section (Optional change in Config.lua)</li>
  <li>Clean UI & Optimized</li>
  <li>Runs at ~ 0.00 to 0.01 ms</li>
  <li>Blurred inventory background</li>
  <li>Weight progress bar</li>
  <li>ALL Images follow the same Dimensions (100px X 100px)</li>
  <li>Decay System</li>
</ul>

# Set up the decay system

<h3> Here is the way to add decay in your Items</h3> <br>

Add the Decay Value In ```qb-core/shared/items.lua``` <br>

# Example
Decay Value in core (the variable stands for the number of days it takes to decay)

```lua
["decay"] = 28.0,
```
<br>

you can also add Delete System to delete the item after the decay time

```lua
["delete"] = true
```

<h3> Complete Example to Add Decay in your Items </h3><br>
<h3> Add your Item Like This </h3>

```lua
['battery'] = {['name'] = 'battery', ['label'] = 'Battery', ['weight'] = 2000, ['type'] = 'item', ['image'] = 'battery.png', ['unique'] = true, ['useable'] = true, ['shouldClose'] = true,	['combinable'] = nil, ['description'] = 'Heavy Battery to charge you Devices', ["decay"] = 3.0, ["delete"] = true},
```
<h4> as per this example means the Battery will Despawn/Delete or you can say not useable after 3 days </h4>




