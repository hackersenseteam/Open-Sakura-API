local set_clantag = ffi.cast("int(__fastcall*)(const char*, const char*)", memory.find_pattern("engine.dll", "53 56 57 8B DA 8B F9 FF 15"))


client.add_callback("on_paint", function()


set_clantag("Sakura.cc", "Sakura.cc")


end)
