# 樱花MC开放API
## 1. 使用'Jar脚本系统'进行开发 ##

1.添加@Inject(name, developer, version)来定义脚本主类 例如
@Inject("Sample", "Timeline", 1)
public class Sample {
}
2.为class贯彻API方法 例如
@Inject("Sample", "Timeline", 1)
public class Sample implements API {
@Override
public void onLoad() // 在载入脚本时会引用的方法
{
}

@Override
public List<ModuleCore> modules() // 用于返回模块
{
  return null;
}
  
@Override
public List<CMDCore> commands() // 用于返回指令
{
  return null;
}
}

例如 我想要编写一个在游戏内每次打开模块都会发送一个'Hello World!'的脚本

@Inject("Sample", "Timeline", 1)
public class Sample implements API {
@Override
public void onLoad() // 在载入脚本时会引用的方法
{
}

@Override
public List<ModuleCore> modules() // 用于返回模块
{
  return Arrays.asList(new Test());
}
  
@Override
public List<CMDCore> commands() // 用于返回指令
{
  return null;
}
}
  
@RegisterModule(name = "TEST MODULE", type = ModuleType.Misc)
class Test extends ModuleCore // 添加一个新的Class
{
    @Override
    public void onEnable()
    {
        mc.player.sendChatMessage("Hello World!");
    }
}
