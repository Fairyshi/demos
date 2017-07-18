## 在线制作：
* [http://alloyteam.github.io/gopng/](http://alloyteam.github.io/gopng/)

## 腾讯gopng_sprite: 
* [工具说明 link](http://www.alloyteam.com/2012/05/gopng-sprite-figure-synthesis-tool-another-html5-app/)


## 学习笔记：
### Css Template可定制，demo：
* 设置相对路径 Sprite relative path: ./sprite.png

* Css Template
```
    .demo_<%=name%>_outer {
	    height: <%=h%>px;
	    width: <%=w%>px;
	    overflow: hidden;
	}
	.demo_<%=name%> {
	    background: url(<%= relative_path%>) -<%=x%>px -<%=y%>px no-repeat;
	    width: 100%;
	    height: 100%;
	}
```

* 结果
```
	.demo_gur-project-11_outer {
	    height: 32px;
	    width: 32px;
	    overflow: hidden;
	}
	.demo_gur-project-11 {
	    background: url(./sprite.png) -0px -0px no-repeat;
	    width: 100%;
	    height: 100%;
	}
```

### 注意点	
* 生成后的应用主要用到background定位来取图，不用模板或修改模板后，注意两点:
    * 子图height的设置；
    * 子图display属性的设置(display:inline-block)，行内元素的高度由内容决定，如果没有内容（只有背景）的话会导致height为0，无法显示
