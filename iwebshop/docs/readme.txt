
目前最新的iwebshop2.6版本就已经融入了多客户端，即手机端的判定，可以让一套系统自动识别不同的客户端进行展示！
具体实现方法：
1，在config/config.php中的theme和skin属性写成数组的格式，比如：theme => array('pc' => 'default','mobile' => 'mobile_theme')，此时只要在views目录下开发一套mobile_theme也就是手机主题，那么当客户端为手机用户访问的时候，就会自动访问mobile_theme主题了。对于客户端的判断在lib/util/client.php中的getDevice()方法，用户可以自由扩展，源码100%开放！
