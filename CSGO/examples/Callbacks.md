## `CreateMove`
CreateMove callback

    client.add_callback("on_createmove", function(user_cmd)
        
    end)

Paint callback

    client.add_callback("on_paint", function()
        
    end)

Shot callback

    client.add_callback("on_shot", function(shot_info)
        
    end)

Resolver callback

    client.add_callback("on_resolver", function(isYaw, beforeAnimYaw_Pitch, eyeYaw_Pitch, maxDesyncDelta, targetName, misses, targetShooting)
        
    end)

CS:GO Event callback

    events.register_event("player_hurt", function(event)
        
    end)
