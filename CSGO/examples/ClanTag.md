local set_clantag_pattern = ffi.cast("int(__fastcall*)(const char*, const char*)", utils.find_signature("engine.dll", "53 56 57 8B DA 8B F9 FF 15"))


client.add_callback("on_paint", function()

set_clantag_pattern("Sakura.cc", "Sakura.cc")
      
end)
