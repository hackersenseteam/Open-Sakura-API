## `Pre_Prediction`
Pre_Prediction callback

    client.add_callback("on_preprediction", function(user_cmd)
        
    end)
    
 ## `Prediction`
Prediction callback

    client.add_callback("on_prediction", function(user_cmd)
        
    end)
    
## `CreateMove`
CreateMove callback

    client.add_callback("on_createmove", function(user_cmd)
        
    end)

## `PaintTraverse`
Paint callback

    client.add_callback("on_paint", function()
        
    end)

## `Shooting`
Shot callback

    client.add_callback("on_shot", function(shot_info)
        
    end)

## `Resolver`
Resolver callback

    client.add_callback("on_resolver", function(resolver_info)
        
    end)

## `Event`
CS:GO Event callback

    events.register_event("player_hurt", function(event)
        
    end)
