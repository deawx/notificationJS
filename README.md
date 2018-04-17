# notificationJS
1º You need to import jQuery. You can do it [here](https://code.jquery.com/jquery-3.3.1.min.js) <br />
2º Import JS script <br />
3º You can try with: <br />
```
  newNotification({
    "title":"NotificationJS test!"
  })
```

## You can add more parameters
```
newNotification({
    "title":"Another NotificationJS test!",                     //Mandatory
    "status":["info" | "error" | "ok" ],                        //Optional. Info by default.
    "description":"Small description about the notification",   //Optional. None by default.    
    "link":{                                                    //Optional. None by default.
        "href":"http://google.es",                              //Mandatory if you use link parameter. None by default. 
        "text":"I'm a link"                                     //Optional. href link by default.
    },
    "time":5,                                                   //Optional. In seconds. 5 seconds by default.
    "hide":true,                                                //Optional. True by default
    "animation_duration":0.2,                                   //Optional. 0.2 seconds by default
    "showCloseIcon": false,                                     //Optional. True by default
    "newestOnTop": true,                                        //Optional. True by default
    "debug": true                                               //Optional. True by default,
    "style": ...                                                //Map of different styles you can apply. Explain below.
})
```

#### time
How long your notification will last?<br />
Values: Positives integers or doubles


#### hide
Will your notification last forever? <br />
Values: [ true | false ]

#### showCloseIcon
Will your notification close? <br />
Values: [ true | false ]

#### debug
Do you want to see logs, errors, info in the console of the browser? <br />
Values: [ true | false ]

### Styles
All options below are optional, and you can apply CSS values. If it a color, you can write: HSV,rgb or hexadecimal code. Or if it distances, you can use: px,em,rem,%... <br />
You may also apply your CSS variables if you have declared it in the root selector.<br />
In the example below, CSS values are the defaults ones.

```
newNotification({
    "title":"Let's try CSS!",
    "description":"NotificationJS is amazing",
    "style":{
      "maxWidth":"375px",                          //Width of the notification      
      "width":"calc(100vw - 80px)",                //This is just for mobile responsive                   
      "backgroundColor":"#F1F5F6",                
      "color":"#242424",                           
      "border":"none",                             
      "padding":"10px 15px",                         
      "borderRadius":"5px",                        
      "boxShadow":"0px 1px 9px 4px #242424;",                          
      "marginTop":"15px",                         
    } 
})
```

## DEMO
[https://onmax.github.io/notificationJS/](https://onmax.github.io/notificationJS/)

