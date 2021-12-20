# 项目说明

## （一）、编写代码
1、执行```npm run dev```或者```gulp``` 启动项目;       
2、打开workspace文件夹编写对应的html,css,js及img文件夹(img文件夹默认没有)下的css、js、img(这些文件夹名称不能变动)；  
## （二）、打包

完成项目后在控制台执行```npm run build```或者```gulp build```会打包你的项目至workspace/dist文件夹中并打开浏览器运行你打包后的项目；不同指令，打包的结果不一样:   

##### 1、生成sourceMap

a、npm run build 或者 gulp build ---    不压缩图片，生成sourceMap，启动打包后的项目

b、npm run build:jk 或者 gulp buildJK ---  不压缩图片，生成sourceMap，不启动打包后的项目  【Jenkins上部署时采用】

##### 2、最终会删除SourceMap文件（以便单独上传SourceMap，与线上文件名对应）
a、npm run build:rmsm 或者 gulp build:rmsm ---    不压缩图片，最终会删除SourceMap文件，以便单独上传SourceMap，与线上文件名对应，启动打包后的项目

b、npm run build:jkrmsm 或者 gulp buildJK:rmsm ---  不压缩图片，最终会删除SourceMap文件，以便单独上传SourceMap，与线上文件名对应，不启动打包后的项目  【Jenkins上部署时采用】

##### 3、不生成sourceMap
a、npm run build:nosm 或者 gulp build:nosm ---    不压缩图片，不生成sourceMap，启动打包后的项目

b、npm run build:jknosm 或者 gulp buildJK:nosm ---  不压缩图片，不生成sourceMap，不启动打包后的项目  【Jenkins上部署时采用】

##### 4、图片相关
a、npm run build:img 或者 gulp buildImg ---    压缩图片，不启动打包后的项目

b、npm run build:imgrun 或者 gulp buildImgRun --- 压缩图片，启动打包后的项目
