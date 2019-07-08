# Node-RED Storing Data 
Storing Data for Node-RED Variables Tutorial

Context Method
-----
```javascript
var cont1 = context.get('cont') || 0;
cont1 += 1;
msg.counter = "Counter Context = " + cont1;
context.set('cont',cont1);
return msg;
```

Flow Method
-----
```javascript
var cont1 = flow.get('flow') || 0;
cont1 += 1;
msg.counter = "Counter Flow = " + cont1;
context.set('flow',cont1);
return msg;
```

Global Method
-----
```javascript
var cont1 = global.get('glob') || 0;
cont1 += 1;
msg.counter = "Counter Flow = " + cont1;
context.set('glob',cont1);
return msg;
```

![Flow 1](https://github.com/esen2202/NodeREDStoringData/blob/master/Captures/Node-RED%20-8.07.2019%2021_40_26.png?raw=true)


![Flow 2](https://github.com/esen2202/NodeREDStoringData/blob/master/Captures/Node-RED%20-%208.07.2019%2021_41_15.png?raw=true)
