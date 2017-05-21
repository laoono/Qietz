# SLICE M端模板 
项目配置文件示例:
```json
{
    // 使用的模板引擎 默认smarty
    "template": "smarty",
    // 模板选项
    "smarty": {
        // 模板变量绑定的接口字典，api url must be JSON
        "dataManifest": {
            "./templates/index.tpl": "api url",
            "./templates/article_detail.tpl": "api url"
        },
        // 每个项目单独的模板常量路径
        "constPath": "./const.json"
    },
    // 是否使用tinypng.com处理图片 默认是false
    "tinypng": false,
    // 雪碧图选项
    "spritesmith": {
        // 各图片间间距，如果设置为奇数，会强制+1以保证生成的2x图片为偶数宽高，默认 0
        "padding": 20,
        // 是否适配rem布局
        "REM": true,
        // 定义字体的基准大小
        "baseFonts2rem": "100px"
    },
    // 浏览器私有前缀配置
    "autoprefixer": {
        "browsers": [
            "> 1%",
            "last 2 versions",
            "Android >= 2.0",
            "ie > 8",
            "Firefox > 20",
            "iOS 7"
        ]
    }
}
```