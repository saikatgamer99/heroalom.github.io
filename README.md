<?xml version="1.0" encoding="UTF-8" ?>
<!DOCTYPE html>
<html b:css='false' b:defaultwidgetversion='2' b:layoutsVersion='3' b:responsive='true' b:templateVersion='2.0.0' expr:class='data:blog.languageDirection' expr:dir='data:blog.languageDirection' expr:lang='data:blog.localeUnderscoreDelimited' xmlns='http://www.w3.org/1999/xhtml' xmlns:b='http://www.google.com/2005/gml/b' xmlns:data='http://www.google.com/2005/gml/data' xmlns:expr='http://www.google.com/2005/gml/expr'>
<b:with value='data:view.isSearch and (data:view.url == data:view.url params { amp: &quot;1&quot; })' var='isFeed'>
<head>
<b:include name='pbt-head'/>
<b:if cond='!data:view.isLayoutMode and !data:isFeed'>
<b:skin version='2.0.0'><![CDATA[/*
-----------------------------------------------
Blogger Template Style
Name:         SmartMag
Version:      1.0.0 - Free
Author:       Pro Blogger Templates
Author Url:   https://probloggertemplates.com/
-----------------------------------------------*/

/*-- Customize Options (Start) --
<Variable name="keycolor" description="Main Color" type="color" default="#3b82f6" value="#3b82f6"/>
<Group description="Layout Options" selector="body">
	  <Variable name="boxedMode" description="Enable Boxed Mode" type="length" default="0px" min="0px" max="1px" value="0px"/>
    <Variable name="row.width" description="Container Width" type="length" default="970px" min="970px" max="1094px" value="970px"/>
    <Variable name="sidebar.width" description="Sidebar Width" type="length" default="300px" min="250px" max="336px" value="300px"/>
    <Variable name="border.radius" description="Rounded Corner" type="length" default="8px" min="2px" max="12px" value="8px"/>
    <Variable name="stickyMenu" description="Enable Sticky Header" type="length" default="1px" min="0px" max="1px" value="1px"/>
    <Variable name="stickySidebar" description="Enable Sticky Sidebar" type="length" default="1px" min="0px" max="1px" value="1px"/>
</Group>
<Group description="Fonts" selector="body">
    <Variable name="main.font" description="Main Font" type="font" family="Montserrat" default="normal 400 14px $(family)" value="normal 400 14px $(family)"/>
    <Variable name="title.font" description="Title Font" type="font" family="Montserrat" default="normal 400 14px $(family)" value="normal 400 14px $(family)"/>
    <Variable name="text.font" description="Text Font" type="font" family="Montserrat" default="normal 400 14px $(family)" value="normal 400 14px $(family)"/>
</Group>
<Group description="Background" selector="body">
	  <Variable name="background.color" description="Body Background (Boxed)" type="color" default="#f1f5f9"  value="#f1f5f9"/>
    <Variable name="outer.bg" description="Outer Background" type="color" default="#f8fafc"  value="#f8fafc"/>
    <Variable name="widget.bg" description="Widget Background" type="color" default="#ffffff" value="#ffffff"/>
</Group>
<Group description="Colors" selector="body">
    <Variable name="accent.color" description="Accent Color" type="color" default="#3b82f6" value="#3b82f6"/>
    <Variable name="title.color" description="Title Color" type="color" default="#0f172a" value="#0f172a"/>
    <Variable name="title.hover.color" description="Title Hover Color" type="color" default="$(accent.color)" value="#3b82f6"/>
    <Variable name="text.color" description="Text Color" type="color" default="#475569"  value="#475569"/>
    <Variable name="meta.color" description="Meta Color" type="color" default="#94a3b8" value="#94a3b8"/>
</Group>
<Group description="Gradient Style" selector="body">
	  <Variable name="gradient" description="Enable Gradient" type="length" default="1px" min="0px" max="1px" value="1px"/>
    <Variable name="gradient.from" description="Background (From)" type="color" default="$(accent.color)" value="#3b82f6"/>
    <Variable name="gradient.to" description="Background (To)" type="color" default="#d946ef" value="#d946ef"/>
</Group>
<Group description="Border Top" selector="body">
    <Variable name="border.top" description="Height" type="length" default="5px" min="0px" max="8px" value="5px"/>
    <Variable name="border.top.bg" description="Background" type="color" default="$(accent.color)" value="#3b82f6"/>
</Group>
<Group description="Header" selector=".site-header">
    <Variable name="header.height" description="Height" type="length" default="62px" min="50px" max="70px" value="62px"/>
    <Variable name="header.bg" description="Background" type="color" default="#ffffff" value="#ffffff"/>
    <Variable name="header.color" description="Color" type="color" default="$(title.color)" value="#0f172a"/>
    <Variable name="header.hover.color" description="Hover Color" type="color" default="$(accent.color)" value="#3b82f6"/>
</Group>
<Group description="Sub Menu" selector=".site-header">
    <Variable name="submenu.bg" description="Background" type="color" default="#ffffff" value="#ffffff"/>
    <Variable name="submenu.color" description="Color" type="color" default="$(title.color)" value="#0f172a"/>
    <Variable name="submenu.hover.color" description="Hover Color" type="color" default="$(accent.color)" value="#3b82f6"/>
</Group>
<Group description="Blog Posts" selector="#main">
    <Variable name="gridStyle" description="Enable Grid Style" type="length" default="0px" min="0px" max="1px" value="0px"/>
    <Variable name="postSummary" description="Show Summary" type="length" default="1px" min="0px" max="1px" value="1px"/>
    <Variable name="postCategory" description="Show Category" type="length" default="1px" min="0px" max="1px" value="1px"/>
</Group>
<Group description="Post Page" selector="body">
    <Variable name="breadcrumb" description="Show Breadcrumbs" type="length" default="1px" min="0px" max="1px" value="1px"/>
    <Variable name="itempost.title.size" description="Title Font Size" type="length" default="35px" min="20px" max="50px" value="35px"/>
    <Variable name="itempost.content.size" description="Content Font Size" type="length" default="14px" min="12px" max="20px" value="14px"/>
    <Variable name="postnav" description="Show Navigation" type="length" default="1px" min="0px" max="1px" value="1px"/>
</Group>
<Group description="Footer" selector=".site-footer">
    <Variable name="footer.bg" description="Background" type="color" default="#1e293b" value="#1e293b"/>
    <Variable name="footer.color" description="Color" type="color" default="#f8fafc" value="#f8fafc"/>
    <Variable name="footer.hover.color" description="Hover Color" type="color" default="$(accent.color)" value="#3b82f6"/>
    <Variable name="footer.text.color" description="Text Color" type="color" default="#cbd5e1" value="#cbd5e1"/>
</Group>
<Group description="Footer Bar" selector=".footer-bar">
    <Variable name="footerbar.bg" description="Background" type="color" default="#0f172a" value="#0f172a"/>
    <Variable name="footerbar.color" description="Color" type="color" default="#f8fafc" value="#f8fafc"/>
    <Variable name="footerbar.hover.color" description="Hover Color" type="color" default="$(accent.color)" value="#3b82f6"/>
</Group>
<Group description="Miscellaneous" selector="body">
    <Variable name="btn.bg" description="Button Background" type="color" default="$(accent.color)" value="#3b82f6"/>
    <Variable name="btn.color" description="Button Color" type="color" default="#ffffff"  value="#ffffff"/>
    <Variable name="rgba" description="RGBA Key (Overlay)" type="color" default="#0f172a"  value="#0f172a"/>
    <Variable name="browser.bg" description="Browser Tab Background" type="color" default="#0f172a"  value="#0f172a"/>
</Group>
<Variable name="body.background" description="Background" type="background" color="$(background.color)" default="$(color) none repeat fixed top left" value="$(color) none repeat fixed top left"/>
<Variable name="body.background.color" description="Comments Background" hideEditor="true" type="color" default="transparent"  value="transparent"/>
<Variable name="body.title.color" description="Comments Color" hideEditor="true" type="color" default="$(title.color)" value="#0f172a"/>
<Variable name="body.text.color" description="Comments Text Color" hideEditor="true" type="color" default="$(text.color)"  value="#475569"/>
<Variable name="body.link.color" description="Comments Link Color" hideEditor="true" type="color" default="$(accent.color)"  value="#3b82f6"/>
<Variable name="body.text.font" description="Comments Font 1" hideEditor="true" type="font" default="normal 400 14px roboto, Arial, sans-serif !important"  value="normal 400 14px roboto, Arial, sans-serif !important"/>
<Variable name="body.action.font.large" description="Comments Font 2" hideEditor="true" type="font" default="normal 700 14px roboto, Arial, sans-serif !important"  value="normal 700 14px roboto, Arial, sans-serif !important"/>
-- Customize Options (End) --*/

/*-- CSS Variables --*/
:root{
--body-font:$(main.font.family), sans-serif;
--menu-font:$(main.font.family), sans-serif;
--title-font:$(title.font.family), sans-serif;
--text-font:$(text.font.family), sans-serif;
--icon-font:"bootstrap-icons", bootstrap-icons;
--body-bg-color:$(background.color);
--body-bg:$(body.background);
--outer-bg:$(outer.bg);
--widget-bg:$(widget.bg);
--accent-color:$(accent.color);
--accent-color-10:$(accent.color)10;
--title-color:$(title.color);
--title-hover-color:$(title.hover.color);
--text-color:$(text.color);
--meta-color:$(meta.color);
--border-top-bg:$(border.top.bg);
--header:$(header.height);
--header-bg:$(header.bg);
--header-color:$(header.color);
--header-hover-color:$(header.hover.color);
--submenu-bg:$(submenu.bg);
--submenu-color:$(submenu.color);
--submenu-hover-color:$(submenu.hover.color);
--footer-bg:$(footer.bg);
--footer-color:$(footer.color);
--footer-hover-color:$(footer.hover.color);
--footer-text-color:$(footer.text.color);
--footerbar-bg:$(footerbar.bg);
--footerbar-color:$(footerbar.color);
--footerbar-hover-color:$(footerbar.hover.color);
--gradient:var(--accent-color);
--modal-bg:var(--widget-bg);
--button-bg:$(btn.bg);
--button-color:$(btn.color);
--h-weight:700;
--gap: 30px;
--deg:45deg;
--gray-bg:$(rgba)08;
--overlay-bg:$(rgba)80;
--border-color:$(rgba)0d;
--shadow:0 1px 2px $(rgba)0d;
--radius:$(border.radius);
}

html.rtl{
--body-font:Cairo, sans-serif;
--menu-font:Cairo, sans-serif;
--title-font:Cairo, sans-serif;
--text-font:Cairo, sans-serif;
--deg:-45deg;
}

.is-gradient{
--gradient:linear-gradient(var(--deg),$(gradient.from),$(gradient.to));
--border-top-bg:var(--gradient);
--button-bg:var(--gradient);
--button-color:#fff;
}

/*-- Reset CSS --*/
html,body,a,abbr,acronym,address,applet,b,big,blockquote,caption,center,cite,code,dd,del,dfn,div,dl,dt,em,fieldset,font,form,input,button,h1,h2,h3,h4,h5,h6,i,iframe,img,ins,kbd,label,legend,li,object,p,pre,q,s,samp,small,span,strike,strong,sub,sup,table,tbody,td,tfoot,th,thead,tr,tt,u,ul,var{padding:0;margin:0;border:0;outline:none;vertical-align:baseline;background:0 0;text-decoration:none}dl,ul{list-style-position:inside;list-style:none}ul li{list-style:none}caption{text-align:center}img{border:none;position:relative}a,a:visited{text-decoration:none}.clearfix{clear:both}.section,.widget,.widget ul{margin:0;padding:0}a{color:var(--accent-color)}a img{border:0}abbr{text-decoration:none}.separator a{text-decoration:none!important;clear:none!important;float:none!important;margin-left:0!important;margin-right:0!important}#Navbar1,#navbar-iframe,.widget-item-control,a.quickedit,.home-link,.feed-links{display:none!important}.center{display:table;margin:0 auto;position:relative}.widget > h2,.widget > h3{display:none}.widget iframe,.widget img{max-width:100%}button,input,select,textarea{background:transparent;font-family:var(--body-font);font-weight:normal;-webkit-appearance:none;-moz-appearance:none;appearance:none;outline:none;border-radius:0}button{cursor:pointer}input[type="search"]::-webkit-search-cancel-button{-webkit-appearance:none}.rtl{direction:rtl}iframe[src*="youtube.com"]{width:100%;height:auto;aspect-ratio:16/9}

/*-- Main CSS --*/
*{box-sizing:border-box}
*:after,*:before{display:inline-block;font-family:var(--icon-font);font-weight:400;font-style:normal;box-sizing:border-box}
html{position:relative;word-break:break-word;word-wrap:break-word;text-rendering:optimizeLegibility;-webkit-font-smoothing:antialiased;-webkit-text-size-adjust:100%}
body{position:relative;background:var(--body-bg);background-color:var(--body-bg-color);font-family:var(--body-font);font-size:14px;color:var(--text-color);font-weight:400;font-style:normal;line-height:1.4em}
h1,h2,h3,h4,h5,h6{font-family:var(--title-font);font-weight:var(--h-weight)}
a,input,textarea,button{transition:all .0s ease}
.site-outer{display:flex;flex-direction:column;justify-content:flex-start;position:relative;overflow:hidden;width:100%;max-width:100%;background:var(--outer-bg);margin:0 auto;padding:0}
.is-boxed .site-outer{width:calc($(row.width) + (var(--gap) * 2));max-width:100%;box-shadow:0 0 15px $(rgba)0d}
.container{position:relative}
.row-x1{width:$(row.width);max-width:100%}
.flex-c{display:flex;justify-content:center}
.flex-col{display:flex;flex-direction:column}
.flex-sb{display:flex;justify-content:space-between}
.content-wrap{position:relative;margin:var(--gap) 0 0}
.is-left .content-wrap > .container,.rtl .is-right .content-wrap > .container{flex-direction:row-reverse}
.rtl .is-left .content-wrap > .container{flex-direction:row}
.pbtStickySidebar:before,.pbtStickySidebar:after{content:"";display:table;clear:both}
.main-wrap{position:relative;width:calc(100% - ($(sidebar.width) + var(--gap)))}
.no-sidebar .main-wrap{width:100%}
.sidebar-wrap{position:relative;width:$(sidebar.width)}
.no-sidebar .sidebar-wrap{display:none}
.entry-thumbnail,.entry-avatar,.comments .avatar-image-container{display:block;position:relative;overflow:hidden;background:var(--gray-bg);z-index:5;border-radius:var(--radius)}
.thumbnail,.avatar{display:block;position:relative;width:100%;height:100%;background-size:cover;background-position:center center;background-repeat:no-repeat;z-index:1;transform-origin:center;opacity:0;transition:opacity .35s ease}
.thumbnail.pbt-lazy,.avatar.pbt-lazy{opacity:1}
a.entry-thumbnail:hover .thumbnail,.entry-inner:hover .thumbnail{filter:brightness(1.05)}
.entry-thumbnail .entry-tag{display:flex;align-items:center;position:absolute;top:20px;left:20px;max-width:fit-content;height:20px;background:var(--button-bg);font-size:12px;color:var(--button-color);font-weight:400;z-index:5;padding:0 8px;border-radius:var(--radius)}
.rtl .entry-thumbnail .entry-tag{left:unset;right:20px}
[class*="yt-img"]:after{display:flex;align-items:center;justify-content:center;content:"\f4f4";position:absolute;right:50%;bottom:50%;width:36px;height:28px;background:var(--button-bg);font-size:22px;color:var(--button-color);text-shadow:2px 2px 0 rgba(0,0,0,.05);z-index:3;padding:0 0 0 2px;border-radius:var(--radius);transform:translate(50%,50%)}
.yt-img\:x1:after{transform:translate(50%,50%) scale(1.1)}
.yt-img\:x2:after{transform:translate(50%,50%) scale(.95)}
.yt-img\:x3:after{transform:translate(50%,50%) scale(.75)}
.yt-img\:x4:after{transform:translate(50%,50%) scale(.65)}
.entry-header{display:flex;flex-direction:column;gap:4px}
.post:not(.cs) .entry-header .entry-tag{font-size:13px;color:var(--accent-color);font-weight:600;text-transform:uppercase}
.entry-title{color:var(--title-color);line-height:1.3em}
.entry-title a{display:-webkit-box;-webkit-line-clamp:3;-webkit-box-orient:vertical;overflow:hidden;color:var(--title-color)}
.entry-title a:hover{color:var(--title-hover-color)}
.entry-meta{display:flex;flex-wrap:wrap;gap:4px;font-size:12px;color:var(--meta-color);line-height:1.3em}
.entry-meta > span{display:flex;gap:4px}
.entry-meta .author-name{color:var(--title-color);font-weight:600}
.excerpt{font-family:var(--text-font);color:var(--text-color);line-height:1.5em}
.cs .entry-inner{display:block;position:relative;width:100%;height:100%;overflow:hidden;z-index:10;box-shadow:var(--shadow);border-radius:var(--radius)}
.cs .entry-thumbnail{width:100%;height:100%}
.cs .entry-thumbnail:before{content:"";position:absolute;top:0;left:0;right:0;bottom:0;background:linear-gradient(var(--deg),$(rgba) 0%,$(rgba)1a 100%);-webkit-backface-visibility:hidden;backface-visibility:hidden;z-index:2;opacity:.5;transition:opacity .25s ease}
.is-gradient .cs .entry-thumbnail:before{background:linear-gradient(var(--deg),$(gradient.from) 0%,$(gradient.to)66 100%);opacity:1}
.cs .yt-img:after{top:20px;right:20px;transform:translate(0)}
.rtl .cs .yt-img:after{left:20px;right:unset}
.cs .entry-header{position:absolute;left:0;bottom:0;width:100%;overflow:hidden;text-shadow:0 1px 2px $(rgba)1a;z-index:10;padding:20px;gap:6px}
body:not(.is-gradient) .cs .entry-header{background:linear-gradient(to top,$(rgba)80 0%,$(rgba)00 100%)}
body.is-gradient .cs .entry-tag{font-size:12px;color:#fff;font-weight:500;line-height:1.3em;text-transform:uppercase}
body:not(.is-gradient) .cs .entry-tag{display:flex;align-items:center;max-width:fit-content;height:20px;background:var(--button-bg);font-size:12px;color:var(--button-color);font-weight:400;text-shadow:none;padding:0 6px;margin:0 0 2px;border-radius:var(--radius)}
.cs .entry-title{display:-webkit-box;overflow:hidden;-webkit-line-clamp:3;-webkit-box-orient:vertical;color:#fff}
.cs .entry-meta,.cs .entry-meta .author-name{color:#f8fafc}
.cs .entry-meta .author-name{font-weight:500}
.btn{position:relative;border-radius:var(--radius)}
.loader{display:flex;align-items:center;justify-content:center;position:relative;width:100%;height:100%;font-size:34px}
.spinner{width:1em;height:1em;z-index:2;animation:rotate 2s linear infinite}
.spinner .path{fill:none;stroke-width:3px;stroke:var(--accent-color);stroke-linecap:round;animation:dash 1.5s ease-in-out infinite}
@keyframes rotate{100%{transform:rotate(360deg)}}
@keyframes dash{0%{stroke-dasharray:1,150;stroke-dashoffset:0}50%{stroke-dasharray:90,150;stroke-dashoffset:-35}100%{stroke-dasharray:90,150;stroke-dashoffset:-124}}
.error-msg{display:flex;align-items:center;font-size:14px;color:var(--meta-color);padding:20px 0;font-weight:400}
.overlay-bg{visibility:hidden;opacity:0;position:fixed;top:0;left:0;right:0;bottom:0;background:var(--overlay-bg);-webkit-backdrop-filter:blur(2px);backdrop-filter:blur(2px);z-index:1000;margin:0;transition:all .25s ease}
.overlay-bg.ms17{transition:all .17s ease}
.social a:before{text-shadow:3px 2px 0 rgba(0,0,0,.05)}
.social .blogger a:before{content:"\f1a6"}
.social .rss a:before{content:"\f521"}
.social .share a:before{content:"\f52d"}
.social .email a:before{content:"\f32c"}
.social .website a:before{content:"\f3ef"}
.social .external-link a:before{content:"\f1c5"}
.color .blogger a{color:#1a73e8}
.color .blogger a{color:#ff5722}
.color .apple a{color:#333}
.color .amazon a{color:#fe9800}
.color .microsoft a{color:#0067B8}
.color .facebook a,.color .facebook-f a{color:#3b5999}
.color .twitter a{color:#00acee}
.color .youtube a{color:#e60023}
.color .instagram a{color:#dd277b;--instagram:linear-gradient(15deg,#ffb13d,#dd277b,#4d5ed4)}
.color .pinterest a,.color .pinterest-p a{color:#e60023}
.color .dribbble a{color:#ea4c89}
.color .linkedin a{color:#0077b5}
.color .twitch a{color:#9147ff}
.color .rss a{color:#ffc200}
.color .skype a{color:#00aff0}
.color .stumbleupon a{color:#eb4823}
.color .vk a{color:#4a76a8}
.color .stack-overflow a{color:#f48024}
.color .github a{color:#24292e}
.color .soundcloud a{color:#ff7400}
.color .behance a{color:#191919}
.color .digg a{color:#1b1a19}
.color .delicious a{color:#0076e8}
.color .codepen a{color:#000}
.color .flipboard a{color:#f52828}
.color .reddit a{color:#ff4500}
.color .whatsapp a{color:#3fbb50}
.color .messenger a{color:#0084ff}
.color .snapchat a{color:#ffe700}
.color .telegram a{color:#179cde}
.color .steam a{color:#112c5b}
.color .discord a{color:#7289da}
.color .quora a{color:#b92b27}
.color .tiktok a{color:#fe2c55}
.color .line a{color:#07b53b}
.color .share a{color:var(--meta-color)}
.color .email a{color:#888}
.color .website a{color:var(--title-color)}
.color .external-link a{color:var(--title-color)}
.site-header{position:relative;z-index:50;box-shadow:var(--shadow)}
.border-top{position:relative;float:left;width:100%;height:$(border.top);background:var(--border-top-bg)}
.main-header,.header-inner,.header-header{float:left;width:100%;height:var(--header);background:var(--header-bg)}
.header-inner{background:transparent}
.header-inner.is-fixed{position:fixed;top:calc(0px - (var(--header) * 2));left:0;width:100%;z-index:990;backface-visibility:hidden;visibility:hidden;opacity:0;transform:translate3d(0,0,0);transition:all .35s ease-in-out}
.header-inner.is-fixed.show{visibility:visible;opacity:1;transform:translate3d(0,calc(var(--header) * 2),0)}
.is-fixed .header-header{box-shadow:var(--shadow)}
.is-boxed .header-header{float:none;width:calc($(row.width) + (var(--gap) * 2));max-width:100%;margin:0 auto}
.header-items{position:relative;display:flex;flex-wrap:wrap;justify-content:space-between}
.flex-left{display:flex;align-items:center;gap:28px;z-index:15}
.flex-right{display:flex;align-items:center;position:absolute;top:0;right:0;height:var(--header);z-index:15}
.rtl .flex-right{left:0;right:unset}
.main-logo{display:flex;align-items:center;flex-shrink:0;height:var(--header);overflow:hidden}
.main-logo img{display:block;max-height:40px}
.main-logo .title{max-width:100%;font-family:var(--title-font);font-size:25px;color:var(--header-color);line-height:40px;font-weight:var(--h-weight);overflow:hidden;white-space:nowrap;text-overflow:ellipsis}
.main-logo .title a{color:var(--header-color)}
.main-logo .title a:hover{color:var(--header-hover-color)}
.main-logo #h1-off{display:none;visibility:hidden}
#main-menu{z-index:10;transition:all .17s ease}
#main-menu .widget,#main-menu .widget > .widget-title{display:none}
#main-menu .widget.is-ready{display:block}
.main-nav{display:flex;height:var(--header);gap:28px}
.main-nav > li{position:relative;display:flex;flex-shrink:0}
.main-nav > li > a{display:flex;align-items:center;font-family:var(--menu-font);font-size:15px;color:var(--header-color);font-weight:600}
.main-nav > li > a > i{margin:0 4px 0 0}
.rtl .main-nav > li > a > i{margin:0 0 0 4px}
.main-nav > li > a > i[code]:before{content:attr(code)}
.main-nav .has-sub > a:after{content:"\f282";font-size:10px;font-weight:700;margin:-4px 0 0 4px}
.rtl .main-nav .has-sub > a:after{margin:-4px 4px 0 0}
.main-nav > li:hover > a{color:var(--header-hover-color)}
.main-nav .sub-menu,.main-nav .ul{position:absolute;left:0;top:calc(var(--header) - 8px);width:180px;background:var(--submenu-bg);z-index:99999;padding:8px 0;box-shadow:var(--shadow),0 10px 15px -3px $(rgba)0d;border-radius:var(--radius);backface-visibility:hidden;visibility:hidden;opacity:0;transform:translate3d(0,8px,0)}
.rtl .main-nav .sub-menu,.rtl .main-nav .ul{left:auto;right:0}
.main-nav .sub-menu.sm-1{left:-14px}
.rtl .main-nav .sub-menu.sm-1{left:unset;right:-14px}
.main-nav .sub-menu.sm-2{top:-8px;left:100%;transform:translate3d(-8px,0,0)}
.rtl .main-nav .sub-menu.sm-2{left:unset;right:100%;transform:translate3d(8px,0,0)}
.main-nav .sub-menu li{position:relative;display:block}
.main-nav .sub-menu li a{display:flex;justify-content:space-between;font-size:14px;color:var(--submenu-color);padding:8px 16px}
.main-nav .sub-menu li:hover > a{color:var(--submenu-hover-color)}
.main-nav .sub-menu > .has-sub > a:after{content:"\f285";margin:0}
.rtl .main-nav .sub-menu > .has-sub > a:after{content:"\f284"}
.main-nav .sub-menu,.main-nav .ul{transition:all .17s ease}
.main-nav li:hover > .sub-menu,.rtl .main-nav li:hover > .sub-menu{backface-visibility:inherit;visibility:visible;opacity:1;transform:translate3d(0,0,0)}
.mobile-menu-toggle{display:none;align-items:center;height:34px;font-size:26px;color:var(--header-color);padding:0 18px}
.mobile-menu-toggle:after{content:"\f479";transform:scaleX(1.2)}
.mobile-menu-toggle:hover{color:var(--header-hover-color)}
.toggle-wrap{display:flex;align-items:center;gap:2px;background:var(--header-bg);z-index:20}
.toggle-wrap .search-toggle{display:flex;align-items:center;justify-content:flex-end;width:34px;height:34px;font-size:18px;color:var(--header-color)}
.toggle-wrap .search-toggle:before{content:"\f52a"}
.toggle-wrap .search-toggle:hover{color:var(--header-hover-color)}
.main-search{display:flex;flex-direction:column;position:fixed;top:25px;left:50%;width:480px;max-width:calc(100% - (20px * 2));max-height:calc(100% - (25px * 2));background:var(--modal-bg);overflow:hidden;z-index:1010;border-radius:var(--radius);box-shadow:var(--shadow),0 10px 15px -3px $(rgba)0d;visibility:hidden;opacity:0;transform:translate3d(-50%,50%,0);transition:all .17s ease}
.main-search .search-form{display:flex;width:100%;height:60px;flex-shrink:0}
.main-search .search-input{flex:1;width:100%;font-size:16px;color:var(--title-color);font-weight:400;padding:0 20px}
.main-search .search-input::placeholder{color:var(--title-color);opacity:.65}
.main-search .search{display:flex;align-items:center;font-size:16px;color:var(--title-color);padding:0 20px;opacity:.65}
.main-search .search:before{content:"\f52a"}
.main-search .search:hover{opacity:1}
.search-content{display:none;flex-direction:column;justify-content:space-between;gap:20px;height:calc(100% - 60px);overflow:hidden;padding:20px;border-top:1px solid var(--border-color)}
.search-content.visible{display:flex}
.search-results{flex:1;overflow:hidden}
.search-results.scroll{overflow-y:auto;-webkit-overflow-scrolling:touch}
.search-items{display:grid;grid-template-columns:1fr;gap:20px}
@keyframes fadeInUp{0%{opacity:0;transform:translate3d(0,5px,0)}100%{opacity:1;transform:translate3d(0,0,0)}}
.search-items .post{display:flex;gap:16px;animation:fadeInUp .5s ease}
.search-items .entry-thumbnail{width:110px;height:74px;border-radius:var(--radius)}
.search-items .entry-header{flex:1;align-self:center}
.search-items .entry-title{display:-webkit-box;font-size:16px;overflow:hidden;-webkit-line-clamp:2;-webkit-box-orient:vertical}
.main-search .view-all{display:flex;align-items:center;justify-content:center;gap:4px;flex-shrink:0;height:36px;background:var(--button-bg);font-size:14px;color:var(--button-color);padding:0 25px}
.main-search .view-all:after{content:"\f138";line-height:1}
.rtl .main-search .view-all:after{content:"\f12f"}
.main-search .view-all:hover{opacity:.9}
.search-content .loader{height:74px}
.search-content .error-msg{justify-content:center;height:74px;padding:0}
.search-on .overlay-bg{cursor:url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='23' height='23' fill='%23ffffff' viewBox='0 0 16 16'%3E%3Cpath d='M2.146 2.854a.5.5 0 1 1 .708-.708L8 7.293l5.146-5.147a.5.5 0 0 1 .708.708L8.707 8l5.147 5.146a.5.5 0 0 1-.708.708L8 8.707l-5.146 5.147a.5.5 0 0 1-.708-.708L7.293 8 2.146 2.854Z'/%3E%3C/svg%3E"),auto;visibility:visible;opacity:1}
.search-on .main-search{backface-visibility:inherit;visibility:visible;opacity:1;transform:translate3d(-50%,0,0)}
.slide-menu{display:none;flex-direction:column;justify-content:flex-start;position:fixed;width:300px;height:100%;top:0;left:0;bottom:0;background:var(--header-bg);overflow:hidden;z-index:1010;left:0;-webkit-transform:translate3d(-100%,0,0);transform:translate3d(-100%,0,0);visibility:hidden;box-shadow:0 0 15px $(rgba)1a;transition:all .25s ease}
.rtl .slide-menu{left:unset;right:0;-webkit-transform:translate3d(100%,0,0);transform:translate3d(100%,0,0)}
.menu-on .slide-menu,.rtl .menu-on .slide-menu{-webkit-transform:translate3d(0,0,0);transform:translate3d(0,0,0);visibility:visible}
.slide-menu-header{display:flex;align-items:center;justify-content:space-between;height:var(--header);background:var(--header-bg);overflow:hidden;box-shadow:var(--shadow)}
.mobile-logo{display:flex;flex:1;width:100%;overflow:hidden;padding:0 0 0 20px}
.rtl .mobile-logo{padding:0 20px 0 0}
.mobile-logo .homepage{max-width:100%;font-size:25px;color:var(--header-color);line-height:40px;font-weight:700;overflow:hidden;white-space:nowrap;text-overflow:ellipsis}
.mobile-logo .homepage:hover{color:var(--header-hover-color)}
.mobile-logo .logo-img img{display:block;width:auto;max-width:100%;height:auto;max-height:40px}
.hide-mobile-menu{display:flex;align-items:center;height:100%;color:var(--header-color);font-size:20px;z-index:20;padding:0 20px}
.hide-mobile-menu:before{content:"\f659"}
.hide-mobile-menu:hover{color:var(--header-hover-color)}
.slide-menu-flex{display:flex;height:calc(100% - var(--header) - $(border.top));flex-direction:column;justify-content:space-between;overflow:hidden;overflow-y:auto;-webkit-overflow-scrolling:touch}
.mobile-menu{padding:20px}
.mobile-menu ul li a{display:block;font-family:var(--menu-font);font-size:14px;color:var(--header-color);font-weight:400;padding:10px 0}
.mobile-menu > ul > li > a{font-weight:700;text-transform:uppercase}
.mobile-menu .sub-menu{display:none;overflow:hidden;padding:0 0 0 15px}
.rtl .mobile-menu .sub-menu{padding:0 15px 0 0}
.mobile-menu .has-sub li a{font-size:14px;opacity:.75}
.mobile-menu .has-sub > a{display:flex;justify-content:space-between}
.mobile-menu .has-sub > a:after{content:"\f282"}
.mobile-menu .has-sub.expanded > a:after{content:"\f286"}
.mobile-menu ul li a:hover{color:var(--header-hover-color)}
.mm-footer{gap:12px;padding:20px}
.mm-footer ul{display:flex;flex-wrap:wrap;gap:15px}
.mm-footer .link-list{gap:5px 15px}
.mm-footer a{display:block;font-size:14px;color:var(--header-color)}
.mm-footer .social a{font-size:15px}
.mm-footer .social a:before{text-shadow:2px 2px 0 var(--gray-bg)}
.mm-footer .social a:hover{opacity:.9}
.mm-footer .link-list a:hover{color:var(--header-hover-color)}
.featured .widget{display:none;margin:var(--gap) 0 0;--height:300px}
.featured .widget.visible,.featured .widget.PopularPosts{display:block}
.featured .widget-content{min-height:var(--height)}
.featured .PopularPosts .widget-content{min-height:unset}
.featured .loader{height:var(--height)}
.featured .error-msg{justify-content:center;height:var(--height);padding:0}
.featured-items{display:grid;grid-template-columns:52% 1fr;align-items:start;gap:25px;width:100%}
.featured-items .post{height:var(--height)}
.featured-items .cs .entry-thumbnail{width:100%;height:100%}
.featured-items .cs.entry-header{padding:20px}
.featured-items .cs .entry-title{font-size:26px}
.featured-grid{display:grid;grid-template-columns:1fr 1fr;gap:25px}
.featured-grid .post{display:flex;flex-direction:column;background:var(--widget-bg);overflow:hidden;z-index:10;box-shadow:var(--shadow);border-radius:var(--radius)}
.featured-grid .entry-thumbnail{width:100%;height:168px;border-radius:var(--radius) var(--radius) 0 0}
.featured-grid .entry-header{padding:20px;gap:6px}
.featured-grid .entry-title{font-size:16px}
.title-wrap{position:relative;display:flex;align-items:center;justify-content:space-between;margin:0 0 20px}
.title-wrap .title{display:flex;align-items:center;position:relative;font-size:18px;color:var(--title-color);line-height:1}
.title-wrap .title-link{display:flex;align-items:center;flex-shrink:0;gap:2px;font-size:13px;color:var(--accent-color);font-weight:500}
.title-wrap .title-link:after{content:"\f138";font-size:12px}
.rtl .title-wrap .title-link:after{content:"\f12f"}
.title-wrap .title-link:hover{opacity:.9}
.list-items{display:grid;grid-template-columns:1fr;gap:25px}
.list-items .post{display:flex;gap:20px}
.list-items .entry-thumbnail{width:calc(50% - (25px / 2));height:180px}
.list-items .entry-header{flex:1;align-self:center;gap:6px}
.list-items .entry-title{font-size:20px}
.list-items .entry-meta{margin:2px 0 0}
.grid-items{display:grid;grid-template-columns:1fr 1fr;gap:25px}
.grid-items .post{display:flex;flex-direction:column;gap:14px}
.grid-items .entry-thumbnail{width:100%;height:180px}
.grid-items .entry-header{gap:6px}
.grid-items .entry-title{font-size:20px}
.grid-items .entry-meta{margin:2px 0 0}
.index-blog{background:var(--widget-bg);padding:20px;box-shadow:var(--shadow);border-radius:var(--radius)}
.queryMessage .query-info{display:flex;align-items:center;font-family:var(--title-font);font-size:18px;color:var(--title-color);font-weight:var(--h-weight);line-height:1;margin:0 0 20px}
.no-posts .queryMessage .query-info{margin:0}
.queryEmpty{font-size:14px;color:var(--meta-color);text-align:center;margin:50px 0}
.index-post-wrap .post.ad-type{display:block;border:0}
@keyframes pbtFadeInUp{0%{opacity:0;transform:translate3d(0,10px,0)}100%{opacity:1;transform:translate3d(0,0,0)}}
.index-post-wrap .post.fadeInUp{animation:pbtFadeInUp .5s ease}
.item-post-inner{background:var(--widget-bg);padding:20px;box-shadow:var(--shadow);border-radius:var(--radius)}
.item-post .post-header{gap:14px}
#breadcrumb{display:flex;align-items:center;gap:2px;font-size:14px;color:var(--accent-color);line-height:1}
#breadcrumb a{color:var(--accent-color)}
#breadcrumb a:hover{opacity:.9}
#breadcrumb .sep:after{content:"\f285";font-size:10px;font-style:normal;font-weight:700}
.rtl #breadcrumb .sep:after{content:"\f284"}
.item-post h1.entry-title{font-size:$(itempost.title.size)}
.post-header .entry-meta{flex-wrap:nowrap;justify-content:space-between;gap:0;font-size:14px}
.entry-meta .align-left,.entry-meta .align-right{display:flex;align-items:center}
.entry-meta .entry-avatar{flex-shrink:0;width:34px;height:34px;overflow:hidden;padding:1px;margin:0 5px 0 0;border:1px solid var(--accent-color);border-radius:50%}
.rtl .entry-meta .entry-avatar{margin:0 0 0 5px}
.entry-meta .avatar{z-index:2;border-radius:50%}
.entry-meta .al-items{display:flex;flex-wrap:wrap;gap:4px}
.entry-meta .align-left .entry-author,.entry-meta .align-left .entry-time{display:flex;gap:4px}
.post-header .entry-meta .author-name{font-weight:700}
.share-toggle{display:flex;align-items:center;justify-content:flex-end;width:34px;height:34px;font-size:20px;color:var(--title-color)}
.share-toggle:before{content:"\f1c6"}
.share-toggle:hover{color:var(--title-hover-color)}
.entry-content-wrap{padding:25px 0 0}
#post-body{position:relative;font-family:var(--text-font);font-size:$(itempost.content.size);color:var(--text-color);line-height:1.6em}
.post-body p{margin-bottom:25px}
.post-body h1,.post-body h2,.post-body h3,.post-body h4,.post-body h5,.post-body h6{font-size:17px;color:var(--title-color);line-height:1.3em;margin:0 0 20px}
.post-body h1{font-size:26px}
.post-body h2{font-size:23px}
.post-body h3{font-size:20px}
.post-body img{height:auto!important}
blockquote{position:relative;background:var(--gray-bg);color:var(--title-color);font-style:normal;padding:25px;margin:0;border-radius:var(--radius)}
blockquote:before{position:absolute;top:10px;left:10px;content:"\f6b0";font-size:50px;color:var(--title-color);font-style:normal;line-height:1;opacity:.05}
.rtl blockquote:before{left:unset;right:10px}
.post-body ul{padding:0 0 0 20px;margin:10px 0}
.rtl .post-body ul{padding:0 20px 0 0}
.post-body li{margin:8px 0;padding:0}
.post-body ul li,.post-body ol ul li{list-style:none}
.post-body ul li:before,.post-body ul li ul li ul li:before{content:"\f287";font-size:.35em;line-height:1;vertical-align:middle;margin:0 5px 0 0}
.post-body ul li ul li:before{content:"\f28a";font-weight:700}
.rtl .post-body ul li:before{margin:0 0 0 5px}
.post-body ol{counter-reset:pbt;padding:0 0 0 20px;margin:10px 0}
.rtl .post-body ol{padding:0 20px 0 0}
.post-body ol > li{counter-increment:pbt;list-style:none}
.post-body ol > li:before{content:counters(pbt,".")".";font-family:inherit;margin:0 5px 0 0}
.rtl .post-body ol > li:before{margin:0 0 0 5px}
.post-body u{text-decoration:underline}
.post-body strike{text-decoration:line-through}
.post-body sup{vertical-align:super}
.post-body a{color:var(--accent-color)}
.post-body a:hover{text-decoration:underline}
.post-body .button{display:inline-block;height:36px;background:var(--button-bg);font-family:var(--body-font);font-size:14px;color:var(--button-color);font-weight:400;line-height:36px;text-align:center;text-decoration:none;cursor:pointer;padding:0 20px;margin:0 6px 8px 0}
.rtl .post-body .button{margin:0 0 8px 6px}
.post-body .button.x2{height:48px;font-size:16px;line-height:48px}
.post-body .button.is-c,.rtl.post-body .button.is-c{margin:0 3px 8px}
.post-body .button.x2 span{display:inline-block;background:rgba(255,255,255,.08);font-size:14px;line-height:16px;padding:4px 6px;margin:0 0 0 20px;border-radius:var(--radius)}
.rtl .post-body .button.x2 span{margin:0 20px 0 0}
.post-body .button:before{font-size:16px;font-style:normal;vertical-align:middle;margin:-2px 6px 0 0}
.rtl .post-body .button:before{margin:-2px 0 0 6px}
.post-body .btn.x2:before{font-size:18px;margin:-2px 10px 0 0}
.rtl .post-body .btn.x2:before{margin:-2px 0 0 10px}
.post-body .btn.preview:before{content:"\f33e"}
.post-body .btn.download:before{content:"\f294"}
.post-body .btn.link:before{content:"\f470"}
.post-body .btn.cart:before{content:"\f23d"}
.post-body .btn.info:before{content:"\f430"}
.post-body .btn.share:before{content:"\f52d"}
.post-body .btn.contact:before{content:"\f32c"}
.post-body .btn.phone:before{content:"\f5b4"}
.post-body .btn.gift:before{content:"\f3eb"}
.post-body .btn.whatsapp:before{content:"\f618"}
.post-body .btn.paypal:before{content:"\f662"}
.post-body .btn.telegram:before{content:"\f5b3"}
.post-body a.color{color:#fff}
.post-body a.button{color:var(--button-color);text-decoration:none}
.post-body a.button:hover{opacity:.9}
.alert-message{display:block;position:relative;background:#22c55e15;color:#22c55e;overflow:hidden;padding:20px;border-radius:var(--radius)}
.alert-message.alert-info{background:#3b82f615;color:#3b82f6}
.alert-message.alert-warning{background:#eab30815;color:#eab308}
.alert-message.alert-error{background:#ef444415;color:#ef4444}
.alert-message:before{content:'\f26a';font-size:16px;line-height:1;vertical-align:middle;margin:-1px 6px 0 0}
.rtl .alert-message:before{margin:-1px 0 0 6px}
.alert-message.alert-info:before{content:'\f430'}
.alert-message.alert-warning:before{content:'\f33a'}
.alert-message.alert-error:before{content:'\f622'}
.alert-message a:not(.btn){color:currentColor;text-decoration:underline}
.alert-message a:not(.btn):hover{opacity:.9}
.post-body table{width:100%;overflow-x:auto;text-align:left;margin:0;border-collapse:collapse;border:1px solid var(--border-color)}
.rtl .post-body table{text-align:right}
.post-body table td,.post-body table th{padding:6px 12px;border:1px solid var(--border-color)}
.post-body table thead th{color:var(--title-color);vertical-align:bottom}
table.tr-caption-container,table.tr-caption-container td,table.tr-caption-container th{line-height:1;padding:0;border:0}
table.tr-caption-container td.tr-caption{font-size:12px;color:var(--meta-color);font-style:italic;padding:6px 0 0}
.post-body .contact-form-widget{display:table;width:100%;font-family:var(--body-font)}
.post-body .contact-form-name.cf-s{width:calc(50% - 5px)}
.rtl .post-body .contact-form-name{float:right}
.post-body .contact-form-email.cf-s{float:right;width:calc(50% - 5px)}
.rtl .post-body .contact-form-email{float:left}
.post-body pre,pre.code-box{display:block;background:var(--gray-bg);font-family:monospace;font-size:13px;color:var(--title-color);white-space:pre-wrap;line-height:1.4em;padding:20px;border:1px solid var(--border-color);border-radius:var(--radius)}
.post-body iframe[allowfullscreen]{height:auto;aspect-ratio:16/9}
.post-body .google-auto-placed{margin:25px 0}
.entry-labels{display:flex;flex-wrap:wrap;gap:5px 6px;margin:25px 0 0}
.entry-labels > *{display:flex;align-items:center;height:22px;font-size:12px;color:var(--title-color);padding:0 8px;box-shadow:inset 0 0 0 1px var(--border-color)}
.entry-labels span{background:var(--title-color);color:var(--widget-bg);box-shadow:none}
.entry-labels a:hover{background:var(--button-bg);color:var(--button-color)}
.post-share{margin:25px 0 0}
ul.share-a{display:flex;flex-wrap:wrap;align-items:start;gap:6px}
.share-a .btn{display:flex;align-items:center;justify-content:center;width:38px;height:36px;background:currentColor;font-size:18px;font-weight:400}
.share-a .has-span .btn{display:flex;gap:10px;width:auto;padding:0 16px}
.share-a .btn:before{color:#fff}
.share-a .btn span{font-size:14px;color:#fff}
.share-a .sl-btn{position:relative;background:var(--widget-bg);font-size:18px;color:var(--title-color);line-height:1;overflow:visible;margin:0 5px 0 0;border:1px solid var(--border-color);border-radius:var(--radius)}
.share-a .sl-btn:before,.share-a .sl-btn:after{content:"";position:absolute;height:0;width:0;pointer-events:none;top:calc(50% - 6px);right:-12px;border:6px solid transparent;border-left-color:var(--border-color)}
.share-a .sl-btn:after{top:calc(50% - 5px);right:-10px;border:5px solid transparent;border-left-color:var(--widget-bg)}
.sl-btn .sl-ico:before{content:"\f52d";font-style:normal;padding:1px 0 0}
.rtl .share-a .sl-btn{margin:0 0 0 5px;transform:scaleX(-1)}
.share-a .show-more .btn{background:var(--gray-bg);font-size:22px}
.share-a .show-more .btn:before{content:"\f64d";color:var(--meta-color)}
.share-a li .btn:not(.sl-btn):hover{opacity:.9}
.share-modal{display:flex;flex-direction:column;position:fixed;top:50%;left:50%;width:440px;max-width:calc(100% - 40px);background:var(--modal-bg);overflow:hidden;z-index:1010;padding:20px;box-shadow:var(--shadow),0 10px 15px -3px $(rgba)0d;border-radius:var(--radius);visibility:hidden;opacity:0;transform:translate3d(-50%,0,0);transition:all .17s ease}
.modal-header{display:flex;align-items:center;justify-content:space-between;padding:0 0 15px;margin:0 0 20px;border-bottom:1px solid var(--border-color)}
.share-modal .title{font-family:var(--title-font);font-size:15px;color:var(--title-color);font-weight:var(--h-weight);text-transform:capitalize}
.hide-modal{display:flex;font-size:20px;color:var(--title-color)}
.hide-modal:before{content:"\f659"}
.hide-modal:hover{color:var(--title-hover-color)}
ul.share-b{display:grid;grid-template-columns:repeat(4,1fr);gap:16px;margin:0 0 20px}
.share-b a{display:flex;align-items:center;justify-content:center;height:36px;background:currentColor;font-size:18px}
.share-b a:before{color:#fff}
.share-b a:hover{opacity:.9}
.copy-link{display:flex;gap:10px;position:relative;width:100%;height:36px;margin:15px 0 0}
.copy-link:before{content:"\f470";position:absolute;top:50%;left:20px;font-size:20px;color:var(--title-color);transform:translate(-50%,-50%)}
.rtl .copy-link:before{left:unset;right:20px;transform:translate(50%,-50%)}
@keyframes pbtOn{0%{opacity:0}100%{opacity:1}}
@keyframes pbtOff{0%{opacity:0}100%{opacity:1}}
.copy-link.copied:before{content:"\f26f";color:#3fbb50;animation:pbtOn .5s ease}
.copy-link.copied-off:before{animation:pbtOff .5s ease}
.copy-link input{flex:1;width:100%;font-size:14px;color:var(--text-color);padding:0 15px 0 40px;border:1px solid var(--border-color);border-radius:var(--radius)}
.rtl .copy-link input{padding:0 40px 0 15px}
.copy-link button{display:flex;align-items:center;justify-content:center;max-width:fit-content;background:var(--button-bg);font-size:14px;color:var(--button-color);padding:0 25px}
.copy-link button:hover{opacity:.9}
.share-on .overlay-bg{visibility:visible;opacity:1}
.share-on .share-modal{visibility:visible;opacity:1;transform:translate3d(-50%,-50%,0)}
.p-widget{margin:var(--gap) 0 0}
.about-author{display:flex;gap:16px;background:var(--widget-bg);padding:20px;box-shadow:var(--shadow);border-radius:var(--radius)}
.about-author .author-avatar{width:60px;height:60px;border-radius:50%}
.author-description{flex:1;gap:10px}
.about-author .author-title{font-size:18px;color:var(--title-color)}
.about-author .author-title a{color:var(--title-color)}
.about-author .author-title a:hover{color:var(--title-hover-color)}
.author-description .author-text{display:block;font-size:14px}
.author-description .author-text br,.author-description .author-text a{display:none}
.author-links{display:flex;flex-wrap:wrap;gap:14px}
.author-links a{display:block;font-size:14px;color:var(--text-color)}
.author-links a:before{text-shadow:2px 2px 0 var(--gray-bg)}
.author-links a:hover{opacity:.9}
#related-posts{display:none}
.related-wrap{background:var(--widget-bg);padding:20px;box-shadow:var(--shadow);border-radius:var(--radius)}
.related-wrap .loader{height:180px}
.related-items{display:grid;grid-template-columns:repeat(3,1fr);gap:25px}
.related-items .post{display:flex;flex-direction:column;gap:10px}
.related-items .entry-thumbnail{width:100%;height:128px}
.related-items .entry-title{font-size:15px}
.blog-post-comments{display:none;flex-direction:column;background:var(--widget-bg);padding:20px;box-shadow:var(--shadow);border-radius:var(--radius)}
.blog-post-comments.visible{display:flex}
.comments-title.has-message{margin:0 0 10px}
.no-comment-form .comments-title.has-message{margin:0 0 20px}
.comment-thread ol{padding:0;margin:0}
.comment-thread .comment{position:relative;list-style:none;padding:20px;margin:20px 0 0;border:1px solid var(--border-color);border-radius:var(--radius)}
.comment-thread .comment .comment{background:var(--gray-bg);padding:20px;border:0}
.toplevel-thread ol > li:first-child{margin:0}
.toplevel-thread ol > li:first-child > .comment-block{padding-top:0;margin:0;border:0}
.comment-thread ol ol .comment:before{content:"\f132";position:absolute;left:-30px;top:-5px;font-size:16px;color:var(--border-color)}
.rtl .comment-thread ol ol .comment:before{content:"\f131";left:unset;right:-30px}
.comments .comment-replybox-single iframe{padding:0 0 0 48px;margin:10px 0 -5px}
.rtl .comments .comment-replybox-single iframe{padding:0 48px 0 0}
.comment-thread .avatar-image-container{position:absolute;top:20px;left:20px;width:35px;height:35px;overflow:hidden;border-radius:50%}
.rtl .comment-thread .avatar-image-container{left:auto;right:20px}
.comment-thread .comment .comment .avatar-image-container{left:20px}
.rtl .comment-thread .comment .comment .avatar-image-container{left:unset;right:20px}
.avatar-image-container img{display:block;width:100%;height:100%}
.comments .comment-block{display:flex;flex-direction:column;gap:10px}
.comments .comment-header{padding:0 0 0 48px}
.rtl .comments .comment-header{padding:0 48px 0 0}
.comments .comment-header .user{display:inline-block;font-family:var(--title-font);font-size:16px;color:var(--title-color);font-weight:var(--h-weight);font-style:normal}
.comments .comment-header .user a{color:var(--title-color)}
.comments .comment-header .user a:hover{color:var(--title-hover-color)}
.comments .comment-header .icon.user{display:none}
.comments .comment-header .icon.blog-author{display:inline-block;background:var(--gradient);-webkit-background-clip:text;background-clip:text;font-size:14px;color:var(--accent-color);-webkit-text-fill-color:transparent;vertical-align:top;margin:-5px 0 0 4px}
.rtl .comments .comment-header .icon.blog-author{margin:-5px 4px 0 0}
.comments .comment-header .icon.blog-author:before{content:"\f4b5"}
.comments .comment-header .datetime{display:block;font-size:12px;margin:1px 0 0}
.comment-header .datetime a{color:var(--meta-color)}
.comments .comment-content{display:block;font-family:var(--text-font);font-size:14px;color:var(--text-color);line-height:1.6em}
.comments .comment-content > a:hover{text-decoration:underline}
.comments .comment-video{position:relative;width:100%;height:auto;aspect-ratio:16/9;overflow:hidden;line-height:1;cursor:pointer}
.comments .comment-video img{display:block;width:100%;height:100%;object-fit:cover;z-index:1}
.comments .comment-video:before{content:"";position:absolute;top:0;left:0;width:100%;height:100%;background:$(rgba)1a;z-index:2}
.comments .comment-video:after{transform:translate(50%, 50%) scale(1.2);transition:all .17s ease}
.comments .comment-video:hover:after{transform:translate(50%, 50%) scale(1.5)}
.comments .comment-actions{display:flex;gap:14px}
.comments .comment-actions a{display:inline-block;font-size:14px;color:var(--accent-color);font-weight:400;font-style:normal}
.comments .comment-actions a:hover{color:var(--accent-color);text-decoration:underline}
.item-control{display:none}
.loadmore.loaded a{display:inline-block;border-bottom:1px solid var(--border-color);text-decoration:none;margin-top:15px}
.comments .continue{display:none}
.comments .comment-replies{padding:0 0 0 48px}
.rtl .comments .comment-replies{padding:0 48px 0 0}
.thread-expanded .thread-count a,.loadmore.hidden,.comment-thread .comment .comment .comment-replies,.comment-thread .comment .comment .comment-replybox-single{display:none}
.comments .footer{float:left;width:100%;font-size:13px;margin:0}
.comments-message{font-size:14px;color:var(--meta-color);font-style:italic;margin:0 0 20px}
.no-comment-form .comments-message{margin:20px 0 0}
.no-comments.no-comment-form .comments-message{margin:0}
.comments-message > a{color:var(--accent-color)}
.comments-message > a:hover{color:var(--title-color)}
.comments-message > em{color:#ff3f34;font-style:normal;margin:0 3px}
#comments[data-embed="false"] p.comments-message > i{color:var(--accent-color);font-style:normal}
.comment-form > p{display:none}
.show-cf,.comments #top-continue a{display:flex;align-items:center;justify-content:center;width:100%;height:38px;font-size:$(itempost.content.size);color:var(--title-color);font-weight:var(--h-weight);padding:0 20px;margin:20px 0 0;border:1px solid var(--border-color)}
.no-comments .show-cf{margin:0}
.show-cf:hover,.comments #top-continue a:hover{color:var(--title-hover-color)}
.cf-on .show-cf{display:none}
.comments .comment-replybox-thread,.no-comments .comment-form{display:none}
.cf-on .comments .comment-replybox-thread,.cf-on .no-comments .comment-form{display:block}
#comment-editor{min-height:67px}
#top-ce #comment-editor{margin:20px 0 0}
.post-nav{display:flex;flex-wrap:wrap;justify-content:space-between;font-size:14px}
.post-nav > *{display:flex;align-items:center;gap:3px;color:var(--meta-color)}
.post-nav a:hover{color:var(--accent-color)}
.post-nav span{color:var(--meta-color);cursor:no-drop;opacity:.65}
.post-nav .post-nav-link:before,.post-nav .post-nav-link:after{font-size:10px;font-weight:700}
.post-nav-newer-link:before,.rtl .post-nav-older-link:after{content:"\f284"}
.post-nav-older-link:after,.rtl .post-nav-newer-link:before{content:"\f285"}
.blog-pager{display:flex;justify-content:center;margin:25px 0 5px}
.blog-pager .btn{display:none;align-items:center;justify-content:center;gap:4px;height:34px;background:var(--button-bg);font-size:14px;color:var(--button-color);padding:0 25px}
.blog-pager a:after{content:"\f282";margin:-2px 0 0}
.blog-pager a:hover{opacity:.9}
.blog-pager .no-more{background:var(--gray-bg);color:var(--meta-color);cursor:not-allowed}
.blog-pager .loading{display:none}
.blog-pager .loader{height:34px}
.blog-pager .visible{display:flex}
.sidebar{position:relative;display:grid;grid-template-columns:100%;gap:var(--gap)}
.sidebar .widget{display:flex;flex-direction:column;background:var(--widget-bg);padding:20px;box-shadow:var(--shadow);border-radius:var(--radius)}
.sidebar .widget.is-ad{display:block;background:transparent;padding:0;box-shadow:none;border-radius:0}
.sidebar .is-ad .title-wrap{display:none}
.sidebar ul.social{display:grid;grid-template-columns:1fr 1fr;gap:6px}
.sidebar .social a{display:flex;align-items:center;gap:10px;width:100%;height:36px;background:currentColor;font-size:18px;font-weight:400;padding:0 16px}
.sidebar .social .instagram a{background:var(--instagram)}
.sidebar .social a:before{color:#fff}
.sidebar .social span{font-size:14px;color:#fff}
.sidebar .social a:hover{opacity:.9}
.pbt-s .loader{height:176px}
.popular-items{display:grid;grid-template-columns:1fr;gap:25px}
.popular-items .cs{height:176px}
.popular-items .cs .entry-title{font-size:18px}
.popular-list{display:grid;grid-template-columns:1fr;gap:25px}
.popular-list .post{display:flex;gap:14px}
.popular-list .entry-thumbnail{width:98px;height:68px}
.popular-list .entry-header{flex:1;align-self:center}
.popular-list .entry-title{font-size:14px}
.featured-post .cs{height:176px}
.featured-post .entry-title{font-size:18px}
.list-style li{font-size:14px}
.list-style li a,.text-list li{display:block;color:var(--title-color);padding:8px 0}
.list-style li a.has-count{display:flex;justify-content:space-between}
.list-style li:first-child a,.text-list li:first-child{padding:0 0 8px}
.list-style li:last-child a,.text-list li:last-child{padding:8px 0 0}
.list-style li a:hover{color:var(--title-hover-color)}
.list-style .count-style{display:inline-block;color:var(--accent-color)}
.cloud-label ul{display:flex;flex-wrap:wrap;gap:6px}
.cloud-label li a{display:flex;height:30px;color:var(--title-color);font-size:14px;font-weight:400;align-items:center;padding:0 13px;box-shadow:inset 0 0 0 1px var(--border-color)}
.cloud-label li a:hover{background:var(--button-bg);color:var(--button-color);box-shadow:none}
.cloud-label .label-count{display:inline-block;margin:0 0 0 4px}
.rtl .cloud-label .label-count{margin:0 4px 0 0}
.BlogSearch .search-input{display:flex;align-items:center;justify-content:space-between;flex:1;width:100%;height:36px;font-size:14px;color:var(--title-color);cursor:text;padding:0 14px;border:1px solid var(--border-color);border-radius:var(--radius)}
.BlogSearch .search-input:before{content:attr(placeholder);font-family:inherit;opacity:.65}
.BlogSearch .search-input:after{content:"\f52a";opacity:.65}
.MailChimp .widget-content{position:relative}
.MailChimp .widget-content:before{content:"\f32f";position:absolute;top:0;right:0;font-size:38px;color:var(--border-color);line-height:1;z-index:1;transform:translate(8px,-8px) rotate(35deg)}
.rtl .MailChimp .widget-content:before{left:0;right:unset;transform:translate(-8px,-8px) rotate(-35deg)}
.MailChimp .mailchimp-title{font-size:18px;color:var(--title-color);margin:0 0 15px}
.MailChimp .mailchimp-text{font-size:14px;margin:0 0 15px}
.MailChimp form{display:flex;flex-direction:column;gap:10px}
.MailChimp .mailchimp-email-address{width:100%;height:36px;font-size:14px;color:var(--title-color);padding:0 14px;border:1px solid var(--border-color);border-radius:var(--radius)}
.MailChimp .mailchimp-email-address::placeholder{color:var(--title-color);opacity:.65}
.MailChimp .mailchimp-email-address:focus{border-color:var(--accent-color);box-shadow:0 0 0 2px var(--accent-color-10)}
.MailChimp .mailchimp-submit{width:100%;height:36px;background:var(--button-bg);font-size:14px;color:var(--button-color);font-weight:400;cursor:pointer;padding:0 20px}
.MailChimp .mailchimp-submit:hover{opacity:.9}
.Profile ul li{float:left;width:100%;padding:20px 0 0;margin:20px 0 0;border-top:1px solid var(--border-color)}
.Profile ul li:first-child{padding:0;margin:0;border:0}
.Profile .individual,.Profile .team-member{display:flex;align-items:center}
.Profile .profile-img{width:45px;height:45px;background:var(--gray-bg);overflow:hidden;margin:0 14px 0 0;border-radius:50%}
.rtl .Profile .profile-img{margin:0 0 0 14px}
.Profile .profile-info{flex:1}
.Profile .profile-name{display:block;font-family:var(--title-font);font-size:16px;color:var(--title-color);font-weight:var(--h-weight)}
.Profile .profile-name:hover{color:var(--title-hover-color)}
.Profile .profile-link{display:block;font-size:12px;color:var(--meta-color);line-height:1.3em}
.Profile .profile-link:hover{color:var(--accent-color)}
.Text .widget-content{font-size:14px}
.Image img{width:auto;height:auto}
.Image .image-caption{font-size:14px;margin:8px 0 0}
.contact-form-widget .cf-s{float:left;width:100%;height:36px;font-size:14px;color:var(--title-color);padding:0 14px;margin:0 0 10px;border:1px solid var(--border-color);border-radius:var(--radius)}
.contact-form-email-message.cf-s{float:left;width:100%;height:auto;resize:vertical;padding:10px 14px}
.contact-form-widget .cf-s::placeholder{color:var(--title-color);opacity:.65}
.contact-form-widget .cf-s:focus{border-color:var(--accent-color);box-shadow:0 0 0 2px var(--accent-color-10)}
.contact-form-button-submit{float:left;width:100%;height:36px;background:var(--button-bg);font-family:inherit;font-size:14px;color:var(--button-color);font-weight:400;cursor:pointer;padding:0 20px;border:0}
.contact-form-button-submit:hover{opacity:.9}
.contact-form-widget p{margin:0}
.contact-form-widget .contact-form-error-message-with-border,.contact-form-widget .contact-form-success-message-with-border{float:left;width:100%;background:transparent;font-size:13px;color:#ef4444;text-align:left;line-height:1;margin:10px 0 0;border:0}
.contact-form-widget .contact-form-success-message-with-border{color:#22c55e}
.rtl .contact-form-error-message-with-border,.rtl .contact-form-success-message-with-border{text-align:right}
.contact-form-cross{cursor:pointer;margin:0 0 0 3px}
.rtl .contact-form-cross{margin:0 3px 0 0}
.Attribution a{display:flex;align-items:center;font-size:14px;color:var(--title-color);font-weight:var(--h-weight)}
.Attribution a > svg{width:16px;height:16px;fill:var(--accent-color);margin:0 4px 0 0}
.rtl .Attribution a > svg{margin:0 0 0 4px}
.Attribution a:hover{color:var(--title-hover-color)}
.Attribution .copyright{font-size:12px;color:var(--meta-color);padding:0 20px;margin:2px 0 0}
#google_translate_element{position:relative;overflow:hidden}
.Stats .text-counter-wrapper{display:flex;align-items:center;gap:6px;font-size:18px;color:var(--title-color);font-weight:700;text-transform:uppercase}
.Stats .text-counter-wrapper:before{content:"\f17a";font-size:16px;line-height:1}
.ReportAbuse > h3{display:flex;gap:4px;font-size:14px;color:var(--accent-color);font-weight:400}
.ReportAbuse > h3:before{content:"\f33a";font-size:16px}
.ReportAbuse > h3 a:hover{text-decoration:underline}
.Header .header-widget a{font-size:18px;color:var(--title-color);font-weight:var(--h-weight)}
.Header .header-widget a:hover{color:var(--title-hover-color)}
.wikipedia-search-form{display:flex;gap:10px}
.wikipedia-search-input{flex:1;width:100%;height:36px;font-size:14px;color:var(--title-color);padding:0 14px;border:1px solid var(--border-color);border-radius:var(--radius)}
.wikipedia-search-input::placeholder{color:var(--title-color);opacity:.65}
.wikipedia-search-input:focus{border-color:var(--accent-color);box-shadow:0 0 0 2px var(--accent-color-10)}
.wikipedia-search-button{height:36px;background:var(--button-bg);font-size:14px;color:var(--button-color);font-weight:400;cursor:pointer;padding:0 20px}
.wikipedia-search-button:hover{opacity:.9}
.wikipedia-search-results-header{display:none!important}
.wikipedia-search-results{font-size:13px;color:#ef4444}
.wikipedia-search-results a{display:flex;align-items:center;gap:6px;font-size:14px;color:var(--title-color);margin:10px 0 0}
.wikipedia-search-results a:after{content:"\f1c5";font-size:12px}
.wikipedia-search-results a:hover{color:var(--title-hover-color)}
.wikipedia-search-more a{display:flex;align-items:center;justify-content:center;height:36px;color:var(--title-color);padding:0 15px;margin:10px 0 0;box-shadow:inset 0 0 0 1px var(--border-color);border-radius:var(--radius)}
.wikipedia-search-more a:hover{background:var(--button-bg);color:var(--button-color);box-shadow:none}
.site-footer{position:relative;background:var(--footer-bg);box-shadow:var(--shadow);margin:var(--gap) 0 0;--title-color:var(--footer-color);--title-hover-color:var(--footer-hover-color);--text-color:var(--footer-text-color);--gray-bg:rgba(155,155,155,.07)}
.site-footer .footer{float:left;width:100%}
#about{gap:var(--gap);padding:40px 0}
.about-section .Image{display:flex;align-items:center;justify-content:space-between;flex:1;max-width:calc(100% - ($(sidebar.width) + var(--gap)));gap:28px}
.footer-info{flex:1}
.footer-info .title{font-size:18px;color:var(--title-color);margin:0 0 10px}
.footer-logo img{display:block;max-height:40px}
.footer-info .image-caption{margin:0}
.footer-info .image-caption a{color:var(--title-color)}
.footer-info .image-caption a:hover{opacity:.9}
.about-section .LinkList{display:flex;align-items:center;justify-content:flex-end;width:$(sidebar.width)}
.about-section ul.social{display:flex;flex-wrap:wrap;gap:10px}
.about-section .social a{display:flex;align-items:center;justify-content:center;width:36px;height:36px;background:var(--gray-bg);font-size:18px}
.about-section .social a:before{color:var(--title-color)}
.about-section .social a:hover{background:currentColor}
.about-section .social a:hover:before{color:#fff}
.about-section .social .instagram a:hover{background:var(--instagram)}
.footer-bar{float:left;width:100%;background:var(--footerbar-bg);color:var(--footerbar-color);padding:20px 0}
.footer-copyright{font-size:14px;font-weight:400}
.footer-copyright a{color:var(--footerbar-color)}
.footer-copyright a:hover{color:var(--footerbar-hover-color)}
.footer-menu{position:relative;display:block;margin:0}
.footer-menu ul{display:flex;flex-wrap:wrap;gap:5px 25px}
.footer-menu a{font-size:14px;color:var(--footerbar-color);padding:0}
.footer-menu a:hover{color:var(--footerbar-hover-color)}
.is-error .main-wrap{width:100%}
.is-error .sidebar-wrap{display:none}
.errorWrap{color:var(--title-color);text-align:center;padding:60px 0}
.errorWrap h3{font-size:160px;color:var(--title-color);line-height:1;margin:0 0 35px}
.errorWrap h4{font-size:27px;color:var(--title-color);margin:0 0 25px}
.errorWrap p{color:var(--text-color);font-size:15px;margin:0 0 30px}
.errorWrap a{display:inline-block;height:36px;background:var(--button-bg);font-size:15px;color:var(--button-color);line-height:36px;padding:0 30px}
.errorWrap a:hover{opacity:.9}
.back-top{display:flex;align-items:center;justify-content:center;position:fixed;bottom:20px;right:20px;width:36px;height:36px;background:var(--button-bg);font-size:18px;color:var(--button-color);z-index:50;opacity:0;visibility:hidden;transition:all .17s ease}
.rtl .back-top{right:auto;left:20px}
.back-top:before{content:"\f286"}
.back-top.show{opacity:1;visibility:visible}
.back-top:hover{opacity:.9}
ins.adsbygoogle-noablate[data-anchor-shown="true"]{z-index:990!important}
.content-wrap > .google-auto-placed,.content-wrap .container > .google-auto-placed{display:none!important}
#hidden,.is-empty{display:none}
.CSS_LIGHTBOX{z-index:999999!important}
.CSS_LIGHTBOX_BG_MASK{background-color:rgba(0,0,0,.9)!important;opacity:1!important;backdrop-filter:blur(1px)}
.CSS_LIGHTBOX_BTN_CLOSE{display:flex;align-items:center;justify-content:center;background:transparent!important;top:0px!important;right:0px!important;width:46px!important;height:46px!important}
.CSS_LIGHTBOX_BTN_CLOSE:before{content:"\f659";font-size:22px;color:#fff}
.CSS_LIGHTBOX_BTN_CLOSE:hover:before{opacity:.85}
.rtl .CSS_LIGHTBOX_BTN_CLOSE{right:unset!important;left:0}
.CSS_LIGHTBOX_ATTRIBUTION_INDEX_CONTAINER .CSS_HCONT_CHILDREN_HOLDER > .CSS_LAYOUT_COMPONENT.CSS_HCONT_CHILD:first-child > .CSS_LAYOUT_COMPONENT{opacity:0}
.pbt-ad{display:flex;align-items:center;justify-content:center}
.pbt-ad img{height:auto}
@media (max-width: $(row.width + 60px)) {
.site-outer,.is-boxed .site-outer,.is-boxed .header-header{width:100%;max-width:100%;margin:0}
.row-x1{width:100%}
.container{padding:0 20px}
.main-wrap{width:calc(70% - var(--gap))}
.sidebar-wrap{width:30%}
}
@media (max-width: 980px) {
.main-header .container{padding:0}
.header-items{flex-wrap:nowrap;gap:20px}
.mobile-menu-toggle{display:flex}
#main-menu{display:none}
.slide-menu{display:flex}
.menu-on .overlay-bg{visibility:visible;opacity:1}
.flex-left{gap:0;overflow:hidden}
.main-logo{flex-shrink:1}
.flex-right,.rtl .flex-right{position:relative;top:unset;left:unset;right:unset}
.toggle-wrap{gap:0}
.toggle-wrap .search-toggle{width:auto;font-size:20px;padding:0 20px}
}
@media (max-width: 880px) {
.widget:not(.type-video) .yt-img\:x3:after{transform:translate(50%,50%) scale(.95)}
.yt-img\:x4:after{transform:translate(50%,50%) scale(.75)}
.content-wrap > .container,.is-left .content-wrap > .container{flex-direction:column!important;justify-content:flex-start}
.main-wrap,.sidebar-wrap{width:100%}
.sidebar-wrap{margin:var(--gap) 0 0}
.featured-items{grid-template-columns:1fr}
.featured-grid .post{height:auto}
.sidebar ul.social{grid-template-columns:repeat(4,1fr)}
.popular-items .cs{height:200px}
.popular-items .cs .entry-title{font-size:22px}
.popular-list .entry-thumbnail{width:110px;height:74px}
.popular-list .entry-title{font-size:15px}
.featured-post .cs{height:200px}
.featured-post .entry-title{font-size:22px}
#about{flex-direction:column;gap:25px}
.about-section .Image{flex-direction:column;justify-content:center;flex:unset;max-width:100%;gap:25px;text-align:center}
.footer-info .title{display:none}
.footer-logo{padding:0!important}
.about-section .LinkList{width:100%;justify-content:center}
.about-section ul.social-icons{justify-content:center}
.footer-bar{height:auto;line-height:inherit;padding:35px 0}
.footer-bar .container{display:grid;grid-template-columns:1fr;gap:15px;text-align:center}
.footer-copyright{order:1}
.footer-menu ul{justify-content:center;gap:5px 20px}
.menu-on .back-top{opacity:0!important}
}
@media (max-width: 680px) {
.type-video .yt-img\:x3:after{transform:translate(50%,50%) scale(.95)}
.featured .widget{--height:220px}
.featured-items .cs{height:220px}
.featured-items .cs .entry-title{font-size:22px}
.featured-grid .entry-thumbnail{height:130px}
.featured-grid .entry-title{font-size:15px}
.list-items .post{flex-direction:column;gap:14px}
.list-items .entry-thumbnail{width:100%;height:200px}
.list-items .entry-header{flex:auto;align-self:start}
.list-items .entry-title{font-size:22px}
.grid-items{grid-template-columns:1fr}
.grid-items .entry-thumbnail{height:200px}
.grid-items .entry-title{font-size:22px}
.item-post h1.entry-title{font-size:31px}
.post-body table{display:block}
.related-items{grid-template-columns:1fr 1fr}
.related-items .entry-thumbnail{height:130px}
.sidebar ul.social{grid-template-columns:1fr 1fr}
.errorWrap{padding:20px 0 30px}
.errorWrap h3{font-size:130px}
.errorWrap h4{line-height:initial}
}
@media (max-width: 480px) {
:root{--gap:25px}
.container{padding:0 16px}
.main-search{top:20px;max-width:calc(100% - (16px * 2));max-height:calc(100% - (20px * 2))}
.featured-items,.featured-grid{gap:20px}
.featured-grid .entry-thumbnail{height:120px}
.featured-grid .entry-header{padding:16px}
.list-items .entry-title{font-size:20px}
.grid-items .entry-title{font-size:20px}
.item-post h1.entry-title{font-size:29px}
.share-a .twitter .btn{width:38px}
.share-a .twitter .btn span{display:none}
.share-a .whatsapp{display:none}
.related-items{gap:25px 20px}
.related-items .entry-thumbnail{height:110px}
.popular-items .cs .entry-title{font-size:20px}
.featured-post .entry-title{font-size:20px}
.share-modal{max-width:calc(100% - (16px * 2))}
.back-top{right:16px}
.rtl .back-top{left:16px;right:auto}
}
@media (max-width: 380px) {
.search-items .post{gap:14px}
.search-items .entry-thumbnail{width:98px;height:68px}
.search-items .entry-title{font-size:14px}
.featured .widget{--height:180px}
.featured-items .cs{height:180px}
.featured-items .cs .entry-title{font-size:20px}
.featured-grid .entry-thumbnail{height:100px}
.featured-grid .entry-title{font-size:14px}
.list-items .entry-thumbnail{height:180px}
.grid-items .entry-thumbnail{height:180px}
.item-post h1.entry-title{font-size:27px}
.share-a .facebook .btn{width:38px}
.share-a .facebook .btn span{display:none}
.related-items .entry-thumbnail{height:90px}
.related-items .entry-title{font-size:14px}
.popular-items .cs{height:180px}
.popular-list .entry-thumbnail{width:98px;height:68px}
.popular-list .entry-title{font-size:14px}
.featured-post .cs{height:180px}
}
@media (max-width: 340px) {
.search-items .entry-thumbnail{width:88px;height:60px}
.item-post h1.entry-title{font-size:25px}
ul.share-b{gap:10px}
.slide-menu{width:100%}
.errorWrap h3{font-size:110px}
.errorWrap h4{font-size:27px}
}
]]></b:skin>
</b:if>
<b:if cond='data:view.isLayoutMode'>
<b:template-skin><![CDATA[
html,body#layout .site-outer,body#layout .row{width:auto;padding:0}
body#layout{position:relative;width:auto;max-width:100%;background-color:#fff;padding:95px 5px 0;margin:0 0 0 1px;border-width:1px 0 0;border-color:#eceff1}
body#layout:before{content:"SmartMag - v1.0.0";position:absolute;top:0;left:5px;right:5px;height:95px;font-family:Roboto,sans-serif;font-size:23px;color:#263238;line-height:95px;text-align:center}
body#layout div.section{display:block;background-color:#eceff1!important;margin:0 5px 10px!important;padding:16px 16px 18px!important;border:0}
body#layout .no-items.section{display:block}
body#layout .section h4{display:-webkit-box;font-size:14px;color:#263238;text-transform:uppercase;margin:0}
body#layout .section h4:after{text-transform:initial;color:#757575;font-weight:400}
body#layout .add_widget a{display:-webkit-box;color:#4385f5!important}
body#layout .widget-wrap3{overflow:hidden}
body#layout .widget-content{width:auto;max-width:none;max-height:none;margin:0;border:1px solid #e7e7e8;border-left:0}
body#layout .locked-widget .widget-content{border-left:1px solid #4385f5}
body#layout .locked-widget .widget-content:hover{border-left-color:#33a453}
body#layout div.layout-title{display:-webkit-box;color:#757575}
body#layout .widget .widget-content a.editlink{border-radius:2px}
body#layout .visibility .editlink{background:#4385f5 url(https://1.bp.blogspot.com/--z1wepFalfQ/YOObl8avCFI/AAAAAAAAAE8/Z-iC0j0LLpo7u2ZpHvW0hGaHhBOvVYYaQCLcBGAsYHQ/s48/edit.png) no-repeat center!important;background-size:20px!important}
body#layout .visibility .editlink:hover{background-color:#33a453!important}
body#layout .draggable-widget .widget-wrap2{background:#4385f5 url(https://1.bp.blogspot.com/-ciJD7MVmo10/YORQlzt9a1I/AAAAAAAAAFk/L4fK5cgelFoWX9rZvGFKZdr1d_RM9kfjACLcBGAsYHQ/s68/drag.png) no-repeat 4px 50%!important;background-size:4px auto!important}
body#layout .draggable-widget .widget-wrap1:hover .widget-wrap2{background-color:#33a453!important}
body#layout .visibility .layout-widget-state.visible{background-image:url(https://1.bp.blogspot.com/-aPoC3YxQo6g/YOOeDVSsJqI/AAAAAAAAAFM/oyvPLSJVIRQpAu-g0gZL89g5Caq4_4DeQCLcBGAsYHQ/s48/visibility_on.png)!important;background-size:24px!important}
body#layout .visibility .layout-widget-state.not-visible{background-image:url(https://1.bp.blogspot.com/-x_kkTMRQfHs/YOOeMUjTE8I/AAAAAAAAAFQ/RRj6YLBNuMEHwTB_81304fCxy8dl7h46gCLcBGAsYHQ/s48/visibility_off.png)!important;background-size:24px!important;opacity:1}
body#layout div.layout-widget-description{display:none;font-size:11px;line-height:1.2em}
body#layout #theme-options,body#layout #main-menu .widget{display:block!important}
body#layout div.pbt-panel{background-color:rgba(67,133,245,.15)!important;overflow:hidden!important}
body#layout .pbt-panel .widget{float:left;width:49.5%;margin-right:1%}
body#layout .pbt-panel .widget-content{border-color:#d5e3fc!important}
body#layout .pbt-panel .HTML{margin-right:0}
body#layout .pbt-panel div.layout-widget-description,body#layout .mobile-menu-toggle,body#layout .flex-right,body#layout .main-search{display:none}
body#layout .flex-left{display:flex}
body#layout .main-logo,body#layout .main-menu{width:50%}
body#layout .content-wrap{padding:0;margin:0}
body#layout .content-wrap > .container{display:flex;margin:0}
body#layout .main-wrap{width:67%;padding:0}
body#layout .sidebar-wrap{width:33%;padding:0}
body#layout #about{overflow:hidden!important}
body#layout #about .widget{float:left;width:49.5%;margin-right:1%}
body#layout #about .LinkList{margin-right:0}
body#layout .footer-bar .container{display:flex}
body#layout #footer-menu,body#layout #footer-copyright{width:50%}
body#layout .section > h4:after{font-size:12px}
body#layout #pbt-panel > h4:after{content:" - Default Thumbnail, Translate and More"}
body#layout #main-logo > h4:after{content:" - Main Logo"}
body#layout #main-menu > h4:after{content:" - Menu Links, Sub Links"}
body#layout #featured > h4:after{content:" - Popular Posts"}
body#layout #main > h4:after{content:" - Default Blog Posts, AdSense In-Feed, Comments and More"}
body#layout #related-posts > h4:after{content:" - Exclusive Non-Duplicate Post System"}
body#layout #sidebar > h4:after{content:" - Default Gadgets"}
body#layout #about > h4:after{content:" - Site Logo, Description and Social Icons"}
body#layout #footer-copyright > h4:after{content:" - Custom Credits"}
body#layout #footer-menu > h4:after{content:" - Custom Links"}
body#layout:after{content:"\0000a9\0000a0\Pro Blogger Templates - Core Version (2.0.0)";display:block;font-family:Roboto,sans-serif;font-size:14px;color:rgba(0,0,0,.54);line-height:1;text-align:center;visibility:visible;padding:20px 0 30px}
body#layout #hidden{display:none!important}
]]></b:template-skin>
</b:if>
<b:defaultmarkups>
  <b:defaultmarkup type='Common'>
    <b:includable id='customOpenGraphMetaData'>
      <!-- Open Graph Meta Tags -->
      <meta expr:content='data:blog.localeUnderscoreDelimited' property='og:locale'/>
      <b:if cond='data:view.isHomepage'>
        <meta content='website' property='og:type'/>
        <b:elseif cond='data:view.isSingleItem'/>
        <meta content='article' property='og:type'/>
        <b:elseif cond='data:view.isMultipleItems and not data:view.isHomepage'/>
        <meta content='object' property='og:type'/>
      </b:if>
      <meta expr:content='data:view.title.escaped' property='og:title'/>
      <meta expr:content='data:blog.title.escaped' property='og:site_name'/>
      <meta expr:content='data:view.description.escaped' property='og:description'/>
      <meta expr:content='data:blog.url.canonical' property='og:url'/>
      <b:tag cond='data:view.isMultipleItems and data:widgets.Blog.first.posts[0].featuredImage' expr:content='data:widgets.Blog.first.posts[0].featuredImage resizeImage 1600' name='meta' property='og:image'/>
      <b:tag cond='data:view.featuredImage' expr:content='data:view.featuredImage resizeImage 1600' name='meta' property='og:image'/>
      <!-- Twitter Meta Tags -->
      <meta content='summary_large_image' name='twitter:card'/>
    </b:includable>
    <b:includable id='pbt-head'>
      <meta content='blogger' name='generator'/>
      <meta expr:content='&quot;text/html; charset=&quot; + data:blog.encoding' http-equiv='Content-Type'/>
      <meta content='width=device-width, initial-scale=1, minimum-scale=1, user-scalable=yes' name='viewport'/>
      <!-- DNS Prefetch -->
      <link href='//fonts.googleapis.com' rel='preconnect'/>
      <link crossorigin='' href='//fonts.gstatic.com' rel='preconnect'/>
      <link href='//cdnjs.cloudflare.com' rel='preconnect'/>
      <link href='//blogger.googleusercontent.com' rel='dns-prefetch'/>
      <link href='//1.bp.blogspot.com' rel='dns-prefetch'/>
      <link href='//2.bp.blogspot.com' rel='dns-prefetch'/>
      <link href='//3.bp.blogspot.com' rel='dns-prefetch'/>
      <link href='//4.bp.blogspot.com' rel='dns-prefetch'/>
      <link href='//www.blogger.com' rel='dns-prefetch'/>
      <!-- Site Info -->
      <title><data:view.title.escaped/></title>
      <b:if cond='!data:isFeed'>
        <meta expr:content='data:view.description.escaped' name='description'/>
        <link expr:href='data:view.url.canonical' rel='canonical'/>
        <b:if cond='data:blog.adultContent'>
          <meta content='adult' name='rating'/>
        </b:if>
        <link expr:href='data:blog.blogspotFaviconUrl' rel='icon' type='image/x-icon'/>
        <meta expr:content='data:skin.vars.browser_bg' name='theme-color'/>
        <b:include name='customOpenGraphMetaData'/>
        <b:if cond='data:blog.feedLinks'>
          <!-- Feed Links -->
          <data:blog.feedLinks/><data:blog.meTag/>
        </b:if>
        <b:if cond='data:view.isHomepage'>
          <!-- Schema Markup -->
          <script type='application/ld+json'>{&quot;@context&quot;:&quot;http://schema.org&quot;,&quot;@type&quot;:&quot;WebSite&quot;,&quot;name&quot;:&quot;<data:view.title.escaped/>&quot;,&quot;url&quot;:&quot;<data:view.url.canonical/>&quot;,&quot;potentialAction&quot;:{&quot;@type&quot;:&quot;SearchAction&quot;,&quot;target&quot;:&quot;<data:view.url.canonical/>search?q={search_term_string}&quot;,&quot;query-input&quot;:&quot;required name=search_term_string&quot;}}</script>
        </b:if>
        <!-- Google Fonts -->
        <b:if cond='data:blog.languageDirection != &quot;rtl&quot;'>
          <b:with value='[data:skin.vars.main_font_family, data:skin.vars.title_font_family, data:skin.vars.text_font_family]' var='fonts'>
            <b:loop index='i' values='data:fonts' var='font'>
              <b:if cond='not(data:font contains &quot;,&quot;)'>
                <b:with value='&quot;https://fonts.googleapis.com/css2?family=&quot; + data:font + &quot;:ital,wght@0,400;0,500;0,600;0,700;1,400;1,500;1,600;1,700&amp;display=swap&quot;' var='fontLink'>
                  <b:tag cond='data:i == 0' expr:href='data:fontLink' name='link' rel='stylesheet'/>
                  <b:tag cond='data:i == 1 and (data:font not in [data:fonts[0]])' expr:href='data:fontLink' name='link' rel='stylesheet'/>
                  <b:tag cond='data:i == 2 and (data:font not in [data:fonts[0], data:fonts[1]])' expr:href='data:fontLink' name='link' rel='stylesheet'/>
                </b:with>
              </b:if>
            </b:loop>
          </b:with>
          <b:else/>
          <link href='https://fonts.googleapis.com/css2?family=Cairo:wght@400;500;600;700&amp;display=swap' rel='stylesheet'/>
        </b:if>
        <!-- Bootstrap Icons -->
        <b:tag href='https://cdnjs.cloudflare.com/ajax/libs/bootstrap-icons/1.10.2/font/bootstrap-icons.min.css' name='link' rel='stylesheet'/>
        <!-- Site Styles -->
      </b:if>
    </b:includable>
    <b:includable id='body-class'>
      <b:if cond='!data:isFeed'>
        <b:class cond='data:view.isHomepage' name='is-home'/>
        <b:class cond='data:view.isMultipleItems' name='is-multiple'/>
        <b:class cond='data:view.isSingleItem' name='is-single'/>
        <b:class cond='data:view.isPage' name='is-page'/>
        <b:class cond='data:view.isPost' name='is-post'/>
        <b:class cond='data:view.isError' name='is-multiple is-error'/>
        <b:class cond='data:blog.isMobileRequest' name='is-mobile'/>
        <b:class cond='data:skin.vars.boxedMode == &quot;1px&quot;' name='is-boxed'/>
        <b:class cond='data:skin.vars.gradient == &quot;1px&quot;' name='is-gradient'/>
      </b:if>
    </b:includable>
    <b:includable id='widget-title'>
      <b:if cond='data:widget.type == &quot;HTML&quot; and data:title contains &quot;getMailchimp&quot;'>
        <b:class name='MailChimp'/>
      </b:if>
      <b:if cond='data:title == &quot;{ads}&quot;'>
        <b:class name='is-ad'/>
        <b:elseif cond='data:widget.type == &quot;AdSense&quot;'/>
        <b:class name='is-ad'/>
      </b:if>
      <b:if cond='data:defaultTitle or data:title'>
        <b:if cond='data:title != &quot;{ads}&quot; and not (data:widget.type == &quot;HTML&quot; and data:title contains &quot;getMailchimp&quot;)'>
          <b:if cond='data:widget.sectionId not in [&quot;pbt-panel&quot;,&quot;main-logo&quot;,&quot;main-menu&quot;,&quot;featured&quot;,&quot;about&quot;,&quot;footer-copyright&quot;,&quot;footer-menu&quot;,&quot;hidden&quot;]'>
            <div expr:class='data:widget.sectionId in [&quot;sidebar&quot;] ? &quot;title-wrap widget-title&quot; : &quot;widget-title&quot;'><h3 class='title'><data:title/></h3></div>
          </b:if>
        </b:if>
      </b:if>
    </b:includable>
    <b:includable id='post-category'>
      <b:if cond='data:post.labels and (data:skin.vars.postCategory == &quot;1px&quot;)'>
        <span class='entry-tag'><data:post.labels.first.name/></span>
      </b:if>
    </b:includable>
    <b:includable id='image-content'>
      <b:if cond='data:widget.sectionId == &quot;pbt-panel&quot;'>
        <b:tag name='script' type='text/javascript'>const noThumbnail = &quot;<b:eval expr='resizeImage(data:sourceUrl, 72, &quot;1:1&quot;)'/>&quot;;</b:tag>
        <b:elseif cond='data:widget.sectionId == &quot;main-logo&quot;'/>
        <a class='logo-img' expr:href='data:blog.homepageUrl.canonical' rel='home'>
          <img expr:alt='data:blog.title' expr:data-src='data:sourceUrl' expr:height='data:height' expr:src='data:sourceUrl' expr:width='data:width'/>
          <b:if cond='data:view.isMultipleItems'><h1 id='h1-off'><data:blog.title/></h1></b:if>
        </a>
        <b:elseif cond='data:widget.sectionId == &quot;about&quot;'/>
        <a class='footer-logo' expr:href='data:blog.homepageUrl.canonical' rel='home'>
          <img expr:alt='data:blog.title' expr:data-src='data:sourceUrl' expr:height='data:height' expr:id='data:widget.instanceId + &quot;_img&quot;' expr:src='data:sourceUrl' expr:width='data:width'/>
        </a>
        <b:if cond='data:caption'>
          <div class='footer-info'>
            <b:if cond='data:title'><h3 class='title'><data:title/></h3></b:if>
            <b:if cond='data:caption'><p class='image-caption excerpt'><data:caption/></p></b:if>
          </div>
        </b:if>
        <b:else/>
        <div class='widget-content'>
          <b:tag cond='data:link' expr:href='data:link' name='a'>
            <b:if cond='data:link and (data:title == &quot;{ads}&quot;)'>
              <b:attr name='rel' value='nofollow noopener'/>
              <b:attr name='target' value='_blank'/>
            </b:if>
            <img expr:alt='data:caption and (data:title == &quot;{ads}&quot;) ? data:caption : data:widget.instanceId' expr:height='data:height' expr:id='data:widget.instanceId + &quot;_img&quot;' expr:src='data:sourceUrl' expr:width='data:width'/>
          </b:tag>
          <b:if cond='data:caption and (data:title != &quot;{ads}&quot;)'>
            <p class='image-caption excerpt'><data:caption/></p>
          </b:if>
        </div>
      </b:if>
    </b:includable>
    <b:includable id='pagelist-content'>
      <div class='widget-content'>
        <ul class='link-list list-style'>
          <b:loop values='data:links' var='link'>
            <li><a expr:href='data:link.href'><data:link.title/></a></li>
          </b:loop>
        </ul>
      </div>
    </b:includable>
    <b:includable id='linklist-content'>
      <b:if cond='data:widget.sectionId in [&quot;sidebar&quot;,&quot;about&quot;]'>
        <b:tag class='widget-content' cond='data:widget.sectionId not in [&quot;about&quot;]' name='div'>
          <b:if cond='data:links any l =&gt; l.name contains &quot;getSocial&quot;'>
            <ul class='social-icons social color'>
              <b:loop values='data:links' var='link'>
                <b:if cond='!(data:link.name contains &quot;getSocial&quot;)'>
                  <li expr:class='data:link.name'><a expr:class='&quot;bi-&quot; + data:link.name + &quot; btn&quot;' expr:href='data:link.target' expr:title='data:link.name' rel='nofollow noopener' target='_blank'><b:attr cond='data:widget.sectionId in [&quot;sidebar&quot;]' name='data-text' value='true'/></a></li>
                </b:if>
              </b:loop>
            </ul>
            <b:else/>
            <ul class='link-list list-style'>
              <b:loop index='i' values='data:links' var='link'>
                <li><a expr:href='data:link.target'><data:link.name/></a></li>
              </b:loop>
            </ul>
          </b:if>
        </b:tag>
        <b:elseif cond='data:widget.sectionId == &quot;main-menu&quot;'/>
        <ul class='main-nav' id='main-nav'>
          <b:loop index='i' values='data:links' var='link'>
            <li expr:id='&quot;item-&quot; + data:i'><a expr:href='data:link.target'><data:link.name/></a></li>
          </b:loop>
        </ul>
        <b:else/>
        <b:tag class='widget-content' cond='data:widget.sectionId not in [&quot;footer-menu&quot;]' name='div'>
          <ul expr:class='data:widget.sectionId in [&quot;footer-menu&quot;] ? &quot;link-list&quot; : &quot;link-list list-style&quot;'>
            <b:loop values='data:links' var='link'>
              <li><a expr:href='data:link.target'><data:link.name/></a></li>
            </b:loop>
          </ul>
        </b:tag>
      </b:if>
    </b:includable>
    <b:includable id='html-content'>
      <b:if cond='data:widget.sectionId == &quot;pbt-panel&quot;'>
        <b:if cond='data:content != &quot;&quot;'>
          <b:with expr:value='data:content' var='option'>
            <b:if cond='data:option.translate'>
              <b:tag name='script' type='text/javascript'>
                <b:if cond='data:option.translate.pageOf'>const pageOf = &quot;<data:option.translate.pageOf/>&quot;;</b:if>
                <b:if cond='data:option.translate.prevMsg'>const prevMsg = &quot;<data:option.translate.prevMsg/>&quot;;</b:if>
                <b:if cond='data:option.translate.nextMsg'>const nextMsg = &quot;<data:option.translate.nextMsg/>&quot;;</b:if>
              </b:tag>
            </b:if>
          </b:with>
        </b:if>
        <b:elseif cond='data:widget.sectionId == &quot;related-posts&quot;'/>
        <b:if cond='data:content and ((data:content contains &quot;results&quot;) or (data:content contains &quot;label&quot;))'>
          <b:attr expr:value='data:content' name='data-shortcode'/>
          <b:else/>
          <b:attr name='data-shortcode' value='{getPosts}'/>
        </b:if>
        <b:else/>
        <b:include name='widget-title'/>
        <div class='widget-content'>
          <b:if cond='data:title contains &quot;getMailchimp&quot;'>
            <b:attr expr:value='data:title' name='data-shortcode'/>
            <div class='mailchimp-header'>
              <h3 class='mailchimp-title'><data:messages.subscribe/></h3>
              <p class='mailchimp-text excerpt'><data:messages.getEmailNotifications/></p>
            </div>
            <form expr:action='data:content' expr:onsubmit='&quot;window.open(\&quot;&quot; + data:content + &quot;\&quot;, \&quot;popupwindow\&quot;, \&quot;scrollbars=yes,width=550,height=520\&quot;); return true&quot;' method='post' name='mc-embedded-subscribe-form' novalidate='' target='popupwindow'>
              <input class='mailchimp-email-address' expr:aria-label='data:messages.emailAddress' expr:placeholder='data:messages.emailAddress' name='EMAIL' type='email' value=''/>
              <input class='mailchimp-submit btn' expr:value='data:messages.subscribe' name='subscribe' type='submit'/>
            </form>
            <b:else/>
            <data:content/>
          </b:if>
        </div>
      </b:if>
    </b:includable>
    <b:includable id='text-content'>
      <b:if cond='data:widget.sectionId == &quot;footer-copyright&quot;'>
        <data:content/>
        <b:else/>
        <b:include name='widget-title'/>
        <div class='widget-content excerpt'>
          <data:content/>
        </div>
      </b:if>
    </b:includable>
    <b:includable id='popular-content'>
      <b:if cond='data:i == 0'>
        <div expr:class='&quot;post cs item-&quot;+data:i'>
          <a class='entry-inner' expr:href='data:post.url.canonical' expr:title='data:post.title ? data:post.title : data:messages.noTitle'>
            <span class='entry-thumbnail'><span class='thumbnail' expr:data-src='data:post.featuredImage ? (data:post.featuredImage.isYouTube ? resizeImage(data:post.featuredImage.youtubeMaxResDefaultUrl.jsonEscaped, 72, &quot;1:1&quot;) : resizeImage(data:post.featuredImage, 72, &quot;1:1&quot;)) : &quot;https://resources.blogblog.com/img/blank.gif&quot;'/><b:class cond='data:post.featuredImage.isYouTube' name='yt-img'/></span>
            <div class='entry-header'>
              <b:include name='post-category'/>
              <h2 class='entry-title'><b:eval expr='data:post.title ? data:post.title : data:messages.noTitle'/></h2>
              <b:if cond='data:widgets.Blog.first.allBylineItems.author or data:widgets.Blog.first.allBylineItems.timestamp'><div class='entry-meta'><b:if cond='data:widgets.Blog.first.allBylineItems.author'><span class='entry-author'><span class='author-name'><data:post.author.name/></span></span></b:if><b:if cond='data:widgets.Blog.first.allBylineItems.timestamp'><span class='entry-time'><b:if cond='data:widgets.Blog.first.allBylineItems.author'><span class='sp'>-</span></b:if><time class='published' expr:datetime='data:post.date.iso8601'><data:post.date/></time></span></b:if></div></b:if>
            </div>
          </a>
        </div>
        <b:else/>
        <div expr:class='&quot;post item-&quot;+data:i'>
          <a class='entry-thumbnail' expr:href='data:post.url.canonical' expr:title='data:post.title ? data:post.title : data:messages.noTitle'><span class='thumbnail' expr:data-src='data:post.featuredImage ? (data:post.featuredImage.isYouTube ? resizeImage(data:post.featuredImage.youtubeMaxResDefaultUrl.jsonEscaped, 72, &quot;1:1&quot;) : resizeImage(data:post.featuredImage, 72, &quot;1:1&quot;)) : &quot;https://resources.blogblog.com/img/blank.gif&quot;'/><b:class cond='data:post.featuredImage.isYouTube' name='yt-img:x4'/></a>
          <div class='entry-header'>
            <h2 class='entry-title'><a expr:href='data:post.url.canonical'><b:eval expr='data:post.title ? data:post.title : data:messages.noTitle'/></a></h2>
            <b:if cond='data:widgets.Blog.first.allBylineItems.timestamp'><div class='entry-meta'><span class='entry-time'><time class='published' expr:datetime='data:post.date.iso8601'><data:post.date/></time></span></div></b:if>
          </div>
        </div>
      </b:if>
    </b:includable>
    <b:includable id='featured-content'>
      <b:class name='featured-post'/>
      <div class='post cs'>
        <a class='entry-inner' expr:href='data:post.url.canonical' expr:title='data:post.title ? data:post.title : data:messages.noTitle'>
          <span class='entry-thumbnail'><span class='thumbnail' expr:data-src='data:post.featuredImage ? (data:post.featuredImage.isYouTube ? resizeImage(data:post.featuredImage.youtubeMaxResDefaultUrl.jsonEscaped, 72, &quot;1:1&quot;) : resizeImage(data:post.featuredImage, 72, &quot;1:1&quot;)) : &quot;https://resources.blogblog.com/img/blank.gif&quot;'/><b:class cond='data:post.featuredImage.isYouTube' name='yt-img'/></span>
          <div class='entry-header'>
            <b:include name='post-category'/>
            <h2 class='entry-title'><b:eval expr='data:post.title ? data:post.title : data:messages.noTitle'/></h2>
            <b:if cond='data:widgets.Blog.first.allBylineItems.author or data:widgets.Blog.first.allBylineItems.timestamp'><div class='entry-meta'><b:if cond='data:widgets.Blog.first.allBylineItems.author'><span class='entry-author'><span class='author-name'><data:post.author.name/></span></span></b:if><b:if cond='data:widgets.Blog.first.allBylineItems.timestamp'><span class='entry-time'><b:if cond='data:widgets.Blog.first.allBylineItems.author'><span class='sp'>-</span></b:if><time class='published' expr:datetime='data:post.date.iso8601'><data:post.date/></time></span></b:if></div></b:if>
          </div>
        </a>
      </div>
    </b:includable>
    <b:includable id='contact-form-content'>
      <div class='widget-content contact-form-widget'>
        <form class='contact-form-form' name='contact-form'>
          <input class='contact-form-name cf-s' expr:ariby='data:contactFormNameMsg' expr:id='data:widget.instanceId + &quot;_contact-form-name&quot;' expr:placeholder='data:contactFormNameMsg' name='name' size='30' type='text' value=''/>
          <input class='contact-form-email cf-s' expr:ariby='data:contactFormEmailMsg + &quot; *&quot;' expr:id='data:widget.instanceId + &quot;_contact-form-email&quot;' expr:placeholder='data:contactFormEmailMsg + &quot; *&quot;' name='email' size='30' type='text' value=''/>
          <textarea class='contact-form-email-message cf-s' cols='25' expr:ariby='data:contactFormMessageMsg + &quot; *&quot;' expr:id='data:widget.instanceId + &quot;_contact-form-email-message&quot;' expr:placeholder='data:contactFormMessageMsg + &quot; *&quot;' name='email-message' rows='5'/>
          <input class='contact-form-button contact-form-button-submit btn' expr:id='data:widget.instanceId + &quot;_contact-form-submit&quot;' expr:value='data:contactFormSendMsg' type='button'/>
          <p class='contact-form-error-message' expr:id='data:widget.instanceId + &quot;_contact-form-error-message&quot;'/>
          <p class='contact-form-success-message' expr:id='data:widget.instanceId + &quot;_contact-form-success-message&quot;'/>
        </form>
      </div>
    </b:includable>
    <b:includable id='adsense-content'>
      <div class='widget-content'>
        <b:if cond='data:adCode'><data:adCode/><b:else/><b:include name='defaultAdUnit'/></b:if>
      </div>
    </b:includable>
    <b:includable id='share-modal'>
      <div class='share-modal'>
        <div class='modal-header'>
          <span class='title'><data:messages.shareToOtherApps/></span>
          <button class='hide-modal' expr:aria-label='data:messages.showLess'/>
        </div>
        <b:with value='data:view.url.canonical' var='shareUrl'>
          <b:with value='data:view.title.jsonEscaped' var='shareTitle'>
            <ul class='share-b social color'>
              <li class='facebook'><a class='bi-facebook btn pbt-wo' expr:href='&quot;https://www.facebook.com/sharer.php?u=&quot; + data:shareUrl' rel='nofollow noopener' title='Facebook'/></li>
              <li class='twitter'><a class='bi-twitter btn pbt-wo' expr:href='&quot;https://twitter.com/intent/tweet?url=&quot; + data:shareUrl' rel='nofollow noopener' title='Twitter'/></li>
              <li class='whatsapp'><a class='bi-whatsapp btn pbt-wo' expr:href='&quot;https://api.whatsapp.com/send?text=&quot; + data:shareTitle + &quot; | &quot; + data:shareUrl' rel='nofollow noopener' title='WhatsApp'/></li>
              <li class='pinterest-p'><a class='bi-pinterest btn pbt-wo' expr:href='&quot;https://www.pinterest.com/pin/create/button/?url=&quot; + data:shareUrl + &quot;&amp;media=&quot; + data:view.featuredImage + &quot;&amp;description=&quot; + data:shareTitle' rel='nofollow noopener' title='Pinterest'/></li>
              <li class='linkedin'><a class='bi-linkedin btn pbt-wo' expr:href='&quot;https://www.linkedin.com/shareArticle?mini=true&amp;url=&quot; + data:shareUrl + &quot;&amp;title=&quot; + data:shareTitle' rel='nofollow noopener' title='LinkedIn'/></li>
              <li class='reddit'><a class='bi-reddit btn pbt-wo' expr:href='&quot;https://reddit.com/submit?url=&quot; + data:shareUrl + &quot;&amp;title=&quot; + data:shareTitle' rel='nofollow noopener' title='Reddit'/></li>
              <li class='telegram'><a class='bi-telegram btn pbt-wo' expr:href='&quot;https://telegram.me/share/url?url=&quot; + data:shareUrl + &quot;&amp;text=&quot; + data:shareTitle' rel='nofollow noopener' title='Telegram'/></li>
              <li class='email'><a class='bi-email btn pbt-wo' expr:href='&quot;mailto:?subject=&quot; + data:shareTitle + &quot;&amp;body=&quot; + data:shareUrl' rel='nofollow noopener' title='Email'/></li>
            </ul>
          </b:with>
          <div class='modal-footer'>
            <span class='title'><data:messages.copy/> <data:messages.postLink/></span>
            <div class='copy-link'>
              <input expr:value='data:shareUrl' readonly='readonly'/>
              <button class='btn' expr:aria-label='data:messages.copy'><data:messages.copy/></button>
            </div>
          </div>
        </b:with>
      </div>
    </b:includable>
    <b:includable id='mobile-menu'>
      <div class='slide-menu'>
        <b:tag class='border-top' cond='data:skin.vars.border_top != &quot;0px&quot;' name='div'/>
        <div class='slide-menu-header'>
          <div class='mobile-logo'/>
          <button aria-label='Hide Menu' class='hide-mobile-menu'/>
        </div>
        <div class='slide-menu-flex'>
          <div class='mobile-menu' id='mobile-menu'/>
          <div class='mm-footer flex-col'/>
        </div>
      </div>
    </b:includable>
    <b:includable id='pbt-search'>
      <div class='main-search'>
        <div class='search-form'>
          <input autocomplete='off' class='search-input' expr:placeholder='data:messages.search' id='mys' type='text' value=''/>
          <button class='search' expr:aria-label='data:messages.search'/>
        </div>
        <div class='search-content'>
          <div class='search-results'/>
        </div>
      </div>
    </b:includable>
    <b:includable id='pbt-messages'>
      <b:switch var='data:message'><b:case value='prevPost'/><b:if cond='data:blog.locale.language == &quot;en&quot;'>Previous Post<b:elseif cond='data:blog.locale.language == &quot;es&quot;'/>Artículo Anterior<b:elseif cond='data:blog.locale.language == &quot;pt&quot;'/>Postagem Anterior<b:else/><data:messages.newer/></b:if><b:case value='nextPost'/><b:if cond='data:blog.locale.language == &quot;en&quot;'>Next Post<b:elseif cond='data:blog.locale.language == &quot;es&quot;'/>Artículo Siguiente<b:elseif cond='data:blog.locale.language == &quot;pt&quot;'/>Próxima Postagem<b:else/><data:messages.older/></b:if><b:case value='loadMorePosts'/><b:if cond='data:blog.locale.language == &quot;en&quot;'>Load More<b:elseif cond='data:blog.locale.language == &quot;es&quot;'/>Carga Más<b:elseif cond='data:blog.locale.language == &quot;pt&quot;'/>Carregar Mais<b:elseif cond='data:blog.locale.language == &quot;ar&quot;'/>تحميل المزيد<b:else/><data:messages.loadMorePosts/></b:if></b:switch>
    </b:includable>
    <b:includable id='pbt-var'>
      <b:tag name='script' type='text/javascript'>const pbt={isRTL:<b:eval expr='data:blog.languageDirection == &quot;rtl&quot; ? &quot;true&quot; : &quot;false&quot;'/>,isMultiple:<b:eval expr='data:view.isMultipleItems ? &quot;true&quot; : &quot;false&quot;'/>,isSingle:<b:eval expr='data:view.isSingleItem ? &quot;true&quot; : &quot;false&quot;'/>,isPost:<b:eval expr='data:view.isPost ? &quot;true&quot; : &quot;false&quot;'/>,isPage:<b:eval expr='data:view.isPage ? &quot;true&quot; : &quot;false&quot;'/>,isBoxed:<b:eval expr='data:skin.vars.boxedMode == &quot;1px&quot; ? &quot;true&quot; : &quot;false&quot;'/>,stickyMenu:<b:eval expr='data:skin.vars.stickyMenu == &quot;1px&quot; ? &quot;true&quot; : &quot;false&quot;'/>,stickySidebar:<b:eval expr='data:skin.vars.stickySidebar == &quot;1px&quot; ? &quot;true&quot; : &quot;false&quot;'/>,postAuthor:<b:eval expr='data:widgets.Blog.first.allBylineItems.author ? &quot;true&quot; : &quot;false&quot;'/>,postDate:<b:eval expr='data:widgets.Blog.first.allBylineItems.timestamp ? &quot;true&quot; : &quot;false&quot;'/>,postAuthorLabel:&quot;<b:eval expr='data:widgets.Blog.first.allBylineItems.author.label ? data:widgets.Blog.first.allBylineItems.author.label : &quot;&quot;'/>&quot;,postDateLabel:&quot;<b:eval expr='data:widgets.Blog.first.allBylineItems.timestamp.label ? data:widgets.Blog.first.allBylineItems.timestamp.label : &quot;&quot;'/>&quot;,postCategory:<b:eval expr='data:skin.vars.postCategory == &quot;1px&quot; ? &quot;true&quot; : &quot;false&quot;'/>,postSummary:<b:eval expr='data:skin.vars.postSummary == &quot;1px&quot; ? &quot;true&quot; : &quot;false&quot;'/>,showMore:&quot;<data:messages.showMore/>&quot;,viewAll:&quot;<data:messages.viewAll/>&quot;,noResults:&quot;<data:messages.noResultsFound/>&quot;,noTitle:&quot;<data:messages.noTitle/>&quot;,noThumb:&quot;https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEhG9GA0058_fE7q8dUjkpL56fvlwSQs-DyuNjRG1C3oYBoWDR2PYrDa0SKVYt6iEJ8pssbajfAujp0g51-SQimyZNawn0waVgbe8cwgMzSXRURuiG7bqguOahIkTzTgPOn67eoasTMjKkxPfqXg1ytQ4NMjLEAGpp3zKKtpo-PVacHSnidorgbmaOFlyQ/w72-h72-p-k-no-nu/ptb-nth.webp&quot;}</b:tag>
    </b:includable>
    <b:includable id='pbt-feeds'>
      <code id='data'>{&quot;version&quot;:&quot;1.0.0&quot;,&quot;encoding&quot;:&quot;UTF-8&quot;,&quot;author&quot;:{&quot;name&quot;:&quot;Pro Blogger Templates&quot;,&quot;url&quot;:&quot;https://probloggertemplates.com/&quot;}<b:if cond='!data:posts.empty'>,&quot;posts&quot;:[<b:loop index='i' values='data:posts' var='post'><b:if cond='data:i != 0'>,</b:if>{&quot;id&quot;:&quot;<data:post.id.jsonEscaped/>&quot;,&quot;published&quot;:{&quot;date&quot;:&quot;<data:post.date.jsonEscaped/>&quot;,&quot;datetime&quot;:&quot;<data:post.date.iso8601.jsonEscaped/>&quot;},&quot;author&quot;:&quot;<data:post.author.name.jsonEscaped/>&quot;,<b:if cond='data:post.labels'>&quot;category&quot;:&quot;<data:post.labels.first.name/>&quot;,</b:if>&quot;title&quot;:&quot;<b:eval expr='data:post.title ? data:post.title.jsonEscaped : data:messages.noTitle.jsonEscaped'/>&quot;,&quot;link&quot;:&quot;<data:post.url.canonical.jsonEscaped/>&quot;,&quot;thumbnail&quot;:{&quot;src&quot;:&quot;<b:if cond='data:post.featuredImage'><b:eval expr='data:post.featuredImage.isYouTube ? resizeImage(data:post.featuredImage.youtubeMaxResDefaultUrl.jsonEscaped, 72, &quot;1:1&quot;) : resizeImage(data:post.featuredImage.jsonEscaped, 72, &quot;1:1&quot;)'/><b:else/>https://resources.blogblog.com/img/blank.gif</b:if>&quot;,&quot;source&quot;:&quot;<b:eval expr='data:post.featuredImage.isYouTube ? &quot;youtube&quot; : &quot;blogger&quot;'/>&quot;}<b:if cond='data:post.snippets.short'>,&quot;summary&quot;:&quot;<data:post.snippets.short.jsonEscaped/>&quot;</b:if>}</b:loop>]</b:if>}</code>
    </b:includable>
  </b:defaultmarkup>
  <b:defaultmarkup type='LinkList'>
    <b:includable id='main' var='this'>
      <b:include name='widget-title'/>
      <b:include name='content'/>
    </b:includable>
    <b:includable id='content'>
      <b:include name='linklist-content'/>
    </b:includable>
  </b:defaultmarkup>
  <b:defaultmarkup type='TextList'>
    <b:includable id='main' var='this'>
      <b:include name='widget-title'/>
      <b:include name='content'/>
    </b:includable>
    <b:includable id='content'>
      <div class='widget-content'>
        <ul class='text-list list-style'>
          <b:loop values='data:items' var='item'>
            <li><data:item/></li>
          </b:loop>
        </ul>
      </div>
    </b:includable>
  </b:defaultmarkup>
  <b:defaultmarkup type='HTML'>
    <b:includable id='main'>
      <b:include name='html-content'/>
    </b:includable>
  </b:defaultmarkup>
  <b:defaultmarkup type='Text'>
    <b:includable id='main'>
      <b:include name='text-content'/>
    </b:includable>
  </b:defaultmarkup>
  <b:defaultmarkup type='Blog'>
    <b:includable id='main' var='this'>
      <b:class cond='data:view.isMultipleItems' name='index-blog flex-col'/>
      <b:if cond='!data:isFeed'>
        <b:include cond='data:view.isHomepage' name='blogPostsTitle'/>
        <b:include name='searchMessage'/>
        <b:if cond='!data:posts.empty'>
          <div class='blog-posts'>
            <b:class cond='data:view.isMultipleItems' expr:name='&quot;index-post-wrap&quot; + (data:skin.vars.gridStyle == &quot;1px&quot; ? &quot; grid-items&quot; : &quot; list-items&quot;)'/>
            <b:class cond='data:view.isSingleItem' name='item-post-wrap flex-col'/>
            <b:loop index='i' values='data:posts' var='post'>
              <b:include data='post' name='postCommentsAndAd'/>
            </b:loop>
          </div>
          <b:include cond='data:view.isMultipleItems' name='ajaxPagination'/>
        </b:if>
        <b:else/>
        <b:include name='pbt-feeds'/>
      </b:if>
    </b:includable>
    <b:includable id='blogPostsTitle'>
      <b:if cond='data:blog.jumpLinkMessage != &quot;{hide}&quot;'>
        <div class='title-wrap blog1-title'><h3 class='title'><data:blog.jumpLinkMessage/></h3><a class='title-link' href='/search'><data:messages.viewAll/></a></div>
      </b:if>
    </b:includable>
    <b:includable id='aboutPostAuthor'/>
    <b:includable id='addComments'>
      <a expr:href='data:post.commentsUrl' expr:onclick='data:post.commentsUrlOnclick'><data:messages.postAComment/></a>
    </b:includable>
    <b:includable id='ajaxPagination'>
      <!-- Ajax Pagination -->
      <b:if cond='data:olderPageUrl'>
        <div class='blog-pager'>
          <a class='load-more btn visible' expr:data-url='data:olderPageUrl.canonical' href='#' id='load-more'><b:include data='{ message: &quot;loadMorePosts&quot; }' name='pbt-messages'/></a>
          <div class='loading'><div class='loader'><svg class='spinner' viewBox='0 0 50 50'><circle class='path' cx='25' cy='25' r='20'/></svg></div></div>
          <span class='no-more btn'><data:messages.noResultsFound/></span>
        </div>
      </b:if>
    </b:includable>
    <b:includable id='backLinks' var='post'/>
    <b:includable id='blogThisShare'/>
    <b:includable id='bylineByName' var='byline'/>
    <b:includable id='bylineRegion' var='regionItems'/>
    <b:includable id='commentAuthorAvatar'/>
    <b:includable id='commentDeleteIcon' var='comment'/>
    <b:includable id='commentForm' var='post'>
      <div class='comment-form'>
        <a name='comment-form'/>
        <b:include data='post' name='commentFormIframeSrc'/>
        <iframe allowtransparency='allowtransparency' class='blogger-iframe-colorize blogger-comment-from-post' expr:height='data:cmtIframeInitialHeight ?: &quot;90px&quot;' frameborder='0' id='comment-editor' name='comment-editor' src='' width='100%'/>
        <data:post.cmtfpIframe/>
        <b:tag name='script' type='text/javascript'>
          BLOG_CMT_createIframe(&#39;<data:post.appRpcRelayPath/>&#39;);
        </b:tag>
      </div>
    </b:includable>
    <b:includable id='commentFormIframeSrc' var='post'>
      <a expr:href='data:post.commentFormIframeSrc params { skin: &quot;soho&quot; }' id='comment-editor-src' rel='nofollow noopener' title='Comment Form Link'/>
    </b:includable>
    <b:includable id='commentItem' var='comment'/>
    <b:includable id='commentList' var='comments'/>
    <b:includable id='commentPicker' var='post'/>
    <b:includable id='comments' var='post'>
      <a name='comments'/>
      <section class='comments threaded flex-col' expr:data-embed='data:post.embedCommentForm' expr:data-num-comments='data:post.numberOfComments' id='comments'>
        <b:class expr:name='data:post.numberOfComments != 0 ? &quot;has-comments&quot; : &quot;no-comments&quot;'/>
        <b:if cond='!data:post.allowNewComments'>
          <b:class name='no-comment-form'/>
        </b:if>
        <b:include name='commentsTitle'/>
        <b:if cond='data:post.allowNewComments'>
          <b:if cond='data:this.messages.blogComment'><p class='comments-message excerpt'><data:this.messages.blogComment/></p></b:if>
          <b:else/>
          <b:if cond='data:post.noNewCommentsText and (data:post.numberOfComments == 0)'><p class='comments-message excerpt'><data:post.noNewCommentsText/><em>*</em></p></b:if>
        </b:if>
        <b:if cond='data:post.embedCommentForm'>
          <b:if cond='data:post.numberOfComments != 0'>
            <div class='comments-content'>
              <div id='comment-holder'>
                <data:post.commentHtml/>
              </div>
            </div>
          </b:if>
          <b:if cond='data:post.allowNewComments'>
            <b:include data='post' name='commentForm'/>
          </b:if>
          <b:if cond='data:post.allowNewComments'><button class='show-cf btn' expr:aria-label='data:messages.postAComment'><data:messages.postAComment/><b:if cond='data:post.numberOfComments == 0'> (<data:post.numberOfComments/>)</b:if></button></b:if>
          <b:if cond='!data:post.allowNewComments'><b:if cond='data:post.noNewCommentsText and (data:post.numberOfComments != 0)'><p class='comments-message excerpt'><data:post.noNewCommentsText/><em>*</em></p></b:if></b:if>
          <b:else/>
          <p class='comments-message excerpt'>Please Select Embedded Mode To Show The Comment System.<em>*</em></p>
        </b:if>
      </section>
    </b:includable>
    <b:includable id='commentsTitle'>
      <!-- Comments Title -->
      <b:if cond='data:post.numberOfComments != 0'><div class='title-wrap comments-title'><b:class expr:name='data:this.messages.blogComment ? &quot;has-message&quot; : &quot;no-message&quot;'/><h3 class='title'><data:post.numberOfComments/> <data:messages.comments/></h3></div></b:if>
    </b:includable>
    <b:includable id='defaultAdUnit'>
      <ins class='adsbygoogle' data-ad-format='fluid' data-ad-layout-key='-g2-16+9a-5i-kj' data-full-width-responsive='false' expr:data-ad-client='data:adClientId ?: data:blog.adsenseClientId' expr:data-ad-host='data:blog.adsenseHostId' expr:data-analytics-uacct='data:blog.analyticsAccountNumber' style='display:block'/>
      <script>(adsbygoogle = window.adsbygoogle || []).push({});</script>
    </b:includable>
    <b:includable id='emailPostIcon'/>
    <b:includable id='facebookShare'/>
    <b:includable id='feedLinks'/>
    <b:includable id='feedLinksBody' var='links'/>
    <b:includable id='footerBylines'/>
    <b:includable id='googlePlusShare'/>
    <b:includable id='headerByline' var='post'>
      <!-- Post Entry Meta -->
      <b:if cond='data:view.isMultipleItems'>
        <b:if cond='data:allBylineItems.author or data:allBylineItems.timestamp'>
          <div class='entry-meta'>
            <b:include cond='data:allBylineItems.author' data='post' name='postAuthor'/>
            <b:include cond='data:allBylineItems.timestamp' data='post' name='postTimestamp'/>
          </div>
        </b:if>
      </b:if>
      <b:if cond='data:view.isPost'>
        <b:if cond='data:allBylineItems.author or data:allBylineItems.timestamp'>
          <b:class name='has-meta'/>
          <div class='entry-meta'>
            <div class='align-left'>
              <b:class cond='data:allBylineItems.timestamp' name='has-time'/>
              <b:if cond='data:allBylineItems.author'><span class='entry-avatar'><span class='avatar' expr:data-src='data:post.author.authorPhoto.image ? resizeImage(data:post.author.authorPhoto.image, 72, &quot;1:1&quot;) : &quot;https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEiCxxt0n6b048h4UEHf-L5T22U8xCk-IsG2qbfVUMBMKdt2t3ijO6qz--5UBg63qH4V_6z8uIBe7z6VNnueFbF3XKIWkCJPmFQqfm3Rmx3tpBOk74LGDZrUEgGnJF2-VDrzlkZSVyJs2sYjtiCytrEjsw23o88dqy5mdjw0KPwNuySVA7iYfdHWYpgsuQ/w72-h72-p-k-no-nu/avatar.webp&quot;'/></span></b:if>
              <b:tag class='al-items' cond='data:allBylineItems.author and data:allBylineItems.timestamp' name='div'>
              <b:include cond='data:allBylineItems.author' data='post' name='postAuthor'/>
              <b:include cond='data:allBylineItems.timestamp' data='post' name='postTimestamp'/>
              </b:tag>
            </div>
            <b:if cond='data:allBylineItems.share'>
              <div class='align-right'>
                <button class='share-toggle' expr:aria-label='data:messages.share'/>
              </div>
            </b:if>
          </div>
        </b:if>
      </b:if>
    </b:includable>
    <b:includable id='homePageLink'/>
    <b:includable id='iframeComments' var='post'/>
    <b:includable id='indexPost' var='post'>
      <!-- Index Post Content -->
      <b:include data='post' name='postFeaturedImage'/>
      <div class='entry-header'>
        <b:include data='post' name='postHeader'/>
        <b:include cond='(data:skin.vars.gridStyle != &quot;1px&quot;) and (data:skin.vars.postSummary == &quot;1px&quot;)' data='post' name='postBodySnippet'/>
        <b:include data='post' name='headerByline'/>
      </div>
    </b:includable>
    <b:includable id='inlineAd' var='post'/>
    <b:includable id='itemPostData' var='post'>
      <b:tag id='data' name='script' type='application/json'>{&quot;postData&quot;:[{&quot;published&quot;:{&quot;date&quot;:&quot;<data:post.date.jsonEscaped/>&quot;,&quot;datetime&quot;:&quot;<data:post.date.iso8601.jsonEscaped/>&quot;},&quot;author&quot;:&quot;<data:post.author.name.jsonEscaped/>&quot;,<b:if cond='data:post.labels'>&quot;category&quot;:&quot;<data:post.labels.first.name/>&quot;,</b:if>&quot;title&quot;:&quot;<b:eval expr='data:post.title ? data:post.title.jsonEscaped : data:messages.noTitle.jsonEscaped'/>&quot;,&quot;link&quot;:&quot;<data:post.url.canonical.jsonEscaped/>&quot;,&quot;thumbnail&quot;:{&quot;src&quot;:&quot;<b:if cond='data:post.featuredImage'><b:eval expr='data:post.featuredImage.isYouTube ? resizeImage(data:post.featuredImage.youtubeMaxResDefaultUrl.jsonEscaped, 72, &quot;1:1&quot;) : resizeImage(data:post.featuredImage.jsonEscaped, 72, &quot;1:1&quot;)'/><b:else/>https://resources.blogblog.com/img/blank.gif</b:if>&quot;,&quot;source&quot;:&quot;<b:eval expr='data:post.featuredImage.isYouTube ? &quot;youtube&quot; : &quot;blogger&quot;'/>&quot;}}]}</b:tag>
    </b:includable>
    <b:includable id='itemPost' var='post'>
      <!-- Item Post Content -->
      <b:include cond='data:view.isPost' data='post' name='itemPostData'/>
      <div class='item-post-inner flex-col'>
        <div class='entry-header post-header'>
          <b:include data='post' name='postHeader'/>
        </div>
        <div class='entry-content-wrap flex-col'>
          <b:include data='post' name='postBody'/>
        </div>
        <b:include cond='data:view.isPost and data:allBylineItems.labels' data='post' name='postLabels'/>
        <b:include cond='data:view.isPost and data:allBylineItems.share' data='post' name='postShareButtons'/>
      </div>
    </b:includable>
    <b:includable id='linkShare'/>
    <b:includable id='nextPageLink'>
      <b:if cond='data:olderPageUrl'>
        <a class='post-nav-link post-nav-older-link' expr:href='data:olderPageUrl.canonical'>
          <b:include data='{ message: &quot;nextPost&quot; }' name='pbt-messages'/>
        </a>
        <b:else/>
        <span class='post-nav-link post-nav-older-link'>
          <b:include data='{ message: &quot;nextPost&quot; }' name='pbt-messages'/>
        </span>
      </b:if>
    </b:includable>
    <b:includable id='otherSharingButton'/>
    <b:includable id='platformShare'/>
    <b:includable id='post' var='post'>
      <!-- Index Posts -->
      <b:if cond='data:view.isMultipleItems'>
        <b:include data='post' name='indexPost'/>
      </b:if>
      <!-- Item Post -->
      <b:if cond='data:view.isSingleItem'>
        <b:include data='post' name='itemPost'/>
      </b:if>
    </b:includable>
    <b:includable id='postAuthor' var='post'>
      <!-- Post Author -->
      <span class='entry-author'><b:if cond='data:allBylineItems.author.label and data:view.isPost'><span class='by sp'><data:allBylineItems.author.label/></span></b:if><span class='author-name'><data:post.author.name/></span></span>
    </b:includable>
    <b:includable id='postBody' var='post'> 
      <!-- Post Body Entry Content -->
      <div class='post-body entry-content' id='post-body'>
        <data:post.body/>
      </div>
    </b:includable>
    <b:includable id='postBodySnippet' var='post'><p class='entry-excerpt excerpt'><b:eval expr='data:post.snippets.long snippet { length: 65 }'/></p></b:includable>
    <b:includable id='postBreadcrumbs' var='post'>
      <!-- Post Breadcrumbs -->
      <nav id='breadcrumb'><a class='home' expr:href='data:blog.homepageUrl.canonical'><data:messages.home/></a><b:if cond='data:post.labels'><i class='sep'/><a class='label' expr:href='data:post.labels.first.url.canonical'><data:post.labels.first.name/></a></b:if></nav>
    </b:includable>
    <b:includable id='postCategory' var='post'>
      <!-- Post Category -->
      <b:include name='post-category'/>
    </b:includable>
    <b:includable id='postCommentsAndAd' var='post'>
      <b:include data='post' name='postMeta'/>
      <article>
        <b:class cond='data:view.isMultipleItems' expr:name='&quot;post hentry item-&quot; + data:i'/>
        <b:class cond='data:view.isSingleItem' name='item-post hentry'/>
        <b:include data='post' name='post'/>
      </article>
      <b:include cond='data:view.isPost' data='post' name='postFooter'/>
      <b:if cond='data:view.isSingleItem and data:post.allowComments'>
        <!-- Post Comments -->
        <div class='blog-post-comments p-widget' expr:data-shortcode='data:allBylineItems.comments.label contains &quot;type&quot; ? data:allBylineItems.comments.label : &quot;$type={blogger}&quot;'>
          <b:include data='post' name='comments'/>
        </div>
      </b:if>
      <!-- Post Navigation -->
      <b:include cond='data:skin.vars.postnav == &quot;1px&quot;' name='postPagination'/>
    </b:includable>
    <b:includable id='postCommentsLink'/>
    <b:includable id='postFeaturedImage' var='post'>
      <!-- Post Featured Image -->
      <a expr:class='data:post.featuredImage.isYouTube ? &quot;entry-thumbnail yt-img&quot; : &quot;entry-thumbnail&quot;' expr:href='data:post.url.canonical' expr:title='data:post.title ? data:post.title : data:messages.noTitle'><span class='thumbnail' expr:data-src='data:post.featuredImage ? (data:post.featuredImage.isYouTube ? resizeImage(data:post.featuredImage.youtubeMaxResDefaultUrl.jsonEscaped, 72, &quot;1:1&quot;) : resizeImage(data:post.featuredImage, 72, &quot;1:1&quot;)) : &quot;https://resources.blogblog.com/img/blank.gif&quot;'/><b:include data='post' name='postCategory'/></a>
    </b:includable>
    <b:includable id='postFooter' var='post'>
      <!-- Post Footer Items -->
      <div class='post-footer flex-col'>
        <b:include cond='data:post.author.aboutMe' data='post' name='postFooterAuthorProfile'/>
        <b:include cond='data:widgets.HTML any w =&gt; w.sectionId == &quot;related-posts&quot;' data='post' name='relatedPosts'/>
      </div>
    </b:includable>
    <b:includable id='postFooterAuthorProfile' var='post'>
      <div class='about-author p-widget'>
        <div class='author-avatar entry-avatar'>
          <span class='avatar' expr:data-src='data:post.author.authorPhoto.image ? resizeImage(data:post.author.authorPhoto.image, 72, &quot;1:1&quot;) : &quot;https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEiCxxt0n6b048h4UEHf-L5T22U8xCk-IsG2qbfVUMBMKdt2t3ijO6qz--5UBg63qH4V_6z8uIBe7z6VNnueFbF3XKIWkCJPmFQqfm3Rmx3tpBOk74LGDZrUEgGnJF2-VDrzlkZSVyJs2sYjtiCytrEjsw23o88dqy5mdjw0KPwNuySVA7iYfdHWYpgsuQ/w72-h72-p-k-no-nu/avatar.webp&quot;'/>
        </div>
        <div class='author-description flex-col'>
          <h3 class='author-title'><data:post.author.name/><b:attr cond='data:post.author.profileUrl' expr:value='data:post.author.profileUrl' name='profile-url'/></h3>
          <p class='author-text excerpt'><data:post.author.aboutMe/></p>
        </div>
      </div>
    </b:includable>
    <b:includable id='postHeader' var='post'>
      <b:include cond='data:view.isPost and (data:skin.vars.breadcrumb == &quot;1px&quot;)' data='post' name='postBreadcrumbs'/>
      <b:include data='post' name='postTitle'/>
      <b:include cond='data:view.isPost' data='post' name='headerByline'/>
    </b:includable>
    <b:includable id='postJumpLink' var='post'>
      <b:if cond='data:blog.jumpLinkMessage != &quot;hide&quot;'>
        <a class='read-more' expr:href='data:post.url.canonical'><data:blog.jumpLinkMessage/></a>
      </b:if>
    </b:includable>
    <b:includable id='postLabels' var='post'>
      <b:if cond='data:post.labels'>
        <div class='entry-labels'>
          <b:if cond='data:allBylineItems.labels.label'><span class='labels-label btn'><data:allBylineItems.labels.label/></span></b:if>
          <b:loop values='data:post.labels' var='label'>
            <a class='label-link btn' expr:href='data:label.url.canonical' rel='tag'><data:label.name/></a>
          </b:loop>
        </div>
      </b:if>
    </b:includable>
    <b:includable id='postLocation'/>
    <b:includable id='postMeta' var='post'>
      <b:if cond='data:view.isPost'>
        <b:tag name='script' type='application/ld+json'>{&quot;@context&quot;:&quot;https://schema.org&quot;,&quot;@graph&quot;:[{&quot;@type&quot;:&quot;NewsArticle&quot;,&quot;mainEntityOfPage&quot;:{&quot;@type&quot;:&quot;WebPage&quot;,&quot;@id&quot;:&quot;<data:post.url.canonical.jsonEscaped/>&quot;},&quot;headline&quot;:&quot;<data:post.title.jsonEscaped/>&quot;,&quot;description&quot;:&quot;<data:post.snippets.short.jsonEscaped/>&quot;,&quot;datePublished&quot;:&quot;<data:post.date.iso8601.jsonEscaped/>&quot;,&quot;dateModified&quot;:&quot;<data:post.lastUpdated.iso8601.jsonEscaped/>&quot;,&quot;image&quot;:{&quot;@type&quot;:&quot;ImageObject&quot;,<b:if cond='data:post.featuredImage.isResizable'>&quot;url&quot;:&quot;<b:eval expr='resizeImage(data:post.featuredImage, 1200, &quot;1200:675&quot;)'/>&quot;,&quot;height&quot;:675,&quot;width&quot;:1200<b:else/>&quot;url&quot;:&quot;https://lh3.googleusercontent.com/ULB6iBuCeTVvSjjjU1A-O8e9ZpVba6uvyhtiWRti_rBAs9yMYOFBujxriJRZ-A=w1200&quot;,&quot;height&quot;:348,&quot;width&quot;:1200</b:if>},&quot;author&quot;:{&quot;@type&quot;:&quot;Person&quot;,&quot;name&quot;:&quot;<data:post.author.name.jsonEscaped/>&quot;<b:if cond='data:post.author.profileUrl'>,&quot;url&quot;:&quot;<data:post.author.profileUrl.jsonEscaped/>&quot;</b:if>},&quot;publisher&quot;:{&quot;@type&quot;:&quot;Organization&quot;,&quot;name&quot;:&quot;Blogger&quot;,&quot;logo&quot;:{&quot;@type&quot;:&quot;ImageObject&quot;,&quot;url&quot;:&quot;https://lh3.googleusercontent.com/ULB6iBuCeTVvSjjjU1A-O8e9ZpVba6uvyhtiWRti_rBAs9yMYOFBujxriJRZ-A=h60&quot;,&quot;width&quot;:206,&quot;height&quot;:60}}},{&quot;@type&quot;:&quot;BreadcrumbList&quot;,&quot;itemListElement&quot;:[{&quot;@type&quot;:&quot;ListItem&quot;,&quot;position&quot;:1,&quot;name&quot;:&quot;<data:messages.home.jsonEscaped/>&quot;,&quot;item&quot;:&quot;<data:blog.homepageUrl.canonical.jsonEscaped/>&quot;},{&quot;@type&quot;:&quot;ListItem&quot;,&quot;position&quot;:2,&quot;name&quot;:&quot;<b:if cond='data:post.labels'><data:post.labels.first.name.jsonEscaped/><b:else/><data:messages.posts/></b:if>&quot;,&quot;item&quot;:&quot;<b:if cond='data:post.labels'><data:post.labels.first.url.canonical.jsonEscaped/><b:else/><b:eval expr='data:blog.homepageUrl.canonical.jsonEscaped + &quot;search/&quot;'/></b:if>&quot;},{&quot;@type&quot;:&quot;ListItem&quot;,&quot;position&quot;:3,&quot;name&quot;:&quot;<data:post.title.jsonEscaped/>&quot;,&quot;item&quot;:&quot;<data:post.url.canonical.jsonEscaped/>&quot;}]}]}</b:tag>
      </b:if>
      <b:if cond='data:view.isPage'>
        <b:tag name='script' type='application/ld+json'>{&quot;@context&quot;:&quot;http://schema.org&quot;,&quot;@type&quot;:&quot;BreadcrumbList&quot;,&quot;itemListElement&quot;:[{&quot;@type&quot;:&quot;ListItem&quot;,&quot;position&quot;:1,&quot;name&quot;:&quot;<data:messages.home.jsonEscaped/>&quot;,&quot;item&quot;:&quot;<data:blog.homepageUrl.canonical.jsonEscaped/>&quot;},{&quot;@type&quot;:&quot;ListItem&quot;,&quot;position&quot;:2,&quot;name&quot;:&quot;<data:post.title.jsonEscaped/>&quot;,&quot;item&quot;:&quot;<data:post.url.canonical.jsonEscaped/>&quot;}]}</b:tag>
      </b:if>
    </b:includable>
    <b:includable id='postMetadataJSONImage'/>
    <b:includable id='postMetadataJSONPublisher'/>
    <b:includable id='postPagination'>
      <b:if cond='data:view.isPost'>
        <div class='post-nav p-widget'>
          <b:include name='previousPageLink'/>
          <b:include name='nextPageLink'/>
        </div>
      </b:if>
    </b:includable>
    <b:includable id='postReactions'/>
    <b:includable id='postShareButtons' var='post'>
      <!-- Post Share Buttons -->
      <div class='post-share'>
        <ul class='share-a social color'>
          <li class='share-label'><span class='sl-btn btn'><i class='sl-ico'/></span></li>
          <li class='facebook has-span'><a class='bi-facebook btn pbt-wo' expr:href='&quot;https://www.facebook.com/sharer.php?u=&quot; + data:post.url.canonical' rel='nofollow noopener' title='Facebook'><span>Facebook</span></a></li>
          <li class='twitter has-span'><a class='bi-twitter btn pbt-wo' expr:href='&quot;https://twitter.com/intent/tweet?url=&quot; + data:post.url.canonical' rel='nofollow noopener' title='Twitter'><span>Twitter</span></a></li>
          <li class='whatsapp'><a class='bi-whatsapp btn pbt-wo' expr:href='&quot;https://api.whatsapp.com/send?text=&quot; + data:post.title.jsonEscaped + &quot; | &quot; + data:post.url.canonical' rel='nofollow noopener' title='WhatsApp'/></li>
          <li class='email'><a class='bi-email btn pbt-wo' expr:href='&quot;mailto:?subject=&quot; + data:post.title.jsonEscaped + &quot;&amp;body=&quot; + data:post.url.canonical' rel='nofollow noopener' title='Email'/></li>
          <li class='show-more'><button class='btn' expr:aria-label='data:messages.showMore'/></li>
        </ul>
      </div>
    </b:includable>
    <b:includable id='postTimestamp' var='post'>
      <!-- Post Timestamp -->
      <span class='entry-time'><b:if cond='data:allBylineItems.author and data:allBylineItems.timestamp.label'><span class='sp'><data:allBylineItems.timestamp.label/></span></b:if><time class='published' expr:datetime='data:post.date.iso8601'><data:post.date/></time></span>
    </b:includable>
    <b:includable id='postTitle' var='post'>
      <!-- Post Title Index and Item -->
      <b:if cond='data:view.isMultipleItems'>
        <h2 class='entry-title'><a expr:href='data:post.url.canonical' rel='bookmark'><b:eval expr='data:post.title ? data:post.title : data:messages.noTitle'/></a></h2>
      </b:if>
      <b:if cond='data:view.isSingleItem'>
        <h1 class='entry-title'><b:eval expr='data:post.title ? data:post.title : data:messages.noTitle'/></h1>
      </b:if>
    </b:includable>
    <b:includable id='previousPageLink'>
      <b:if cond='data:newerPageUrl'>
        <a class='post-nav-link post-nav-newer-link' expr:href='data:newerPageUrl.canonical'>
          <b:include data='{ message: &quot;prevPost&quot; }' name='pbt-messages'/>
        </a>
        <b:else/>
        <span class='post-nav-link post-nav-newer-link'>
          <b:include data='{ message: &quot;prevPost&quot; }' name='pbt-messages'/>
        </span>
      </b:if>
    </b:includable>
    <b:includable id='relatedPosts' var='post'>
      <!-- Related Posts -->
      <div class='related-wrap p-widget'>
        <div class='title-wrap related-title'>
          <b:with value='data:widgets.HTML filter (w =&gt; w.sectionId == &quot;related-posts&quot;) map (w =&gt; w.title)' var='pbtTitle'>
            <h3 class='title'><b:eval expr='data:pbtTitle.first ? data:pbtTitle.first : data:messages.youMayLikeThesePosts'/></h3>
            <a class='title-link' expr:href='data:post.labels ? &quot;/search/label/&quot; + data:post.labels.first.name : &quot;/search&quot;'><data:messages.viewAll/></a>
          </b:with>
        </div>
        <div class='widget-content'>
          <span class='related-tag' expr:data-id='data:post.id' expr:data-label='data:post.labels ? data:post.labels.first.name : &quot;recent&quot;'/>
        </div> 
      </div>  
    </b:includable>
    <b:includable id='searchMessage'>
      <!-- Search Message -->
      <b:if cond='data:posts.empty'>
        <b:class name='no-posts'/>
      </b:if>
      <b:if cond='data:view.search.query'>
        <div class='queryMessage'>
          <b:if cond='data:posts.empty'>
            <span class='query-info query-error'>&quot;<data:view.search.query/>&quot;</span>
            <b:else/>
            <span class='query-info query-success'>&quot;<data:view.search.query/>&quot;</span>
          </b:if>
        </div>
      </b:if>
      <b:if cond='data:view.search.label'>
        <div class='queryMessage '>
          <b:if cond='data:posts.empty'>
            <span class='query-info query-label query-error'><data:view.search.label/></span>
            <b:else/>
            <span class='query-info query-label query-success'><data:view.search.label/></span>
          </b:if>
        </div>
      </b:if>
      <b:if cond='data:view.isArchive'>
        <div class='queryMessage'>
          <b:if cond='data:posts.empty'>
            <span class='query-info query-error'><data:view.archive.rangeMessage/></span>
            <b:else/>
            <span class='query-info query-success'><data:view.archive.rangeMessage/></span>
          </b:if>
        </div>
      </b:if>
      <b:if cond='data:view.isError'>
        <div class='errorWrap'>
          <h3>404</h3>
          <h4><data:messages.theresNothingHere/></h4>
          <p><data:navMessage/></p>
          <a class='homepage btn' expr:href='data:blog.homepageUrl'><data:messages.home/></a>
        </div>
      </b:if>
      <b:if cond='data:view.isMultipleItems and data:posts.empty'><div class='queryEmpty'><data:messages.noResultsFound/></div></b:if>
    </b:includable>
    <b:includable id='sharingButton'/>
    <b:includable id='sharingButtonContent'/>
    <b:includable id='sharingButtons'/>
    <b:includable id='sharingButtonsMenu'/>
    <b:includable id='sharingPlatformIcon'/>
    <b:includable id='threadedCommentForm' var='post'/>
    <b:includable id='threadedCommentJs' var='post'/>
    <b:includable id='threadedComments' var='post'/>
    <b:includable id='threadedCommentsDisqus' var='post'/>
  </b:defaultmarkup>
  <b:defaultmarkup type='PopularPosts'>
    <b:includable id='main' var='this'>
      <b:include name='widget-title'/>
      <div class='widget-content'>
        <b:if cond='data:widget.sectionId == &quot;featured&quot;'>
          <div class='featured-items'>
            <b:loop index='i' values='data:posts' var='post'>
              <b:include cond='data:i in [0]' data='post' name='content'/>
            </b:loop>
            <b:tag class='featured-grid' cond='data:posts.length gt 1' name='div'>
              <b:loop index='i' values='data:posts' var='post'>
                <b:include cond='data:i in [1,2]' data='post' name='content'/>
              </b:loop>
            </b:tag>
          </div>
          <b:else/>
          <div class='popular-items'>
            <b:loop index='i' values='data:posts' var='post'>
              <b:include cond='data:i in [0]' data='post' name='content'/>
            </b:loop>
            <b:tag class='popular-list' cond='data:posts.length gt 1' name='div'>
              <b:loop index='i' values='data:posts' var='post'>
                <b:include cond='data:i not in [0]' data='post' name='content'/>
              </b:loop>
            </b:tag>
          </div>
        </b:if>
      </div>
    </b:includable>
    <b:includable id='blogThisShare'/>
    <b:includable id='bylineByName' var='byline'/>
    <b:includable id='bylineRegion' var='regionItems'/>
    <b:includable id='commentsLink'/>
    <b:includable id='commentsLinkIframe'/>
    <b:includable id='content' var='post'>
      <b:include name='popular-content'/>
    </b:includable>
    <b:includable id='emailPostIcon'/>
    <b:includable id='facebookShare'/>
    <b:includable id='footerBylines'/>
    <b:includable id='googlePlusShare'/>
    <b:includable id='headerByline'/>
    <b:includable id='linkShare'/>
    <b:includable id='otherSharingButton'/>
    <b:includable id='platformShare'/>
    <b:includable id='postAuthor'/>
    <b:includable id='postCommentsLink'/>
    <b:includable id='postJumpLink' var='post'/>
    <b:includable id='postLabels'/>
    <b:includable id='postLocation'/>
    <b:includable id='postReactions'/>
    <b:includable id='postShareButtons'/>
    <b:includable id='postTimestamp'/>
    <b:includable id='sharingButton'/>
    <b:includable id='sharingButtonContent'/>
    <b:includable id='sharingButtons'/>
    <b:includable id='sharingButtonsMenu'/>
    <b:includable id='sharingPlatformIcon'/>
    <b:includable id='snippetedPostByline'/>
    <b:includable id='snippetedPostContent'/>
    <b:includable id='snippetedPostThumbnail'/>
    <b:includable id='snippetedPostTitle'/>
    <b:includable id='snippetedPosts'/>
  </b:defaultmarkup>
  <b:defaultmarkup type='FeaturedPost'>
    <b:includable id='main' var='this'>
      <b:include name='widget-title'/>
      <div class='widget-content'>
        <b:loop values='data:posts' var='post'>
          <b:include data='post' name='content'/>
        </b:loop>
      </div>
    </b:includable>
    <b:includable id='blogThisShare'/>
    <b:includable id='bylineByName' var='byline'/>
    <b:includable id='bylineRegion' var='regionItems'/>
    <b:includable id='commentsLink'/>
    <b:includable id='commentsLinkIframe'/>
    <b:includable id='content' var='post'>
      <b:include name='featured-content'/>
    </b:includable>
    <b:includable id='emailPostIcon'/>
    <b:includable id='facebookShare'/>
    <b:includable id='footerBylines'/>
    <b:includable id='googlePlusShare'/>
    <b:includable id='headerByline'/>
    <b:includable id='linkShare'/>
    <b:includable id='otherSharingButton'/>
    <b:includable id='platformShare'/>
    <b:includable id='postAuthor'/>
    <b:includable id='postCommentsLink'/>
    <b:includable id='postJumpLink' var='post'/>
    <b:includable id='postLabels'/>
    <b:includable id='postLocation'/>
    <b:includable id='postReactions'/>
    <b:includable id='postShareButtons'/>
    <b:includable id='postTimestamp'/>
    <b:includable id='sharingButton'/>
    <b:includable id='sharingButtonContent'/>
    <b:includable id='sharingButtons'/>
    <b:includable id='sharingButtonsMenu'/>
    <b:includable id='sharingPlatformIcon'/>
    <b:includable id='snippetedPostByline'/>
    <b:includable id='snippetedPostContent'/>
    <b:includable id='snippetedPostThumbnail'/>
    <b:includable id='snippetedPostTitle'/>
    <b:includable id='snippetedPosts'/>
  </b:defaultmarkup>
  <b:defaultmarkup type='ContactForm'>
    <b:includable id='main' var='this'>
      <b:include name='widget-title'/>
      <b:include name='content'/>
    </b:includable>
    <b:includable id='content'>
      <b:include name='contact-form-content'/>
    </b:includable>       
  </b:defaultmarkup>
  <b:defaultmarkup type='Label'>
    <b:includable id='main' var='this'>
      <b:include name='widget-title'/>
      <b:include name='content'/>
    </b:includable>
    <b:includable id='content'>
      <div class='widget-content'>
        <b:class expr:name='data:this.display + &quot;-label&quot;'/>
        <b:include cond='data:this.display == &quot;list&quot;' name='list'/>
        <b:include cond='data:this.display == &quot;cloud&quot;' name='cloud'/>
      </div>
    </b:includable>
    <b:includable id='list'>
      <ul class='list-style'>
        <b:loop values='data:labels' var='label'>
          <li><a class='label-name' expr:href='data:label.url'><data:label.name/><b:if cond='data:this.showFreqNumbers'><b:class name='has-count'/><span class='label-count count-style'>(<data:label.count/>)</span></b:if></a></li>
        </b:loop>
      </ul>
    </b:includable>
    <b:includable id='cloud'>
      <ul class='cloud-style'>
        <b:loop values='data:labels' var='label'>
          <li><a class='label-name btn' expr:href='data:label.url'><data:label.name/><b:if cond='data:this.showFreqNumbers'><b:class name='has-count'/><span class='label-count count-style'>(<data:label.count/>)</span></b:if></a></li>
        </b:loop>
      </ul>
    </b:includable>
  </b:defaultmarkup>
  <b:defaultmarkup type='FollowByEmail'>
    <b:includable id='main' var='this'>
      <b:include name='content'/>
    </b:includable>
    <b:includable id='content'>
      <div class='widget-content'>
		<p>This gadget is no longer available.</p>
      </div>
    </b:includable>
  </b:defaultmarkup> 
  <b:defaultmarkup type='Image'>
    <b:includable id='main' var='this'>
      <b:include name='widget-title'/>
      <b:include name='content'/>
    </b:includable>
    <b:includable id='content'>
      <b:include name='image-content'/>
    </b:includable>
  </b:defaultmarkup> 
  <b:defaultmarkup type='BlogArchive'>
    <b:includable id='main' var='this'>
      <b:include name='widget-title'/>
      <b:include name='content'/>
    </b:includable>
    <b:includable id='content'>
      <div class='widget-content'>
        <b:class name='archive-list'/>
        <b:include cond='data:this.style in {&quot;FLAT&quot;, &quot;MENU&quot;, &quot;HIERARCHY&quot;}' name='flat'/>
      </div>
    </b:includable>
    <b:includable id='flat'>
      <ul class='list-style'>
        <b:loop values='data:data' var='i'>
          <li><a class='archive-name' expr:href='data:i.url'><data:i.name/><b:if cond='data:i.post-count'><b:class name='has-count'/><span class='archive-count count-style'>(<data:i.post-count/>)</span></b:if></a></li>
        </b:loop>
      </ul>
    </b:includable>
  </b:defaultmarkup>
  <b:defaultmarkup type='PageList'>
    <b:includable id='main'>
      <b:include name='widget-title'/>
      <b:include name='content'/>
    </b:includable>
    <b:includable id='content'>
      <b:include name='pagelist-content'/>
    </b:includable>
    <b:includable id='overflowButton'/>
    <b:includable id='overflowablePageList'/>
    <b:includable id='pageLink'/>
    <b:includable id='pageList'/>
  </b:defaultmarkup>
  <b:defaultmarkup type='BlogSearch'>
    <b:includable id='main'>
      <b:include name='widget-title'/>
      <b:include name='content'/>
    </b:includable>
    <b:includable id='content'>
      <b:include name='searchForm'/>
    </b:includable>
    <b:includable id='searchForm'>
      <div class='search-form search-toggle'>
        <span class='search-input' expr:placeholder='data:messages.search'/>
      </div>
    </b:includable>
    <b:includable id='searchSubmit'/>
  </b:defaultmarkup>
  <b:defaultmarkup type='Profile'>
    <b:includable id='main' var='this'>
      <b:include name='widget-title'/>
      <b:include name='content'/>
    </b:includable>
    <b:includable id='authorProfileImage' var='this'>
      <img class='profile-img' expr:alt='data:messages.myPhoto' expr:src='resizeImage(data:authorPhoto.image, 50, &quot;1:1&quot;)'/>
    </b:includable>
    <b:includable id='defaultProfileImage' var='this'>
      <img class='profile-img' expr:alt='data:messages.myPhoto' src='https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEiCxxt0n6b048h4UEHf-L5T22U8xCk-IsG2qbfVUMBMKdt2t3ijO6qz--5UBg63qH4V_6z8uIBe7z6VNnueFbF3XKIWkCJPmFQqfm3Rmx3tpBOk74LGDZrUEgGnJF2-VDrzlkZSVyJs2sYjtiCytrEjsw23o88dqy5mdjw0KPwNuySVA7iYfdHWYpgsuQ/w50-h50-p-k-no-nu/avatar.webp'/>
    </b:includable>
    <b:includable id='userProfileInfo' var='this'>
      <div class='profile-info'>
        <dl class='profile-datablock'>
          <b:include name='userProfileData'/>
        </dl>
        <b:include name='viewProfileLink'/>
      </div>
    </b:includable>
    <b:includable id='teamProfileLink' var='this'>
      <b:include name='profileImage'/>
      <div class='profile-info'>
        <a class='profile-name' expr:href='data:userUrl' rel='noopener nofollow' target='_blank'><data:display-name/></a>
        <a class='profile-link' expr:href='data:userUrl' rel='noopener nofollow' target='_blank'><data:messages.showMore/></a>
      </div>
    </b:includable>
    <b:includable id='userProfile' var='this'>
      <b:include name='profileImage'/>
      <div class='profile-info'>
        <a class='profile-name' expr:href='data:userUrl' rel='noopener nofollow' target='_blank'><data:displayname/></a>
        <a class='profile-link' expr:href='data:userUrl' rel='noopener nofollow' target='_blank'><data:messages.showMore/></a>
      </div>
    </b:includable>
  </b:defaultmarkup>
  <b:defaultmarkup type='AdSense'>
    <b:includable id='main'>
      <b:include name='adsense-content'/>
    </b:includable>
  </b:defaultmarkup>
  <b:defaultmarkup type='Header'>
    <b:includable id='main' var='this'>
      <div class='widget-content'>
        <b:include name='title'/>
      </div>
    </b:includable>
    <b:includable id='behindImageStyle'/>
    <b:includable id='description'/>
    <b:includable id='image'/>
    <b:includable id='title'>
      <b:tag expr:href='data:blog.homepageUrl' name='a'><data:title/></b:tag>
    </b:includable>
  </b:defaultmarkup>
  <b:defaultmarkup type='Wikipedia'>
    <b:includable id='main'>
      <b:include name='widget-title'/>
      <b:include name='content'/>
    </b:includable>
    <b:includable id='content'>
      <div class='widget-content'>
        <form class='wikipedia-search-form' expr:id='data:widget.instanceId + &quot;_wikipedia-search-form&quot;' name='wikipedia'>
          <input class='wikipedia-search-input' expr:id='data:widget.instanceId + &quot;_wikipedia-search-input&quot;' expr:placeholder='data:messages.search' type='text'/>
          <input class='wikipedia-search-button btn' expr:value='data:messages.ok' type='submit'/>
        </form>
        <div class='wikipedia-search-results-wrap'>
          <div class='wikipedia-search-results-header' expr:id='data:widget.instanceId + &quot;_wikipedia-search-results-header&quot;'><data:searchResultsMsg/></div>
          <div class='wikipedia-search-results' expr:id='data:widget.instanceId + &quot;_wikipedia-search-results&quot;'/>
          <div class='wikipedia-search-more' expr:id='data:widget.instanceId + &quot;_wikipedia-search-more&quot;'/>
        </div>
      </div>
    </b:includable>
  </b:defaultmarkup>
</b:defaultmarkups>
<b:if cond='!data:isFeed'>
<!-- Miscellaneous -->
<b:include name='pbt-var'/>
<b:if cond='data:widgets.AdSense.first or data:blog.adsenseClientId'>
  <script async='async' crossorigin='anonymous' src='https://pagead2.googlesyndication.com/pagead/js/adsbygoogle.js'/>
</b:if>
<b:if cond='data:blog.analyticsAccountNumber'>
  <b:include cond='data:blog.analyticsAccountNumber' data='blog' name='google-analytics'/>
</b:if>
</b:if>
</head>
<body>
<b:include name='body-class'/>
<b:if cond='data:view.isLayoutMode or (data:widgets any w =&gt; w.sectionId == &quot;pbt-panel&quot;) and !data:isFeed'>
  <div id='theme-options' style='display:none'>
    <b:section class='pbt-panel' id='pbt-panel' maxwidgets='2' name='Theme Options' showaddelement='no'>
      <b:widget id='Image52' locked='true' title='Default Thumbnail' type='Image' visible='false'>
        <b:widget-settings>
          <b:widget-setting name='displayUrl'>https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEhG9GA0058_fE7q8dUjkpL56fvlwSQs-DyuNjRG1C3oYBoWDR2PYrDa0SKVYt6iEJ8pssbajfAujp0g51-SQimyZNawn0waVgbe8cwgMzSXRURuiG7bqguOahIkTzTgPOn67eoasTMjKkxPfqXg1ytQ4NMjLEAGpp3zKKtpo-PVacHSnidorgbmaOFlyQ/s800/ptb-nth.webp</b:widget-setting>
          <b:widget-setting name='displayHeight'>450</b:widget-setting>
          <b:widget-setting name='sectionWidth'>150</b:widget-setting>
          <b:widget-setting name='shrinkToFit'>false</b:widget-setting>
          <b:widget-setting name='displayWidth'>800</b:widget-setting>
          <b:widget-setting name='link'/>
          <b:widget-setting name='caption'/>
        </b:widget-settings>
        <b:includable id='main' var='this'>
      <b:include name='widget-title'/>
      <b:include name='content'/>
    </b:includable>
        <b:includable id='content'>
      <b:include name='image-content'/>
    </b:includable>
      </b:widget>
      <b:widget id='HTML50' locked='true' title='Translate' type='HTML' visible='false'>
        <b:widget-settings>
          <b:widget-setting name='content'/>
        </b:widget-settings>
        <b:includable id='main'>
      <b:include name='html-content'/>
    </b:includable>
      </b:widget>
    </b:section>
  </div>
</b:if>
<!-- Site Content -->
<div class='site-outer'>
  <b:if cond='!data:isFeed'>
    <header class='site-header'>
      <b:tag class='border-top' cond='data:skin.vars.border_top != &quot;0px&quot;' name='div'/>
      <div class='main-header'>
        <div class='header-inner'>
          <div class='header-header flex-c'>
            <div class='container row-x1'>
              <div class='header-items'>
                <div class='flex-left'>
                  <b:tag aria-label='Show Menu' class='mobile-menu-toggle' name='button'/>
                  <b:if cond='data:view.isLayoutMode or (data:widgets.Image any w =&gt; w.sectionId == &quot;main-logo&quot;)'>
                    <b:section class='main-logo' id='main-logo' maxwidgets='1' name='Header Logo' showaddelement='no'>
                      <b:widget id='Image50' locked='true' title='' type='Image' visible='true'>
                        <b:widget-settings>
                          <b:widget-setting name='displayUrl'>https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEiV6mVPBMMm_R_5TZl55lOW8ytafZbG7eZblVLVUfIN3h0bdYVcXMwuitQ9jqmZDp_HQtFuOqgfw8tiBRUVZ1SlUN7dWPWL7kDUmF_JTq_JXACLtQLzYxlbK3eFDMS9KSrXRySfR_7gmHGXlzFkfaVNRzRxHeycSVpbbUNG0xb3mZ7NU8ohTog3LQoXuw/s497/logo.webp</b:widget-setting>
                          <b:widget-setting name='displayHeight'>134</b:widget-setting>
                          <b:widget-setting name='sectionWidth'>148</b:widget-setting>
                          <b:widget-setting name='shrinkToFit'>false</b:widget-setting>
                          <b:widget-setting name='displayWidth'>497</b:widget-setting>
                          <b:widget-setting name='link'/>
                          <b:widget-setting name='caption'/>
                        </b:widget-settings>
                        <b:includable id='main' var='this'>
      <b:include name='widget-title'/>
      <b:include name='content'/>
    </b:includable>
                        <b:includable id='content'>
      <b:include name='image-content'/>
    </b:includable>
                      </b:widget>
                    </b:section>
                    <b:else/>
                    <div class='main-logo'>
                      <b:tag class='title' expr:name='data:view.isMultipleItems ? &quot;h1&quot; : &quot;span&quot;'>
                        <a class='homepage' expr:href='data:blog.homepageUrl.canonical' rel='home'><data:blog.title/></a>
                      </b:tag>
                    </div>
                  </b:if>
                  <b:section class='main-menu' id='main-menu' maxwidgets='1' name='Header Menu' showaddelement='no'>
                    <b:widget id='LinkList200' locked='true' title='' type='LinkList' visible='true'>
                      <b:widget-settings>
                        <b:widget-setting name='text-10'>_Error Page</b:widget-setting>
                        <b:widget-setting name='sorting'>NONE</b:widget-setting>
                        <b:widget-setting name='link-1'>#</b:widget-setting>
                        <b:widget-setting name='link-13'>#</b:widget-setting>
                        <b:widget-setting name='link-2'>#</b:widget-setting>
                        <b:widget-setting name='link-12'>#</b:widget-setting>
                        <b:widget-setting name='link-15'>#</b:widget-setting>
                        <b:widget-setting name='link-0'>/</b:widget-setting>
                        <b:widget-setting name='link-14'>#</b:widget-setting>
                        <b:widget-setting name='link-11'>#</b:widget-setting>
                        <b:widget-setting name='link-10'>#</b:widget-setting>
                        <b:widget-setting name='text-9'>_Download</b:widget-setting>
                        <b:widget-setting name='link-9'>#</b:widget-setting>
                        <b:widget-setting name='text-8'>_Post Split</b:widget-setting>
                        <b:widget-setting name='link-7'>#</b:widget-setting>
                        <b:widget-setting name='link-8'>#</b:widget-setting>
                        <b:widget-setting name='link-5'>#</b:widget-setting>
                        <b:widget-setting name='link-6'>#</b:widget-setting>
                        <b:widget-setting name='link-3'>#</b:widget-setting>
                        <b:widget-setting name='link-4'>#</b:widget-setting>
                        <b:widget-setting name='text-1'>Features</b:widget-setting>
                        <b:widget-setting name='text-0'>Home</b:widget-setting>
                        <b:widget-setting name='text-3'>_Post Layouts</b:widget-setting>
                        <b:widget-setting name='text-2'>_Featured Posts</b:widget-setting>
                        <b:widget-setting name='text-5'>__Full Width</b:widget-setting>
                        <b:widget-setting name='text-4'>__Left Sidebar</b:widget-setting>
                        <b:widget-setting name='text-7'>_Post Cards</b:widget-setting>
                        <b:widget-setting name='text-6'>__Right Sidebar</b:widget-setting>
                        <b:widget-setting name='text-15'>Shortcodes</b:widget-setting>
                        <b:widget-setting name='text-11'>_RTL Support</b:widget-setting>
                        <b:widget-setting name='text-12'>Trending</b:widget-setting>
                        <b:widget-setting name='text-13'>Categories</b:widget-setting>
                        <b:widget-setting name='text-14'>Tipography</b:widget-setting>
                      </b:widget-settings>
                      <b:includable id='main' var='this'>
      <b:include name='widget-title'/>
      <b:include name='content'/>
    </b:includable>
                      <b:includable id='content'>
      <b:include name='linklist-content'/>
    </b:includable>
                    </b:widget>
                  </b:section>
                </div>
                <div class='flex-right'>
                  <div class='toggle-wrap'>
                    <b:tag class='search-toggle' expr:aria-label='data:messages.search' name='button'/>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </header>
    <b:if cond='data:view.isLayoutMode or (data:view.isHomepage and (data:widgets any w =&gt; w.sectionId == &quot;featured&quot;))'>
      <section class='flex-c'>
        <b:section class='featured container row-x1' id='featured' maxwidgets='1' name='Featured Posts' showaddelement='yes'>
          <b:widget id='PopularPosts2' locked='false' title='Popular Posts' type='PopularPosts' visible='true'>
            <b:widget-settings>
              <b:widget-setting name='numItemsToShow'>3</b:widget-setting>
              <b:widget-setting name='showThumbnails'>true</b:widget-setting>
              <b:widget-setting name='showSnippets'>true</b:widget-setting>
              <b:widget-setting name='timeRange'>LAST_YEAR</b:widget-setting>
            </b:widget-settings>
            <b:includable id='main' var='this'>
      <b:include name='widget-title'/>
      <div class='widget-content'>
        <b:if cond='data:widget.sectionId == &quot;featured&quot;'>
          <div class='featured-items'>
            <b:loop index='i' values='data:posts' var='post'>
              <b:include cond='data:i in [0]' data='post' name='content'/>
            </b:loop>
            <b:tag class='featured-grid' cond='data:posts.length gt 1' name='div'>
              <b:loop index='i' values='data:posts' var='post'>
                <b:include cond='data:i in [1,2]' data='post' name='content'/>
              </b:loop>
            </b:tag>
          </div>
          <b:else/>
          <div class='popular-items'>
            <b:loop index='i' values='data:posts' var='post'>
              <b:include cond='data:i in [0]' data='post' name='content'/>
            </b:loop>
            <b:tag class='popular-list' cond='data:posts.length gt 1' name='div'>
              <b:loop index='i' values='data:posts' var='post'>
                <b:include cond='data:i not in [0]' data='post' name='content'/>
              </b:loop>
            </b:tag>
          </div>
        </b:if>
      </div>
    </b:includable>
            <b:includable id='blogThisShare'/>
            <b:includable id='bylineByName' var='byline'/>
            <b:includable id='bylineRegion' var='regionItems'/>
            <b:includable id='commentsLink'/>
            <b:includable id='commentsLinkIframe'/>
            <b:includable id='content' var='post'>
      <b:include name='popular-content'/>
    </b:includable>
            <b:includable id='emailPostIcon'/>
            <b:includable id='facebookShare'/>
            <b:includable id='footerBylines'/>
            <b:includable id='googlePlusShare'/>
            <b:includable id='headerByline'/>
            <b:includable id='linkShare'/>
            <b:includable id='otherSharingButton'/>
            <b:includable id='platformShare'/>
            <b:includable id='postAuthor'/>
            <b:includable id='postCommentsLink'/>
            <b:includable id='postJumpLink' var='post'/>
            <b:includable id='postLabels'/>
            <b:includable id='postLocation'/>
            <b:includable id='postReactions'/>
            <b:includable id='postShareButtons'/>
            <b:includable id='postTimestamp'/>
            <b:includable id='sharingButton'/>
            <b:includable id='sharingButtonContent'/>
            <b:includable id='sharingButtons'/>
            <b:includable id='sharingButtonsMenu'/>
            <b:includable id='sharingPlatformIcon'/>
            <b:includable id='snippetedPostByline'/>
            <b:includable id='snippetedPostContent'/>
            <b:includable id='snippetedPostThumbnail'/>
            <b:includable id='snippetedPostTitle'/>
            <b:includable id='snippetedPosts'/>
          </b:widget>
        </b:section>
      </section>
    </b:if>
  </b:if>
  <section class='content-wrap flex-c'>
    <div class='container row-x1 flex-sb'>
      <main class='main-wrap'>
        <b:section class='main' id='main' maxwidgets='1' name='Main Posts' showaddelement='yes'>
          <b:widget id='Blog1' locked='true' title='Blog Posts' type='Blog' visible='true'>
            <b:widget-settings>
              <b:widget-setting name='showDateHeader'>false</b:widget-setting>
              <b:widget-setting name='commentLabel'>$type={blogger}</b:widget-setting>
              <b:widget-setting name='style.textcolor'>#f8fafc</b:widget-setting>
              <b:widget-setting name='showShareButtons'>true</b:widget-setting>
              <b:widget-setting name='authorLabel'>by</b:widget-setting>
              <b:widget-setting name='showCommentLink'>true</b:widget-setting>
              <b:widget-setting name='style.urlcolor'>#ffffff</b:widget-setting>
              <b:widget-setting name='showAuthor'>true</b:widget-setting>
              <b:widget-setting name='style.linkcolor'>#f1f5f9</b:widget-setting>
              <b:widget-setting name='style.unittype'>TextAndImage</b:widget-setting>
              <b:widget-setting name='style.bgcolor'>#000000</b:widget-setting>
              <b:widget-setting name='timestampLabel'>-</b:widget-setting>
              <b:widget-setting name='reactionsLabel'/>
              <b:widget-setting name='showAuthorProfile'>true</b:widget-setting>
              <b:widget-setting name='style.layout'>1x1</b:widget-setting>
              <b:widget-setting name='showLabels'>true</b:widget-setting>
              <b:widget-setting name='showLocation'>false</b:widget-setting>
              <b:widget-setting name='postLabelsLabel'>Tags:</b:widget-setting>
              <b:widget-setting name='showTimestamp'>true</b:widget-setting>
              <b:widget-setting name='postsPerAd'>1</b:widget-setting>
              <b:widget-setting name='showBacklinks'>false</b:widget-setting>
              <b:widget-setting name='style.bordercolor'>#000000</b:widget-setting>
              <b:widget-setting name='showInlineAds'>false</b:widget-setting>
              <b:widget-setting name='showReactions'>false</b:widget-setting>
            </b:widget-settings>
            <b:includable id='main' var='this'>
      <b:class cond='data:view.isMultipleItems' name='index-blog flex-col'/>
      <b:if cond='!data:isFeed'>
        <b:include cond='data:view.isHomepage' name='blogPostsTitle'/>
        <b:include name='searchMessage'/>
        <b:if cond='!data:posts.empty'>
          <div class='blog-posts'>
            <b:class cond='data:view.isMultipleItems' expr:name='&quot;index-post-wrap&quot; + (data:skin.vars.gridStyle == &quot;1px&quot; ? &quot; grid-items&quot; : &quot; list-items&quot;)'/>
            <b:class cond='data:view.isSingleItem' name='item-post-wrap flex-col'/>
            <b:loop index='i' values='data:posts' var='post'>
              <b:include data='post' name='postCommentsAndAd'/>
            </b:loop>
          </div>
          <b:include cond='data:view.isMultipleItems' name='ajaxPagination'/>
        </b:if>
        <b:else/>
        <b:include name='pbt-feeds'/>
      </b:if>
    </b:includable>
            <b:includable id='aboutPostAuthor'/>
            <b:includable id='addComments'>
      <a expr:href='data:post.commentsUrl' expr:onclick='data:post.commentsUrlOnclick'><data:messages.postAComment/></a>
    </b:includable>
            <b:includable id='ajaxPagination'>
      <!-- Ajax Pagination -->
      <b:if cond='data:olderPageUrl'>
        <div class='blog-pager'>
          <a class='load-more btn visible' expr:data-url='data:olderPageUrl.canonical' href='#' id='load-more'><b:include data='{ message: &quot;loadMorePosts&quot; }' name='pbt-messages'/></a>
          <div class='loading'><div class='loader'><svg class='spinner' viewBox='0 0 50 50'><circle class='path' cx='25' cy='25' r='20'/></svg></div></div>
          <span class='no-more btn'><data:messages.noResultsFound/></span>
        </div>
      </b:if>
    </b:includable>
            <b:includable id='backLinks' var='post'/>
            <b:includable id='blogPostsTitle'>
      <b:if cond='data:blog.jumpLinkMessage != &quot;{hide}&quot;'>
        <div class='title-wrap blog1-title'><h3 class='title'><data:blog.jumpLinkMessage/></h3><a class='title-link' href='/search'><data:messages.viewAll/></a></div>
      </b:if>
    </b:includable>
            <b:includable id='blogThisShare'/>
            <b:includable id='bylineByName' var='byline'/>
            <b:includable id='bylineRegion' var='regionItems'/>
            <b:includable id='commentAuthorAvatar'/>
            <b:includable id='commentDeleteIcon' var='comment'/>
            <b:includable id='commentForm' var='post'>
      <div class='comment-form'>
        <a name='comment-form'/>
        <b:include data='post' name='commentFormIframeSrc'/>
        <iframe allowtransparency='allowtransparency' class='blogger-iframe-colorize blogger-comment-from-post' expr:height='data:cmtIframeInitialHeight ?: &quot;90px&quot;' frameborder='0' id='comment-editor' name='comment-editor' src='' width='100%'/>
        <data:post.cmtfpIframe/>
        <b:tag name='script' type='text/javascript'>
          BLOG_CMT_createIframe(&#39;<data:post.appRpcRelayPath/>&#39;);
        </b:tag>
      </div>
    </b:includable>
            <b:includable id='commentFormIframeSrc' var='post'>
      <a expr:href='data:post.commentFormIframeSrc params { skin: &quot;soho&quot; }' id='comment-editor-src' rel='nofollow noopener' title='Comment Form Link'/>
    </b:includable>
            <b:includable id='commentItem' var='comment'/>
            <b:includable id='commentList' var='comments'/>
            <b:includable id='commentPicker' var='post'/>
            <b:includable id='comments' var='post'>
      <a name='comments'/>
      <section class='comments threaded flex-col' expr:data-embed='data:post.embedCommentForm' expr:data-num-comments='data:post.numberOfComments' id='comments'>
        <b:class expr:name='data:post.numberOfComments != 0 ? &quot;has-comments&quot; : &quot;no-comments&quot;'/>
        <b:if cond='!data:post.allowNewComments'>
          <b:class name='no-comment-form'/>
        </b:if>
        <b:include name='commentsTitle'/>
        <b:if cond='data:post.allowNewComments'>
          <b:if cond='data:this.messages.blogComment'><p class='comments-message excerpt'><data:this.messages.blogComment/></p></b:if>
          <b:else/>
          <b:if cond='data:post.noNewCommentsText and (data:post.numberOfComments == 0)'><p class='comments-message excerpt'><data:post.noNewCommentsText/><em>*</em></p></b:if>
        </b:if>
        <b:if cond='data:post.embedCommentForm'>
          <b:if cond='data:post.numberOfComments != 0'>
            <div class='comments-content'>
              <div id='comment-holder'>
                <data:post.commentHtml/>
              </div>
            </div>
          </b:if>
          <b:if cond='data:post.allowNewComments'>
            <b:include data='post' name='commentForm'/>
          </b:if>
          <b:if cond='data:post.allowNewComments'><button class='show-cf btn' expr:aria-label='data:messages.postAComment'><data:messages.postAComment/><b:if cond='data:post.numberOfComments == 0'> (<data:post.numberOfComments/>)</b:if></button></b:if>
          <b:if cond='!data:post.allowNewComments'><b:if cond='data:post.noNewCommentsText and (data:post.numberOfComments != 0)'><p class='comments-message excerpt'><data:post.noNewCommentsText/><em>*</em></p></b:if></b:if>
          <b:else/>
          <p class='comments-message excerpt'>Please Select Embedded Mode To Show The Comment System.<em>*</em></p>
        </b:if>
      </section>
    </b:includable>
            <b:includable id='commentsTitle'>
      <!-- Comments Title -->
      <b:if cond='data:post.numberOfComments != 0'><div class='title-wrap comments-title'><b:class expr:name='data:this.messages.blogComment ? &quot;has-message&quot; : &quot;no-message&quot;'/><h3 class='title'><data:post.numberOfComments/> <data:messages.comments/></h3></div></b:if>
    </b:includable>
            <b:includable id='defaultAdUnit'>
      <ins class='adsbygoogle' data-ad-format='fluid' data-ad-layout-key='-g2-16+9a-5i-kj' data-full-width-responsive='false' expr:data-ad-client='data:adClientId ?: data:blog.adsenseClientId' expr:data-ad-host='data:blog.adsenseHostId' expr:data-analytics-uacct='data:blog.analyticsAccountNumber' style='display:block'/>
      <script>(adsbygoogle = window.adsbygoogle || []).push({});</script>
    </b:includable>
            <b:includable id='emailPostIcon'/>
            <b:includable id='facebookShare'/>
            <b:includable id='feedLinks'/>
            <b:includable id='feedLinksBody' var='links'/>
            <b:includable id='footerBylines'/>
            <b:includable id='googlePlusShare'/>
            <b:includable id='headerByline' var='post'>
      <!-- Post Entry Meta -->
      <b:if cond='data:view.isMultipleItems'>
        <b:if cond='data:allBylineItems.author or data:allBylineItems.timestamp'>
          <div class='entry-meta'>
            <b:include cond='data:allBylineItems.author' data='post' name='postAuthor'/>
            <b:include cond='data:allBylineItems.timestamp' data='post' name='postTimestamp'/>
          </div>
        </b:if>
      </b:if>
      <b:if cond='data:view.isPost'>
        <b:if cond='data:allBylineItems.author or data:allBylineItems.timestamp'>
          <b:class name='has-meta'/>
          <div class='entry-meta'>
            <div class='align-left'>
              <b:class cond='data:allBylineItems.timestamp' name='has-time'/>
              <b:if cond='data:allBylineItems.author'><span class='entry-avatar'><span class='avatar' expr:data-src='data:post.author.authorPhoto.image ? resizeImage(data:post.author.authorPhoto.image, 72, &quot;1:1&quot;) : &quot;https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEiCxxt0n6b048h4UEHf-L5T22U8xCk-IsG2qbfVUMBMKdt2t3ijO6qz--5UBg63qH4V_6z8uIBe7z6VNnueFbF3XKIWkCJPmFQqfm3Rmx3tpBOk74LGDZrUEgGnJF2-VDrzlkZSVyJs2sYjtiCytrEjsw23o88dqy5mdjw0KPwNuySVA7iYfdHWYpgsuQ/w72-h72-p-k-no-nu/avatar.webp&quot;'/></span></b:if>
              <b:tag class='al-items' cond='data:allBylineItems.author and data:allBylineItems.timestamp' name='div'>
              <b:include cond='data:allBylineItems.author' data='post' name='postAuthor'/>
              <b:include cond='data:allBylineItems.timestamp' data='post' name='postTimestamp'/>
              </b:tag>
            </div>
            <b:if cond='data:allBylineItems.share'>
              <div class='align-right'>
                <button class='share-toggle' expr:aria-label='data:messages.share'/>
              </div>
            </b:if>
          </div>
        </b:if>
      </b:if>
    </b:includable>
            <b:includable id='homePageLink'/>
            <b:includable id='iframeComments' var='post'/>
            <b:includable id='indexPost' var='post'>
      <!-- Index Post Content -->
      <b:include data='post' name='postFeaturedImage'/>
      <div class='entry-header'>
        <b:include data='post' name='postHeader'/>
        <b:include cond='(data:skin.vars.gridStyle != &quot;1px&quot;) and (data:skin.vars.postSummary == &quot;1px&quot;)' data='post' name='postBodySnippet'/>
        <b:include data='post' name='headerByline'/>
      </div>
    </b:includable>
            <b:includable id='inlineAd' var='post'/>
            <b:includable id='itemPost' var='post'>
      <!-- Item Post Content -->
      <b:include cond='data:view.isPost' data='post' name='itemPostData'/>
      <div class='item-post-inner flex-col'>
        <div class='entry-header post-header'>
          <b:include data='post' name='postHeader'/>
        </div>
        <div class='entry-content-wrap flex-col'>
          <b:include data='post' name='postBody'/>
        </div>
        <b:include cond='data:view.isPost and data:allBylineItems.labels' data='post' name='postLabels'/>
        <b:include cond='data:view.isPost and data:allBylineItems.share' data='post' name='postShareButtons'/>
      </div>
    </b:includable>
            <b:includable id='itemPostData' var='post'>
      <b:tag id='data' name='script' type='application/json'>{&quot;postData&quot;:[{&quot;published&quot;:{&quot;date&quot;:&quot;<data:post.date.jsonEscaped/>&quot;,&quot;datetime&quot;:&quot;<data:post.date.iso8601.jsonEscaped/>&quot;},&quot;author&quot;:&quot;<data:post.author.name.jsonEscaped/>&quot;,<b:if cond='data:post.labels'>&quot;category&quot;:&quot;<data:post.labels.first.name/>&quot;,</b:if>&quot;title&quot;:&quot;<b:eval expr='data:post.title ? data:post.title.jsonEscaped : data:messages.noTitle.jsonEscaped'/>&quot;,&quot;link&quot;:&quot;<data:post.url.canonical.jsonEscaped/>&quot;,&quot;thumbnail&quot;:{&quot;src&quot;:&quot;<b:if cond='data:post.featuredImage'><b:eval expr='data:post.featuredImage.isYouTube ? resizeImage(data:post.featuredImage.youtubeMaxResDefaultUrl.jsonEscaped, 72, &quot;1:1&quot;) : resizeImage(data:post.featuredImage.jsonEscaped, 72, &quot;1:1&quot;)'/><b:else/>https://resources.blogblog.com/img/blank.gif</b:if>&quot;,&quot;source&quot;:&quot;<b:eval expr='data:post.featuredImage.isYouTube ? &quot;youtube&quot; : &quot;blogger&quot;'/>&quot;}}]}</b:tag>
    </b:includable>
            <b:includable id='linkShare'/>
            <b:includable id='nextPageLink'>
      <b:if cond='data:olderPageUrl'>
        <a class='post-nav-link post-nav-older-link' expr:href='data:olderPageUrl.canonical'>
          <b:include data='{ message: &quot;nextPost&quot; }' name='pbt-messages'/>
        </a>
        <b:else/>
        <span class='post-nav-link post-nav-older-link'>
          <b:include data='{ message: &quot;nextPost&quot; }' name='pbt-messages'/>
        </span>
      </b:if>
    </b:includable>
            <b:includable id='otherSharingButton'/>
            <b:includable id='platformShare'/>
            <b:includable id='post' var='post'>
      <!-- Index Posts -->
      <b:if cond='data:view.isMultipleItems'>
        <b:include data='post' name='indexPost'/>
      </b:if>
      <!-- Item Post -->
      <b:if cond='data:view.isSingleItem'>
        <b:include data='post' name='itemPost'/>
      </b:if>
    </b:includable>
            <b:includable id='postAuthor' var='post'>
      <!-- Post Author -->
      <span class='entry-author'><b:if cond='data:allBylineItems.author.label and data:view.isPost'><span class='by sp'><data:allBylineItems.author.label/></span></b:if><span class='author-name'><data:post.author.name/></span></span>
    </b:includable>
            <b:includable id='postBody' var='post'> 
      <!-- Post Body Entry Content -->
      <div class='post-body entry-content' id='post-body'>
        <data:post.body/>
      </div>
    </b:includable>
            <b:includable id='postBodySnippet' var='post'><p class='entry-excerpt excerpt'><b:eval expr='data:post.snippets.long snippet { length: 65 }'/></p></b:includable>
            <b:includable id='postBreadcrumbs' var='post'>
      <!-- Post Breadcrumbs -->
      <nav id='breadcrumb'><a class='home' expr:href='data:blog.homepageUrl.canonical'><data:messages.home/></a><b:if cond='data:post.labels'><i class='sep'/><a class='label' expr:href='data:post.labels.first.url.canonical'><data:post.labels.first.name/></a></b:if></nav>
    </b:includable>
            <b:includable id='postCategory' var='post'>
      <!-- Post Category -->
      <b:include name='post-category'/>
    </b:includable>
            <b:includable id='postCommentsAndAd' var='post'>
      <b:include data='post' name='postMeta'/>
      <article>
        <b:class cond='data:view.isMultipleItems' expr:name='&quot;post hentry item-&quot; + data:i'/>
        <b:class cond='data:view.isSingleItem' name='item-post hentry'/>
        <b:include data='post' name='post'/>
      </article>
      <b:include cond='data:view.isPost' data='post' name='postFooter'/>
      <b:if cond='data:view.isSingleItem and data:post.allowComments'>
        <!-- Post Comments -->
        <div class='blog-post-comments p-widget' expr:data-shortcode='data:allBylineItems.comments.label contains &quot;type&quot; ? data:allBylineItems.comments.label : &quot;$type={blogger}&quot;'>
          <b:include data='post' name='comments'/>
        </div>
      </b:if>
      <!-- Post Navigation -->
      <b:include cond='data:skin.vars.postnav == &quot;1px&quot;' name='postPagination'/>
    </b:includable>
            <b:includable id='postCommentsLink'/>
            <b:includable id='postFeaturedImage' var='post'>
      <!-- Post Featured Image -->
      <a expr:class='data:post.featuredImage.isYouTube ? &quot;entry-thumbnail yt-img&quot; : &quot;entry-thumbnail&quot;' expr:href='data:post.url.canonical' expr:title='data:post.title ? data:post.title : data:messages.noTitle'><span class='thumbnail' expr:data-src='data:post.featuredImage ? (data:post.featuredImage.isYouTube ? resizeImage(data:post.featuredImage.youtubeMaxResDefaultUrl.jsonEscaped, 72, &quot;1:1&quot;) : resizeImage(data:post.featuredImage, 72, &quot;1:1&quot;)) : &quot;https://resources.blogblog.com/img/blank.gif&quot;'/><b:include data='post' name='postCategory'/></a>
    </b:includable>
            <b:includable id='postFooter' var='post'>
      <!-- Post Footer Items -->
      <div class='post-footer flex-col'>
        <b:include cond='data:post.author.aboutMe' data='post' name='postFooterAuthorProfile'/>
        <b:include cond='data:widgets.HTML any w =&gt; w.sectionId == &quot;related-posts&quot;' data='post' name='relatedPosts'/>
      </div>
    </b:includable>
            <b:includable id='postFooterAuthorProfile' var='post'>
      <div class='about-author p-widget'>
        <div class='author-avatar entry-avatar'>
          <span class='avatar' expr:data-src='data:post.author.authorPhoto.image ? resizeImage(data:post.author.authorPhoto.image, 72, &quot;1:1&quot;) : &quot;https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEiCxxt0n6b048h4UEHf-L5T22U8xCk-IsG2qbfVUMBMKdt2t3ijO6qz--5UBg63qH4V_6z8uIBe7z6VNnueFbF3XKIWkCJPmFQqfm3Rmx3tpBOk74LGDZrUEgGnJF2-VDrzlkZSVyJs2sYjtiCytrEjsw23o88dqy5mdjw0KPwNuySVA7iYfdHWYpgsuQ/w72-h72-p-k-no-nu/avatar.webp&quot;'/>
        </div>
        <div class='author-description flex-col'>
          <h3 class='author-title'><data:post.author.name/><b:attr cond='data:post.author.profileUrl' expr:value='data:post.author.profileUrl' name='profile-url'/></h3>
          <p class='author-text excerpt'><data:post.author.aboutMe/></p>
        </div>
      </div>
    </b:includable>
            <b:includable id='postHeader' var='post'>
      <b:include cond='data:view.isPost and (data:skin.vars.breadcrumb == &quot;1px&quot;)' data='post' name='postBreadcrumbs'/>
      <b:include data='post' name='postTitle'/>
      <b:include cond='data:view.isPost' data='post' name='headerByline'/>
    </b:includable>
            <b:includable id='postJumpLink' var='post'>
      <b:if cond='data:blog.jumpLinkMessage != &quot;hide&quot;'>
        <a class='read-more' expr:href='data:post.url.canonical'><data:blog.jumpLinkMessage/></a>
      </b:if>
    </b:includable>
            <b:includable id='postLabels' var='post'>
      <b:if cond='data:post.labels'>
        <div class='entry-labels'>
          <b:if cond='data:allBylineItems.labels.label'><span class='labels-label btn'><data:allBylineItems.labels.label/></span></b:if>
          <b:loop values='data:post.labels' var='label'>
            <a class='label-link btn' expr:href='data:label.url.canonical' rel='tag'><data:label.name/></a>
          </b:loop>
        </div>
      </b:if>
    </b:includable>
            <b:includable id='postLocation'/>
            <b:includable id='postMeta' var='post'>
      <b:if cond='data:view.isPost'>
        <b:tag name='script' type='application/ld+json'>{&quot;@context&quot;:&quot;https://schema.org&quot;,&quot;@graph&quot;:[{&quot;@type&quot;:&quot;NewsArticle&quot;,&quot;mainEntityOfPage&quot;:{&quot;@type&quot;:&quot;WebPage&quot;,&quot;@id&quot;:&quot;<data:post.url.canonical.jsonEscaped/>&quot;},&quot;headline&quot;:&quot;<data:post.title.jsonEscaped/>&quot;,&quot;description&quot;:&quot;<data:post.snippets.short.jsonEscaped/>&quot;,&quot;datePublished&quot;:&quot;<data:post.date.iso8601.jsonEscaped/>&quot;,&quot;dateModified&quot;:&quot;<data:post.lastUpdated.iso8601.jsonEscaped/>&quot;,&quot;image&quot;:{&quot;@type&quot;:&quot;ImageObject&quot;,<b:if cond='data:post.featuredImage.isResizable'>&quot;url&quot;:&quot;<b:eval expr='resizeImage(data:post.featuredImage, 1200, &quot;1200:675&quot;)'/>&quot;,&quot;height&quot;:675,&quot;width&quot;:1200<b:else/>&quot;url&quot;:&quot;https://lh3.googleusercontent.com/ULB6iBuCeTVvSjjjU1A-O8e9ZpVba6uvyhtiWRti_rBAs9yMYOFBujxriJRZ-A=w1200&quot;,&quot;height&quot;:348,&quot;width&quot;:1200</b:if>},&quot;author&quot;:{&quot;@type&quot;:&quot;Person&quot;,&quot;name&quot;:&quot;<data:post.author.name.jsonEscaped/>&quot;<b:if cond='data:post.author.profileUrl'>,&quot;url&quot;:&quot;<data:post.author.profileUrl.jsonEscaped/>&quot;</b:if>},&quot;publisher&quot;:{&quot;@type&quot;:&quot;Organization&quot;,&quot;name&quot;:&quot;Blogger&quot;,&quot;logo&quot;:{&quot;@type&quot;:&quot;ImageObject&quot;,&quot;url&quot;:&quot;https://lh3.googleusercontent.com/ULB6iBuCeTVvSjjjU1A-O8e9ZpVba6uvyhtiWRti_rBAs9yMYOFBujxriJRZ-A=h60&quot;,&quot;width&quot;:206,&quot;height&quot;:60}}},{&quot;@type&quot;:&quot;BreadcrumbList&quot;,&quot;itemListElement&quot;:[{&quot;@type&quot;:&quot;ListItem&quot;,&quot;position&quot;:1,&quot;name&quot;:&quot;<data:messages.home.jsonEscaped/>&quot;,&quot;item&quot;:&quot;<data:blog.homepageUrl.canonical.jsonEscaped/>&quot;},{&quot;@type&quot;:&quot;ListItem&quot;,&quot;position&quot;:2,&quot;name&quot;:&quot;<b:if cond='data:post.labels'><data:post.labels.first.name.jsonEscaped/><b:else/><data:messages.posts/></b:if>&quot;,&quot;item&quot;:&quot;<b:if cond='data:post.labels'><data:post.labels.first.url.canonical.jsonEscaped/><b:else/><b:eval expr='data:blog.homepageUrl.canonical.jsonEscaped + &quot;search/&quot;'/></b:if>&quot;},{&quot;@type&quot;:&quot;ListItem&quot;,&quot;position&quot;:3,&quot;name&quot;:&quot;<data:post.title.jsonEscaped/>&quot;,&quot;item&quot;:&quot;<data:post.url.canonical.jsonEscaped/>&quot;}]}]}</b:tag>
      </b:if>
      <b:if cond='data:view.isPage'>
        <b:tag name='script' type='application/ld+json'>{&quot;@context&quot;:&quot;http://schema.org&quot;,&quot;@type&quot;:&quot;BreadcrumbList&quot;,&quot;itemListElement&quot;:[{&quot;@type&quot;:&quot;ListItem&quot;,&quot;position&quot;:1,&quot;name&quot;:&quot;<data:messages.home.jsonEscaped/>&quot;,&quot;item&quot;:&quot;<data:blog.homepageUrl.canonical.jsonEscaped/>&quot;},{&quot;@type&quot;:&quot;ListItem&quot;,&quot;position&quot;:2,&quot;name&quot;:&quot;<data:post.title.jsonEscaped/>&quot;,&quot;item&quot;:&quot;<data:post.url.canonical.jsonEscaped/>&quot;}]}</b:tag>
      </b:if>
    </b:includable>
            <b:includable id='postMetadataJSONImage'/>
            <b:includable id='postMetadataJSONPublisher'/>
            <b:includable id='postPagination'>
      <b:if cond='data:view.isPost'>
        <div class='post-nav p-widget'>
          <b:include name='previousPageLink'/>
          <b:include name='nextPageLink'/>
        </div>
      </b:if>
    </b:includable>
            <b:includable id='postReactions'/>
            <b:includable id='postShareButtons' var='post'>
      <!-- Post Share Buttons -->
      <div class='post-share'>
        <ul class='share-a social color'>
          <li class='share-label'><span class='sl-btn btn'><i class='sl-ico'/></span></li>
          <li class='facebook has-span'><a class='bi-facebook btn pbt-wo' expr:href='&quot;https://www.facebook.com/sharer.php?u=&quot; + data:post.url.canonical' rel='nofollow noopener' title='Facebook'><span>Facebook</span></a></li>
          <li class='twitter has-span'><a class='bi-twitter btn pbt-wo' expr:href='&quot;https://twitter.com/intent/tweet?url=&quot; + data:post.url.canonical' rel='nofollow noopener' title='Twitter'><span>Twitter</span></a></li>
          <li class='whatsapp'><a class='bi-whatsapp btn pbt-wo' expr:href='&quot;https://api.whatsapp.com/send?text=&quot; + data:post.title.jsonEscaped + &quot; | &quot; + data:post.url.canonical' rel='nofollow noopener' title='WhatsApp'/></li>
          <li class='email'><a class='bi-email btn pbt-wo' expr:href='&quot;mailto:?subject=&quot; + data:post.title.jsonEscaped + &quot;&amp;body=&quot; + data:post.url.canonical' rel='nofollow noopener' title='Email'/></li>
          <li class='show-more'><button class='btn' expr:aria-label='data:messages.showMore'/></li>
        </ul>
      </div>
    </b:includable>
            <b:includable id='postTimestamp' var='post'>
      <!-- Post Timestamp -->
      <span class='entry-time'><b:if cond='data:allBylineItems.author and data:allBylineItems.timestamp.label'><span class='sp'><data:allBylineItems.timestamp.label/></span></b:if><time class='published' expr:datetime='data:post.date.iso8601'><data:post.date/></time></span>
    </b:includable>
            <b:includable id='postTitle' var='post'>
      <!-- Post Title Index and Item -->
      <b:if cond='data:view.isMultipleItems'>
        <h2 class='entry-title'><a expr:href='data:post.url.canonical' rel='bookmark'><b:eval expr='data:post.title ? data:post.title : data:messages.noTitle'/></a></h2>
      </b:if>
      <b:if cond='data:view.isSingleItem'>
        <h1 class='entry-title'><b:eval expr='data:post.title ? data:post.title : data:messages.noTitle'/></h1>
      </b:if>
    </b:includable>
            <b:includable id='previousPageLink'>
      <b:if cond='data:newerPageUrl'>
        <a class='post-nav-link post-nav-newer-link' expr:href='data:newerPageUrl.canonical'>
          <b:include data='{ message: &quot;prevPost&quot; }' name='pbt-messages'/>
        </a>
        <b:else/>
        <span class='post-nav-link post-nav-newer-link'>
          <b:include data='{ message: &quot;prevPost&quot; }' name='pbt-messages'/>
        </span>
      </b:if>
    </b:includable>
            <b:includable id='relatedPosts' var='post'>
      <!-- Related Posts -->
      <div class='related-wrap p-widget'>
        <div class='title-wrap related-title'>
          <b:with value='data:widgets.HTML filter (w =&gt; w.sectionId == &quot;related-posts&quot;) map (w =&gt; w.title)' var='pbtTitle'>
            <h3 class='title'><b:eval expr='data:pbtTitle.first ? data:pbtTitle.first : data:messages.youMayLikeThesePosts'/></h3>
            <a class='title-link' expr:href='data:post.labels ? &quot;/search/label/&quot; + data:post.labels.first.name : &quot;/search&quot;'><data:messages.viewAll/></a>
          </b:with>
        </div>
        <div class='widget-content'>
          <span class='related-tag' expr:data-id='data:post.id' expr:data-label='data:post.labels ? data:post.labels.first.name : &quot;recent&quot;'/>
        </div> 
      </div>  
    </b:includable>
            <b:includable id='searchMessage'>
      <!-- Search Message -->
      <b:if cond='data:posts.empty'>
        <b:class name='no-posts'/>
      </b:if>
      <b:if cond='data:view.search.query'>
        <div class='queryMessage'>
          <b:if cond='data:posts.empty'>
            <span class='query-info query-error'>&quot;<data:view.search.query/>&quot;</span>
            <b:else/>
            <span class='query-info query-success'>&quot;<data:view.search.query/>&quot;</span>
          </b:if>
        </div>
      </b:if>
      <b:if cond='data:view.search.label'>
        <div class='queryMessage '>
          <b:if cond='data:posts.empty'>
            <span class='query-info query-label query-error'><data:view.search.label/></span>
            <b:else/>
            <span class='query-info query-label query-success'><data:view.search.label/></span>
          </b:if>
        </div>
      </b:if>
      <b:if cond='data:view.isArchive'>
        <div class='queryMessage'>
          <b:if cond='data:posts.empty'>
            <span class='query-info query-error'><data:view.archive.rangeMessage/></span>
            <b:else/>
            <span class='query-info query-success'><data:view.archive.rangeMessage/></span>
          </b:if>
        </div>
      </b:if>
      <b:if cond='data:view.isError'>
        <div class='errorWrap'>
          <h3>404</h3>
          <h4><data:messages.theresNothingHere/></h4>
          <p><data:navMessage/></p>
          <a class='homepage btn' expr:href='data:blog.homepageUrl'><data:messages.home/></a>
        </div>
      </b:if>
      <b:if cond='data:view.isMultipleItems and data:posts.empty'><div class='queryEmpty'><data:messages.noResultsFound/></div></b:if>
    </b:includable>
            <b:includable id='sharingButton'/>
            <b:includable id='sharingButtonContent'/>
            <b:includable id='sharingButtons'/>
            <b:includable id='sharingButtonsMenu'/>
            <b:includable id='sharingPlatformIcon'/>
            <b:includable id='threadedCommentForm' var='post'/>
            <b:includable id='threadedCommentJs' var='post'/>
            <b:includable id='threadedComments' var='post'/>
            <b:includable id='threadedCommentsDisqus' var='post'/>
          </b:widget>
        </b:section>
        <b:section cond='data:view.isPost and (data:widgets.HTML any w =&gt; w.sectionId == &quot;related-posts&quot;)' id='related-posts' maxwidgets='1' name='Related Posts' showaddelement='yes'>
          <b:widget id='HTML51' locked='true' title='You might like' type='HTML' visible='true'>
            <b:widget-settings>
              <b:widget-setting name='content'>$results={3}</b:widget-setting>
            </b:widget-settings>
            <b:includable id='main'>
      <b:include name='html-content'/>
    </b:includable>
          </b:widget>
        </b:section>
      </main>
      <b:if cond='!data:isFeed'>
        <aside class='sidebar-wrap'>
          <b:section class='sidebar pbt-s' cond='!data:view.isError' id='sidebar' name='Sidebar' showaddelement='yes'>
            <b:widget id='LinkList1' locked='false' title='Follow Us' type='LinkList' visible='true'>
              <b:widget-settings>
                <b:widget-setting name='link-3'>https://www.youtube.com/probloggertemplates?sub_confirmation=1#65.4k</b:widget-setting>
                <b:widget-setting name='sorting'>NONE</b:widget-setting>
                <b:widget-setting name='link-4'>https://instagram.com/probloggertemplates#23.9k</b:widget-setting>
                <b:widget-setting name='text-1'>facebook</b:widget-setting>
                <b:widget-setting name='link-1'>https://www.facebook.com/probloggertemplates#25.7k</b:widget-setting>
                <b:widget-setting name='text-0'>{getSocial}</b:widget-setting>
                <b:widget-setting name='link-2'>https://twitter.com/probtemplates#39.3k</b:widget-setting>
                <b:widget-setting name='text-3'>youtube</b:widget-setting>
                <b:widget-setting name='link-0'>#</b:widget-setting>
                <b:widget-setting name='text-2'>twitter</b:widget-setting>
                <b:widget-setting name='text-4'>instagram</b:widget-setting>
              </b:widget-settings>
              <b:includable id='main' var='this'>
      <b:include name='widget-title'/>
      <b:include name='content'/>
    </b:includable>
              <b:includable id='content'>
      <b:include name='linklist-content'/>
    </b:includable>
            </b:widget>
            <b:widget id='PopularPosts1' locked='false' title='Popular Articles' type='PopularPosts' visible='true'>
              <b:widget-settings>
                <b:widget-setting name='numItemsToShow'>4</b:widget-setting>
                <b:widget-setting name='showThumbnails'>true</b:widget-setting>
                <b:widget-setting name='showSnippets'>true</b:widget-setting>
                <b:widget-setting name='timeRange'>LAST_YEAR</b:widget-setting>
              </b:widget-settings>
              <b:includable id='main' var='this'>
      <b:include name='widget-title'/>
      <div class='widget-content'>
        <b:if cond='data:widget.sectionId == &quot;featured&quot;'>
          <div class='featured-items'>
            <b:loop index='i' values='data:posts' var='post'>
              <b:include cond='data:i in [0]' data='post' name='content'/>
            </b:loop>
            <b:tag class='featured-grid' cond='data:posts.length gt 1' name='div'>
              <b:loop index='i' values='data:posts' var='post'>
                <b:include cond='data:i in [1,2]' data='post' name='content'/>
              </b:loop>
            </b:tag>
          </div>
          <b:else/>
          <div class='popular-items'>
            <b:loop index='i' values='data:posts' var='post'>
              <b:include cond='data:i in [0]' data='post' name='content'/>
            </b:loop>
            <b:tag class='popular-list' cond='data:posts.length gt 1' name='div'>
              <b:loop index='i' values='data:posts' var='post'>
                <b:include cond='data:i not in [0]' data='post' name='content'/>
              </b:loop>
            </b:tag>
          </div>
        </b:if>
      </div>
    </b:includable>
              <b:includable id='blogThisShare'/>
              <b:includable id='bylineByName' var='byline'/>
              <b:includable id='bylineRegion' var='regionItems'/>
              <b:includable id='commentsLink'/>
              <b:includable id='commentsLinkIframe'/>
              <b:includable id='content' var='post'>
      <b:include name='popular-content'/>
    </b:includable>
              <b:includable id='emailPostIcon'/>
              <b:includable id='facebookShare'/>
              <b:includable id='footerBylines'/>
              <b:includable id='googlePlusShare'/>
              <b:includable id='headerByline'/>
              <b:includable id='linkShare'/>
              <b:includable id='otherSharingButton'/>
              <b:includable id='platformShare'/>
              <b:includable id='postAuthor'/>
              <b:includable id='postCommentsLink'/>
              <b:includable id='postJumpLink' var='post'/>
              <b:includable id='postLabels'/>
              <b:includable id='postLocation'/>
              <b:includable id='postReactions'/>
              <b:includable id='postShareButtons'/>
              <b:includable id='postTimestamp'/>
              <b:includable id='sharingButton'/>
              <b:includable id='sharingButtonContent'/>
              <b:includable id='sharingButtons'/>
              <b:includable id='sharingButtonsMenu'/>
              <b:includable id='sharingPlatformIcon'/>
              <b:includable id='snippetedPostByline'/>
              <b:includable id='snippetedPostContent'/>
              <b:includable id='snippetedPostThumbnail'/>
              <b:includable id='snippetedPostTitle'/>
              <b:includable id='snippetedPosts'/>
            </b:widget>
            <b:widget id='HTML6' locked='false' title='{getMailchimp} $title={Stay Informed} $text={Subscribe to our mailing list to get the new updates.}' type='HTML' visible='true'>
              <b:widget-settings>
                <b:widget-setting name='content'><![CDATA[https://probloggertemplates.us6.list-manage.com/subscribe?u=98155398e3195ed8f58e2b86c&id=64e8605563]]></b:widget-setting>
              </b:widget-settings>
              <b:includable id='main'>
      <b:include name='html-content'/>
    </b:includable>
            </b:widget>
            <b:widget id='Label1' locked='false' title='Main Tags' type='Label' visible='true'>
              <b:widget-settings>
                <b:widget-setting name='sorting'>ALPHA</b:widget-setting>
                <b:widget-setting name='display'>CLOUD</b:widget-setting>
                <b:widget-setting name='selectedLabelsList'/>
                <b:widget-setting name='showType'>ALL</b:widget-setting>
                <b:widget-setting name='showFreqNumbers'>false</b:widget-setting>
              </b:widget-settings>
              <b:includable id='main' var='this'>
      <b:include name='widget-title'/>
      <b:include name='content'/>
    </b:includable>
              <b:includable id='cloud'>
      <ul class='cloud-style'>
        <b:loop values='data:labels' var='label'>
          <li><a class='label-name btn' expr:href='data:label.url'><data:label.name/><b:if cond='data:this.showFreqNumbers'><b:class name='has-count'/><span class='label-count count-style'>(<data:label.count/>)</span></b:if></a></li>
        </b:loop>
      </ul>
    </b:includable>
              <b:includable id='content'>
      <div class='widget-content'>
        <b:class expr:name='data:this.display + &quot;-label&quot;'/>
        <b:include cond='data:this.display == &quot;list&quot;' name='list'/>
        <b:include cond='data:this.display == &quot;cloud&quot;' name='cloud'/>
      </div>
    </b:includable>
              <b:includable id='list'>
      <ul class='list-style'>
        <b:loop values='data:labels' var='label'>
          <li><a class='label-name' expr:href='data:label.url'><data:label.name/><b:if cond='data:this.showFreqNumbers'><b:class name='has-count'/><span class='label-count count-style'>(<data:label.count/>)</span></b:if></a></li>
        </b:loop>
      </ul>
    </b:includable>
            </b:widget>
          </b:section>
        </aside>
      </b:if>
    </div>
  </section>
  <b:if cond='!data:isFeed'>
    <footer class='site-footer'>
      <b:if cond='data:view.isLayoutMode or (data:widgets.Image any w =&gt; w.sectionId == &quot;about&quot;)'>
        <div class='footer flex-c'>
          <div class='container row-x1'>
            <b:section class='about-section flex-sb' id='about' maxwidgets='2' name='About Section' showaddelement='yes'>
              <b:widget id='Image51' locked='true' title='About Us' type='Image' visible='true'>
                <b:widget-settings>
                  <b:widget-setting name='displayUrl'>https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEjuknG77iGav6ZDMKsk2llf3KaP60zDA62f9Z-Mtv5aWg0bOzOCc8kEs9-884U5Xt3hTeSFL5rExUnX6GlId9yk-uyL3vIQQOsAIDscL6tEqFY3vKKSQ6rOWHqcdjpfQztH5WBJl1EZKE11WzY1kH1g5S38Sm0cIkfV0z8HO2HVvQsXEJuwg_p5EAw4ng/s497/dark-logo.webp</b:widget-setting>
                  <b:widget-setting name='displayHeight'>134</b:widget-setting>
                  <b:widget-setting name='sectionWidth'>150</b:widget-setting>
                  <b:widget-setting name='shrinkToFit'>false</b:widget-setting>
                  <b:widget-setting name='displayWidth'>497</b:widget-setting>
                  <b:widget-setting name='link'/>
                  <b:widget-setting name='caption'><![CDATA[Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's.]]></b:widget-setting>
                </b:widget-settings>
                <b:includable id='main' var='this'>
      <b:include name='widget-title'/>
      <b:include name='content'/>
    </b:includable>
                <b:includable id='content'>
      <b:include name='image-content'/>
    </b:includable>
              </b:widget>
              <b:widget id='LinkList203' locked='true' title='Follow Us' type='LinkList' visible='true'>
                <b:widget-settings>
                  <b:widget-setting name='link-5'>https://probloggertemplates.com/</b:widget-setting>
                  <b:widget-setting name='link-3'>https://www.youtube.com/probloggertemplates?sub_confirmation=1</b:widget-setting>
                  <b:widget-setting name='link-4'>https://instagram.com/probloggertemplates</b:widget-setting>
                  <b:widget-setting name='text-1'>facebook</b:widget-setting>
                  <b:widget-setting name='text-0'>{getSocial}</b:widget-setting>
                  <b:widget-setting name='text-3'>youtube</b:widget-setting>
                  <b:widget-setting name='text-2'>twitter</b:widget-setting>
                  <b:widget-setting name='text-5'>rss</b:widget-setting>
                  <b:widget-setting name='text-4'>instagram</b:widget-setting>
                  <b:widget-setting name='sorting'>NONE</b:widget-setting>
                  <b:widget-setting name='link-1'>https://www.facebook.com/probloggertemplates</b:widget-setting>
                  <b:widget-setting name='link-2'>https://twitter.com/probtemplates</b:widget-setting>
                  <b:widget-setting name='link-0'>#</b:widget-setting>
                </b:widget-settings>
                <b:includable id='main' var='this'>
      <b:include name='widget-title'/>
      <b:include name='content'/>
    </b:includable>
                <b:includable id='content'>
      <b:include name='linklist-content'/>
    </b:includable>
              </b:widget>
            </b:section>
          </div>
        </div>
      </b:if>
      <div class='footer-bar flex-c'>
        <b:class cond='data:widgets.Image none w =&gt; w.sectionId == &quot;about&quot;' name='is-simple'/>
        <div class='container row-x1 flex-sb'>
          <div class='footer-copyright' id='footer-copyright'>
            <span class='copyright-text'>Design by - <a href='https://copybloggerthemes.com/' rel='dofollow' title='Blogger Templates' style='color:#3b82f6;' target='_blank'>Blogger Templates</a> | <a href='https://probloggertemplates.com/' id='probtemplates' title='Pro Blogger Templates'>Premium Blogger Templates</a></span>
          </div>
          <b:section class='footer-menu' id='footer-menu' maxwidgets='1' name='Footer Menu' showaddelement='yes'>
            <b:widget id='LinkList204' locked='true' title='' type='LinkList' visible='true'>
              <b:widget-settings>
                <b:widget-setting name='link-3'>#</b:widget-setting>
                <b:widget-setting name='sorting'>NONE</b:widget-setting>
                <b:widget-setting name='text-1'>About Us</b:widget-setting>
                <b:widget-setting name='link-1'>#</b:widget-setting>
                <b:widget-setting name='text-0'>Home</b:widget-setting>
                <b:widget-setting name='link-2'>#</b:widget-setting>
                <b:widget-setting name='text-3'>Contact Us</b:widget-setting>
                <b:widget-setting name='link-0'>/</b:widget-setting>
                <b:widget-setting name='text-2'>Privacy Policy</b:widget-setting>
              </b:widget-settings>
              <b:includable id='main' var='this'>
      <b:include name='widget-title'/>
      <b:include name='content'/>
    </b:includable>
              <b:includable id='content'>
      <b:include name='linklist-content'/>
    </b:includable>
            </b:widget>
          </b:section>
        </div>
      </div>
    </footer>
  </b:if>
</div>
<b:if cond='!data:isFeed'>
<div class='site-overlay'>
  <div class='overlay-bg' id='overlay-bg'/>
  <b:include name='pbt-search'/>
  <b:include cond='data:view.isPost' name='share-modal'/>
  <b:include name='mobile-menu'/>
  <button aria-label='Back To Top' class='back-top btn'/>
</div>
<b:if cond='data:view.isSingleItem'>
  <!-- Hidden Widgets -->
  <b:section class='hidden' deleted='true' id='hidden' maxwidgets='1' showaddelement='no'>
    <b:widget id='ContactForm1' locked='true' title='Contact Form' type='ContactForm' visible='true'>
      <b:includable id='main' var='this'>
      <b:include name='widget-title'/>
      <b:include name='content'/>
    </b:includable>
      <b:includable id='content'>
      <b:include name='contact-form-content'/>
    </b:includable>
    </b:widget>
  </b:section>
</b:if>
<!-- Site Plugins -->
<b:tag name='script' src='https://cdnjs.cloudflare.com/ajax/libs/jquery/3.6.0/jquery.min.js' type='text/javascript'/>
<b:tag name='script' type='text/javascript'>
//<![CDATA[
/*! pbtStickySidebar | v1.0.0 - https://probloggertemplates.com/ */
!function(a){a.fn.pbtStickySidebar=function(b){function c(a,b){return!0===a.initialized|| !($("body").width()<a.minWidth)&&(d(a,b),!0)}function d(a,b){a.initialized=!0,b.each(function(){let b={};if(b.sidebar=$(this),b.options=a||{},b.container=$(b.options.containerSelector),0==b.container.length&&(b.container=b.sidebar.parent()),b.sidebar.parent().css("-webkit-transform","none"),b.sidebar.css({position:b.options.defaultPosition,overflow:"visible","-webkit-box-sizing":"border-box","-moz-box-sizing":"border-box","box-sizing":"border-box"}),b.stickySidebar=b.sidebar.find(".pbtStickySidebar"),0==b.stickySidebar.length){var f,g,i=/(?:text|application)\/(?:x-)?(?:javascript|ecmascript)/i;b.sidebar.find("script").filter(function(b,a){return 0===a.type.length||a.type.match(i)}).remove(),b.stickySidebar=$("<div>").addClass("pbtStickySidebar").append(b.sidebar.children()),b.sidebar.append(b.stickySidebar)}b.marginBottom=parseInt(b.sidebar.css("margin-bottom")),b.paddingTop=parseInt(b.sidebar.css("padding-top")),b.paddingBottom=parseInt(b.sidebar.css("padding-bottom"));let c=b.stickySidebar.offset().top,d=b.stickySidebar.outerHeight();function h(){b.fixedScrollTop=0,b.sidebar.css({"min-height":"1px"}),b.stickySidebar.css({position:"static",width:"",transform:"none"})}b.stickySidebar.css("padding-top",1),b.stickySidebar.css("padding-bottom",1),c-=b.stickySidebar.offset().top,d=b.stickySidebar.outerHeight()-d-c,0==c?(b.stickySidebar.css("padding-top",0),b.stickySidebarPaddingTop=0):b.stickySidebarPaddingTop=1,0==d?(b.stickySidebar.css("padding-bottom",0),b.stickySidebarPaddingBottom=0):b.stickySidebarPaddingBottom=1,b.previousScrollTop=null,b.fixedScrollTop=0,h(),b.onScroll=function(b){if(!b.stickySidebar.is(":visible"))return;if($("body").width()<b.options.minWidth||b.options.disableOnResponsiveLayouts&&b.sidebar.outerWidth("none"==b.sidebar.css("float"))+50>b.container.width()){h();return}let d=$(document).scrollTop(),g="static",c=0;if(d>=b.sidebar.offset().top+(b.paddingTop-b.options.additionalMarginTop)){let k,n=b.paddingTop+a.additionalMarginTop,o=b.paddingBottom+b.marginBottom+a.additionalMarginBottom,p=b.sidebar.offset().top,q=b.sidebar.offset().top+(k=(v=b.container).height(),v.children().each(function(){k=Math.max(k,$(this).height())}),k),j=0+a.additionalMarginTop,i,r=b.stickySidebar.outerHeight()+n+o<$(window).height();i=r?j+b.stickySidebar.outerHeight():$(window).height()-b.marginBottom-b.paddingBottom-a.additionalMarginBottom;let s=p-d+b.paddingTop,t=q-d-b.paddingBottom-b.marginBottom;c=b.stickySidebar.offset().top-d;let l=b.previousScrollTop-d;"fixed"==b.stickySidebar.css("position")&&"modern"==b.options.sidebarBehavior&&(c+=l),"stick-to-top"==b.options.sidebarBehavior&&(c=a.additionalMarginTop),"stick-to-bottom"==b.options.sidebarBehavior&&(c=i-b.stickySidebar.outerHeight()),c=l>0?Math.min(c,j):Math.max(c,i-b.stickySidebar.outerHeight()),c=Math.max(c,s),c=Math.min(c,t-b.stickySidebar.outerHeight());var v,m=b.container.height()==b.stickySidebar.outerHeight();g=(m||c!=j)&&(m||c!=i-b.stickySidebar.outerHeight())?d+c-b.sidebar.offset().top-b.paddingTop<=a.additionalMarginTop?"static":"absolute":"fixed"}if("fixed"==g){let u=$(document).scrollLeft();b.stickySidebar.css({position:"fixed",width:e(b.stickySidebar)+"px",transform:"translate3d(0, "+c+"px, 0)",left:b.sidebar.offset().left+parseInt(b.sidebar.css("padding-left"))-u+"px",top:"0px"})}else if("absolute"==g){let f={};"absolute"!=b.stickySidebar.css("position")&&(f.position="absolute",f.transform="translate3d(0, "+(d+c-b.sidebar.offset().top-b.stickySidebarPaddingTop-b.stickySidebarPaddingBottom)+"px, 0)",f.top="0px"),f.width=e(b.stickySidebar)+"px",f.left="",b.stickySidebar.css(f)}else"static"==g&&h();"static"!=g&& !0==b.options.updateSidebarHeight&&b.sidebar.css({"min-height":b.stickySidebar.outerHeight()+b.stickySidebar.offset().top-b.sidebar.offset().top+b.paddingBottom}),b.previousScrollTop=d},b.onScroll(b),$(document).on("scroll."+b.options.namespace,(f=b,function(){f.onScroll(f)})),$(window).on("resize."+b.options.namespace,(g=b,function(){g.stickySidebar.css({position:"static"}),g.onScroll(g)}))})}function e(b){let a;try{a=b[0].getBoundingClientRect().width}catch(c){}return void 0===a&&(a=b.width()),a}return(b=a.extend({containerSelector:"",additionalMarginTop:0,additionalMarginBottom:0,updateSidebarHeight:!0,minWidth:0,disableOnResponsiveLayouts:!0,sidebarBehavior:"modern",defaultPosition:"relative",namespace:"PBT"},b)).additionalMarginTop=parseInt(b.additionalMarginTop)||0,b.additionalMarginBottom=parseInt(b.additionalMarginBottom)||0,function(a,b){let d=c(a,b);if(!d){var e,f,g,h;console.log("PBT: Body width smaller than options.minWidth. Init is delayed."),$(document).on("scroll."+a.namespace,(e=a,f=b,function(a){let b=c(e,f);b&&$(this).unbind(a)})),$(window).on("resize."+a.namespace,(g=a,h=b,function(a){let b=c(g,h);b&&$(this).unbind(a)}))}}(b,this),this}}(jQuery);

/*! pbtMenu by Pro Blogger Templates | v1.5.0 - https://probloggertemplates.com */
!function(a){a.fn.pbtMenu=function(){return this.each(function(){const b=a(this),c=b.find("a"),d=c.length;function e(e,h,f,g){for(let a=0;a<h;a++){const c=e.eq(a),d=c.text(),b="_";if(d.charAt(0)!==b){const i=e.eq(a+1),j=i.text();j.charAt(0)===b&&(g=c.parent()).append('<ul class="sub-menu sm-'+f+'"/>')}d.charAt(0)===b&&c.text(d.replace(b,"")).parent().appendTo(g.children(".sm-"+f))}}e(c,d,1),e(c,d,2),b.find(".sub-menu").parent("li").addClass("has-sub"),b.children(".widget").addClass("is-ready")})}}(jQuery);

/*! jQuery replaceText | v1.1.0 - https://benalman.com/projects/jquery-replacetext-plugin */
!function(a){a.fn.replaceText=function(a,b,c){return this.each(function(){var g,e,d=this.firstChild,f=[];if(d)do 3===d.nodeType&&(e=(g=d.nodeValue).replace(a,b))!==g&&(!c&&/</.test(e)?($(d).before(e),f.push(d)):d.nodeValue=e);while(d=d.nextSibling)f.length&&$(f).remove()})}}(jQuery);
//]]>
</b:tag>
<!-- Site Scripts -->
<b:tag name='script' type='text/javascript'>
//<![CDATA[
var _$_pbtJS=["\x32\x7A\x20\x61\x24\x65\x3D\x5B\x22\x5C\x44\x5C\x6C\x5C\x66\x5C\x78\x5C\x6C\x5C\x69\x5C\x6D\x5C\x6E\x5C\x73\x5C\x69\x22\x2C\x22\x5C\x76\x5C\x7A\x5C\x69\x5C\x31\x79\x5C\x6A\x5C\x31\x6B\x5C\x4C\x22\x2C\x22\x5C\x53\x5C\x70\x22\x2C\x22\x5C\x66\x5C\x54\x5C\x69\x5C\x66\x5C\x70\x5C\x41\x22\x2C\x22\x5C\x52\x5C\x6E\x5C\x41\x5C\x69\x5C\x47\x22\x2C\x22\x5C\x47\x5C\x66\x5C\x6E\x5C\x48\x5C\x47\x5C\x69\x22\x2C\x22\x5C\x52\x22\x2C\x22\x5C\x6D\x5C\x6B\x5C\x44\x5C\x70\x5C\x41\x22\x2C\x22\x5C\x72\x5C\x47\x22\x2C\x22\x5C\x72\x5C\x76\x5C\x72\x5C\x57\x5C\x72\x5C\x70\x5C\x6B\x5C\x72\x5C\x70\x5C\x44\x22\x2C\x22\x5C\x6C\x5C\x6D\x5C\x73\x22\x2C\x22\x5C\x41\x5C\x6A\x5C\x69\x5C\x6A\x22\x2C\x22\x5C\x45\x5C\x52\x5C\x66\x5C\x7A\x5C\x76\x22\x2C\x22\x5C\x75\x5C\x6A\x5C\x69\x5C\x73\x5C\x47\x22\x2C\x22\x5C\x69\x5C\x6B\x5C\x31\x79\x5C\x6B\x5C\x52\x5C\x66\x5C\x6D\x5C\x31\x6E\x5C\x6A\x5C\x6C\x5C\x66\x22\x2C\x22\x22\x2C\x22\x5C\x72\x5C\x6D\x5C\x52\x22\x2C\x22\x5C\x6D\x5C\x66\x5C\x6C\x5C\x6B\x5C\x44\x5C\x6D\x5C\x73\x5C\x66\x5C\x6C\x5C\x45\x5C\x7A\x5C\x6F\x5C\x6B\x5C\x48\x5C\x7A\x5C\x6F\x5C\x6B\x5C\x48\x5C\x45\x5C\x73\x5C\x6B\x5C\x75\x22\x2C\x22\x5C\x44\x5C\x70\x5C\x41\x5C\x66\x5C\x53\x5C\x6E\x5C\x70\x5C\x66\x5C\x41\x22\x2C\x22\x5C\x70\x5C\x6B\x5C\x31\x6F\x5C\x47\x5C\x44\x5C\x75\x5C\x7A\x22\x2C\x22\x5C\x4B\x5C\x6E\x5C\x75\x5C\x48\x5C\x4B\x5C\x6A\x22\x2C\x22\x5C\x4B\x5C\x7A\x5C\x6F\x5C\x6B\x5C\x48\x5C\x48\x5C\x66\x5C\x6D\x5C\x31\x4E\x5C\x6E\x5C\x75\x5C\x48\x5C\x31\x4E\x5C\x76\x5C\x6D\x5C\x6B\x5C\x54\x5C\x4C\x22\x2C\x22\x5C\x4A\x22\x2C\x22\x5C\x6C\x5C\x76\x5C\x6F\x5C\x6E\x5C\x69\x22\x2C\x22\x5C\x4A\x5C\x52\x5C\x31\x71\x5C\x31\x61\x5C\x72\x5C\x47\x5C\x31\x71\x5C\x31\x61\x5C\x72\x5C\x76\x5C\x72\x5C\x57\x5C\x72\x5C\x70\x5C\x6B\x5C\x72\x5C\x70\x5C\x44\x22\x2C\x22\x5C\x69\x5C\x66\x5C\x6C\x5C\x69\x5C\x6B\x5C\x70\x5C\x6F\x5C\x4C\x22\x2C\x22\x5C\x72\x5C\x69\x5C\x66\x5C\x6C\x5C\x69\x5C\x6B\x5C\x70\x5C\x6F\x5C\x4C\x5C\x45\x22\x2C\x22\x5C\x45\x22\x2C\x22\x5C\x6D\x5C\x66\x5C\x76\x5C\x6F\x5C\x6A\x5C\x73\x5C\x66\x22\x2C\x22\x5C\x6B\x5C\x70\x5C\x6F\x5C\x6B\x5C\x6A\x5C\x41\x22\x2C\x22\x5C\x76\x5C\x7A\x5C\x69\x5C\x72\x5C\x6F\x5C\x6A\x5C\x31\x6B\x5C\x4C\x22\x2C\x22\x5C\x6A\x5C\x41\x5C\x41\x5C\x31\x6E\x5C\x6F\x5C\x6A\x5C\x6C\x5C\x6C\x22\x2C\x22\x5C\x6C\x5C\x69\x5C\x4C\x5C\x6F\x5C\x66\x22\x2C\x22\x5C\x7A\x5C\x6A\x5C\x73\x5C\x57\x5C\x48\x5C\x6D\x5C\x6B\x5C\x44\x5C\x70\x5C\x41\x5C\x72\x5C\x6E\x5C\x75\x5C\x6A\x5C\x48\x5C\x66\x5C\x31\x62\x5C\x44\x5C\x6D\x5C\x6F\x5C\x34\x6E\x5C\x37\x6A\x22\x2C\x22\x5C\x37\x6A\x5C\x34\x65\x22\x2C\x22\x5C\x6A\x5C\x69\x5C\x69\x5C\x6D\x22\x2C\x22\x5C\x4B\x5C\x6C\x5C\x31\x71\x5C\x31\x61\x5C\x72\x5C\x73\x22\x2C\x22\x5C\x4B\x22\x2C\x22\x5C\x4B\x5C\x52\x5C\x31\x71\x5C\x31\x61\x5C\x72\x5C\x47\x22\x2C\x22\x5C\x4B\x5C\x52\x5C\x31\x71\x5C\x31\x61\x5C\x72\x5C\x47\x5C\x31\x71\x5C\x31\x61\x5C\x72\x5C\x76\x5C\x72\x5C\x57\x5C\x72\x5C\x70\x5C\x6B\x5C\x72\x5C\x70\x5C\x44\x22\x2C\x22\x5C\x4A\x5C\x52\x5C\x31\x71\x5C\x31\x61\x5C\x72\x5C\x47\x22\x2C\x22\x5C\x6B\x5C\x70\x5C\x31\x75\x5C\x73\x5C\x6D\x5C\x6B\x5C\x6F\x5C\x6F\x22\x2C\x22\x5C\x6C\x5C\x73\x5C\x6D\x5C\x6B\x5C\x6F\x5C\x6F\x22\x2C\x22\x5C\x69\x5C\x6D\x5C\x6E\x5C\x48\x5C\x48\x5C\x66\x5C\x6D\x22\x2C\x22\x5C\x6F\x5C\x6B\x5C\x6A\x5C\x41\x5C\x78\x5C\x6D\x5C\x66\x5C\x6C\x5C\x6E\x5C\x31\x6B\x5C\x66\x5C\x78\x5C\x6C\x5C\x73\x5C\x6D\x5C\x6B\x5C\x6F\x5C\x6F\x22\x2C\x22\x5C\x6C\x5C\x73\x5C\x6D\x5C\x6B\x5C\x6F\x5C\x6F\x5C\x31\x6F\x5C\x6B\x5C\x76\x22\x2C\x22\x5C\x69\x5C\x6B\x5C\x76\x22\x2C\x22\x5C\x6B\x5C\x53\x5C\x53\x5C\x6C\x5C\x66\x5C\x69\x22\x2C\x22\x5C\x6B\x5C\x53\x5C\x53\x22\x2C\x22\x5C\x6B\x5C\x70\x22\x2C\x22\x5C\x6F\x5C\x6B\x5C\x6A\x5C\x41\x22\x2C\x22\x5C\x66\x5C\x6A\x5C\x73\x5C\x47\x22\x2C\x22\x5C\x47\x5C\x69\x5C\x75\x5C\x6F\x22\x2C\x22\x5C\x7A\x5C\x6B\x5C\x41\x5C\x4C\x22\x2C\x22\x5C\x32\x43\x22\x2C\x22\x5C\x6F\x5C\x66\x5C\x70\x5C\x48\x5C\x69\x5C\x47\x22\x2C\x22\x5C\x69\x5C\x6D\x5C\x6E\x5C\x75\x22\x2C\x22\x5C\x6C\x5C\x66\x5C\x6A\x5C\x6D\x5C\x73\x5C\x47\x5C\x31\x4E\x5C\x69\x5C\x66\x5C\x6D\x5C\x75\x22\x2C\x22\x5C\x75\x5C\x6C\x5C\x31\x69\x5C\x31\x71\x22\x2C\x22\x5C\x45\x5C\x6B\x5C\x50\x5C\x66\x5C\x6D\x5C\x6F\x5C\x6A\x5C\x4C\x5C\x72\x5C\x7A\x5C\x48\x22\x2C\x22\x5C\x6C\x5C\x66\x5C\x6A\x5C\x6D\x5C\x73\x5C\x47\x5C\x72\x5C\x6B\x5C\x70\x22\x2C\x22\x5C\x53\x5C\x6B\x5C\x73\x5C\x44\x5C\x6C\x22\x2C\x22\x5C\x45\x5C\x75\x5C\x6A\x5C\x6E\x5C\x70\x5C\x72\x5C\x6C\x5C\x66\x5C\x6A\x5C\x6D\x5C\x73\x5C\x47\x5C\x78\x5C\x6E\x5C\x70\x5C\x76\x5C\x44\x5C\x69\x22\x2C\x22\x5C\x50\x5C\x6A\x5C\x6F\x22\x2C\x22\x5C\x7A\x5C\x6F\x5C\x44\x5C\x6D\x22\x2C\x22\x5C\x50\x5C\x6E\x5C\x6C\x5C\x6E\x5C\x7A\x5C\x6F\x5C\x66\x22\x2C\x22\x5C\x6D\x5C\x66\x5C\x75\x5C\x6B\x5C\x50\x5C\x66\x5C\x31\x6E\x5C\x6F\x5C\x6A\x5C\x6C\x5C\x6C\x22\x2C\x22\x5C\x76\x5C\x6A\x5C\x6D\x5C\x66\x5C\x70\x5C\x69\x22\x2C\x22\x5C\x45\x5C\x6C\x5C\x66\x5C\x6A\x5C\x6D\x5C\x73\x5C\x47\x5C\x72\x5C\x6D\x5C\x66\x5C\x6C\x5C\x44\x5C\x6F\x5C\x69\x5C\x6C\x22\x2C\x22\x5C\x73\x5C\x6F\x5C\x6E\x5C\x73\x5C\x57\x22\x2C\x22\x5C\x45\x5C\x6C\x5C\x66\x5C\x6A\x5C\x6D\x5C\x73\x5C\x47\x5C\x72\x5C\x6B\x5C\x70\x5C\x78\x5C\x45\x5C\x6B\x5C\x50\x5C\x66\x5C\x6D\x5C\x6F\x5C\x6A\x5C\x4C\x5C\x72\x5C\x7A\x5C\x48\x22\x2C\x22\x5C\x57\x5C\x66\x5C\x4C\x5C\x41\x5C\x6B\x5C\x52\x5C\x70\x22\x2C\x22\x5C\x57\x5C\x66\x5C\x4C\x5C\x31\x6E\x5C\x6B\x5C\x41\x5C\x66\x22\x2C\x22\x5C\x6C\x5C\x47\x5C\x6A\x5C\x6D\x5C\x66\x5C\x72\x5C\x6B\x5C\x70\x22\x2C\x22\x5C\x45\x5C\x47\x5C\x6E\x5C\x41\x5C\x66\x5C\x72\x5C\x75\x5C\x6B\x5C\x41\x5C\x6A\x5C\x6F\x5C\x31\x77\x5C\x78\x5C\x45\x5C\x6C\x5C\x47\x5C\x6A\x5C\x6D\x5C\x66\x5C\x72\x5C\x6B\x5C\x70\x5C\x78\x5C\x45\x5C\x6B\x5C\x50\x5C\x66\x5C\x6D\x5C\x6F\x5C\x6A\x5C\x4C\x5C\x72\x5C\x7A\x5C\x48\x22\x2C\x22\x5C\x47\x5C\x6D\x5C\x66\x5C\x53\x22\x2C\x22\x5C\x31\x4E\x5C\x6C\x5C\x66\x5C\x6F\x5C\x53\x22\x2C\x22\x5C\x6B\x5C\x76\x5C\x66\x5C\x70\x22\x2C\x22\x5C\x4E\x5C\x6C\x5C\x76\x5C\x6A\x5C\x70\x5C\x78\x5C\x73\x5C\x6F\x5C\x6A\x5C\x6C\x5C\x6C\x5C\x4A\x5C\x42\x5C\x66\x5C\x6D\x5C\x6D\x5C\x6B\x5C\x6D\x5C\x72\x5C\x75\x5C\x6C\x5C\x48\x5C\x42\x5C\x4F\x22\x2C\x22\x5C\x6C\x5C\x66\x5C\x6A\x5C\x6D\x5C\x73\x5C\x47\x22\x2C\x22\x5C\x4E\x5C\x7A\x5C\x4F\x5C\x31\x42\x5C\x6D\x5C\x6D\x5C\x6B\x5C\x6D\x5C\x31\x62\x5C\x4E\x5C\x4B\x5C\x7A\x5C\x4F\x5C\x31\x4D\x5C\x70\x5C\x7A\x5C\x6C\x5C\x76\x5C\x31\x65\x22\x2C\x22\x5C\x70\x5C\x6B\x5C\x32\x77\x5C\x66\x5C\x6C\x5C\x44\x5C\x6F\x5C\x69\x5C\x6C\x22\x2C\x22\x5C\x4E\x5C\x4B\x5C\x6C\x5C\x76\x5C\x6A\x5C\x70\x5C\x4F\x22\x2C\x22\x5C\x4E\x5C\x41\x5C\x6E\x5C\x50\x5C\x78\x5C\x73\x5C\x6F\x5C\x6A\x5C\x6C\x5C\x6C\x5C\x4A\x5C\x42\x5C\x6F\x5C\x6B\x5C\x6A\x5C\x41\x5C\x66\x5C\x6D\x5C\x42\x5C\x4F\x5C\x4E\x5C\x6C\x5C\x50\x5C\x48\x5C\x78\x5C\x73\x5C\x6F\x5C\x6A\x5C\x6C\x5C\x6C\x5C\x4A\x5C\x42\x5C\x6C\x5C\x76\x5C\x6E\x5C\x70\x5C\x70\x5C\x66\x5C\x6D\x5C\x42\x5C\x78\x5C\x50\x5C\x6E\x5C\x66\x5C\x52\x5C\x31\x50\x5C\x6B\x5C\x54\x5C\x4A\x5C\x42\x5C\x31\x66\x5C\x78\x5C\x31\x66\x5C\x78\x5C\x31\x67\x5C\x31\x66\x5C\x78\x5C\x31\x67\x5C\x31\x66\x5C\x42\x5C\x4F\x5C\x4E\x5C\x73\x5C\x6E\x5C\x6D\x5C\x73\x5C\x6F\x5C\x66\x5C\x78\x5C\x73\x5C\x6F\x5C\x6A\x5C\x6C\x5C\x6C\x5C\x4A\x5C\x42\x5C\x76\x5C\x6A\x5C\x69\x5C\x47\x5C\x42\x5C\x78\x5C\x73\x5C\x54\x5C\x4A\x5C\x42\x5C\x31\x61\x5C\x31\x67\x5C\x42\x5C\x78\x5C\x73\x5C\x4C\x5C\x4A\x5C\x42\x5C\x31\x61\x5C\x31\x67\x5C\x42\x5C\x78\x5C\x6D\x5C\x4A\x5C\x42\x5C\x31\x61\x5C\x31\x66\x5C\x42\x5C\x4F\x5C\x4E\x5C\x4B\x5C\x73\x5C\x6E\x5C\x6D\x5C\x73\x5C\x6F\x5C\x66\x5C\x4F\x5C\x4E\x5C\x4B\x5C\x6C\x5C\x50\x5C\x48\x5C\x4F\x5C\x4E\x5C\x4B\x5C\x41\x5C\x6E\x5C\x50\x5C\x4F\x22\x2C\x22\x5C\x6D\x5C\x66\x5C\x73\x5C\x66\x5C\x70\x5C\x69\x22\x2C\x22\x5C\x4B\x5C\x6C\x5C\x66\x5C\x6A\x5C\x6D\x5C\x73\x5C\x47\x5C\x4B\x5C\x32\x79\x5C\x7A\x5C\x4C\x5C\x72\x5C\x41\x5C\x6A\x5C\x69\x5C\x66\x5C\x4A\x5C\x69\x5C\x6D\x5C\x44\x5C\x66\x5C\x31\x4D\x5C\x75\x5C\x6A\x5C\x54\x5C\x72\x5C\x6D\x5C\x66\x5C\x6C\x5C\x44\x5C\x6F\x5C\x69\x5C\x6C\x5C\x4A\x22\x2C\x22\x5C\x31\x4D\x5C\x6A\x5C\x75\x5C\x76\x5C\x4A\x5C\x31\x69\x22\x2C\x22\x5C\x4B\x5C\x6C\x5C\x66\x5C\x6A\x5C\x6D\x5C\x73\x5C\x47\x5C\x4B\x5C\x6F\x5C\x6A\x5C\x7A\x5C\x66\x5C\x6F\x5C\x4B\x22\x2C\x22\x5C\x32\x79\x5C\x7A\x5C\x4C\x5C\x72\x5C\x41\x5C\x6A\x5C\x69\x5C\x66\x5C\x4A\x5C\x69\x5C\x6D\x5C\x44\x5C\x66\x5C\x31\x4D\x5C\x75\x5C\x6A\x5C\x54\x5C\x72\x5C\x6D\x5C\x66\x5C\x6C\x5C\x44\x5C\x6F\x5C\x69\x5C\x6C\x5C\x4A\x22\x2C\x22\x5C\x6E\x5C\x41\x22\x2C\x22\x5C\x6F\x5C\x6E\x5C\x70\x5C\x57\x22\x2C\x22\x5C\x69\x5C\x6E\x5C\x69\x5C\x6F\x5C\x66\x22\x2C\x22\x5C\x76\x5C\x6B\x5C\x6C\x5C\x69\x5C\x31\x58\x5C\x44\x5C\x69\x5C\x47\x5C\x6B\x5C\x6D\x5C\x31\x79\x5C\x6A\x5C\x7A\x5C\x66\x5C\x6F\x22\x2C\x22\x5C\x76\x5C\x6B\x5C\x6C\x5C\x69\x5C\x31\x58\x5C\x44\x5C\x69\x5C\x47\x5C\x6B\x5C\x6D\x22\x2C\x22\x5C\x4E\x5C\x6C\x5C\x76\x5C\x6A\x5C\x70\x5C\x78\x5C\x73\x5C\x6F\x5C\x6A\x5C\x6C\x5C\x6C\x5C\x4A\x5C\x42\x5C\x66\x5C\x70\x5C\x69\x5C\x6D\x5C\x4C\x5C\x72\x5C\x6A\x5C\x44\x5C\x69\x5C\x47\x5C\x6B\x5C\x6D\x5C\x42\x5C\x4F\x5C\x4E\x5C\x6C\x5C\x76\x5C\x6A\x5C\x70\x5C\x78\x5C\x73\x5C\x6F\x5C\x6A\x5C\x6C\x5C\x6C\x5C\x4A\x5C\x42\x5C\x6A\x5C\x44\x5C\x69\x5C\x47\x5C\x6B\x5C\x6D\x5C\x72\x5C\x70\x5C\x6A\x5C\x75\x5C\x66\x5C\x42\x5C\x4F\x22\x2C\x22\x5C\x6A\x5C\x44\x5C\x69\x5C\x47\x5C\x6B\x5C\x6D\x22\x2C\x22\x5C\x4E\x5C\x4B\x5C\x6C\x5C\x76\x5C\x6A\x5C\x70\x5C\x4F\x5C\x4E\x5C\x4B\x5C\x6C\x5C\x76\x5C\x6A\x5C\x70\x5C\x4F\x22\x2C\x22\x5C\x41\x5C\x6A\x5C\x69\x5C\x66\x22\x2C\x22\x5C\x76\x5C\x44\x5C\x7A\x5C\x6F\x5C\x6E\x5C\x6C\x5C\x47\x5C\x66\x5C\x41\x22\x2C\x22\x5C\x41\x5C\x6A\x5C\x69\x5C\x66\x5C\x69\x5C\x6E\x5C\x75\x5C\x66\x22\x2C\x22\x5C\x76\x5C\x6B\x5C\x6C\x5C\x69\x5C\x31\x52\x5C\x6A\x5C\x69\x5C\x66\x5C\x31\x79\x5C\x6A\x5C\x7A\x5C\x66\x5C\x6F\x22\x2C\x22\x5C\x4E\x5C\x6C\x5C\x76\x5C\x6A\x5C\x70\x5C\x78\x5C\x73\x5C\x6F\x5C\x6A\x5C\x6C\x5C\x6C\x5C\x4A\x5C\x42\x5C\x6C\x5C\x76\x5C\x42\x5C\x4F\x22\x2C\x22\x5C\x76\x5C\x6B\x5C\x6C\x5C\x69\x5C\x31\x52\x5C\x6A\x5C\x69\x5C\x66\x22\x2C\x22\x5C\x4E\x5C\x6C\x5C\x76\x5C\x6A\x5C\x70\x5C\x78\x5C\x73\x5C\x6F\x5C\x6A\x5C\x6C\x5C\x6C\x5C\x4A\x5C\x42\x5C\x66\x5C\x70\x5C\x69\x5C\x6D\x5C\x4C\x5C\x72\x5C\x69\x5C\x6E\x5C\x75\x5C\x66\x5C\x42\x5C\x4F\x22\x2C\x22\x5C\x4E\x5C\x69\x5C\x6E\x5C\x75\x5C\x66\x5C\x78\x5C\x73\x5C\x6F\x5C\x6A\x5C\x6C\x5C\x6C\x5C\x4A\x5C\x42\x5C\x76\x5C\x44\x5C\x7A\x5C\x6F\x5C\x6E\x5C\x6C\x5C\x47\x5C\x66\x5C\x41\x5C\x42\x5C\x78\x5C\x41\x5C\x6A\x5C\x69\x5C\x66\x5C\x69\x5C\x6E\x5C\x75\x5C\x66\x5C\x4A\x5C\x42\x22\x2C\x22\x5C\x42\x5C\x4F\x22\x2C\x22\x5C\x4E\x5C\x4B\x5C\x69\x5C\x6E\x5C\x75\x5C\x66\x5C\x4F\x5C\x4E\x5C\x4B\x5C\x6C\x5C\x76\x5C\x6A\x5C\x70\x5C\x4F\x22\x2C\x22\x5C\x4E\x5C\x6C\x5C\x76\x5C\x6A\x5C\x70\x5C\x78\x5C\x73\x5C\x6F\x5C\x6A\x5C\x6C\x5C\x6C\x5C\x4A\x5C\x42\x5C\x66\x5C\x70\x5C\x69\x5C\x6D\x5C\x4C\x5C\x72\x5C\x69\x5C\x6E\x5C\x75\x5C\x66\x5C\x42\x5C\x4F\x5C\x4E\x5C\x69\x5C\x6E\x5C\x75\x5C\x66\x5C\x78\x5C\x73\x5C\x6F\x5C\x6A\x5C\x6C\x5C\x6C\x5C\x4A\x5C\x42\x5C\x76\x5C\x44\x5C\x7A\x5C\x6F\x5C\x6E\x5C\x6C\x5C\x47\x5C\x66\x5C\x41\x5C\x42\x5C\x78\x5C\x41\x5C\x6A\x5C\x69\x5C\x66\x5C\x69\x5C\x6E\x5C\x75\x5C\x66\x5C\x4A\x5C\x42\x22\x2C\x22\x5C\x4E\x5C\x41\x5C\x6E\x5C\x50\x5C\x78\x5C\x73\x5C\x6F\x5C\x6A\x5C\x6C\x5C\x6C\x5C\x4A\x5C\x42\x5C\x66\x5C\x70\x5C\x69\x5C\x6D\x5C\x4C\x5C\x72\x5C\x75\x5C\x66\x5C\x69\x5C\x6A\x5C\x42\x5C\x4F\x22\x2C\x22\x5C\x4E\x5C\x4B\x5C\x41\x5C\x6E\x5C\x50\x5C\x4F\x22\x2C\x22\x5C\x69\x5C\x47\x5C\x44\x5C\x75\x5C\x7A\x5C\x70\x5C\x6A\x5C\x6E\x5C\x6F\x22\x2C\x22\x5C\x78\x5C\x4C\x5C\x69\x5C\x72\x5C\x6E\x5C\x75\x5C\x48\x22\x2C\x22\x5C\x31\x62\x5C\x54\x22\x2C\x22\x5C\x4C\x5C\x6B\x5C\x44\x5C\x69\x5C\x44\x5C\x7A\x5C\x66\x22\x2C\x22\x5C\x6C\x5C\x6B\x5C\x44\x5C\x6D\x5C\x73\x5C\x66\x22\x2C\x22\x5C\x50\x5C\x6E\x5C\x41\x5C\x66\x5C\x6B\x22\x2C\x22\x5C\x73\x5C\x6A\x5C\x69\x5C\x66\x5C\x48\x5C\x6B\x5C\x6D\x5C\x4C\x22\x2C\x22\x5C\x76\x5C\x6B\x5C\x6C\x5C\x69\x5C\x31\x6E\x5C\x6A\x5C\x69\x5C\x66\x5C\x48\x5C\x6B\x5C\x6D\x5C\x4C\x22\x2C\x22\x5C\x4E\x5C\x6C\x5C\x76\x5C\x6A\x5C\x70\x5C\x78\x5C\x73\x5C\x6F\x5C\x6A\x5C\x6C\x5C\x6C\x5C\x4A\x5C\x42\x5C\x66\x5C\x70\x5C\x69\x5C\x6D\x5C\x4C\x5C\x72\x5C\x69\x5C\x6A\x5C\x48\x5C\x42\x5C\x4F\x22\x2C\x22\x5C\x6C\x5C\x44\x5C\x75\x5C\x75\x5C\x6A\x5C\x6D\x5C\x4C\x22\x2C\x22\x5C\x76\x5C\x6B\x5C\x6C\x5C\x69\x5C\x31\x75\x5C\x44\x5C\x75\x5C\x75\x5C\x6A\x5C\x6D\x5C\x4C\x22\x2C\x22\x5C\x4E\x5C\x6C\x5C\x76\x5C\x6A\x5C\x70\x5C\x78\x5C\x73\x5C\x6F\x5C\x6A\x5C\x6C\x5C\x6C\x5C\x4A\x5C\x42\x5C\x66\x5C\x70\x5C\x69\x5C\x6D\x5C\x4C\x5C\x72\x5C\x66\x5C\x54\x5C\x73\x5C\x66\x5C\x6D\x5C\x76\x5C\x69\x5C\x78\x5C\x66\x5C\x54\x5C\x73\x5C\x66\x5C\x6D\x5C\x76\x5C\x69\x5C\x42\x5C\x4F\x22\x2C\x22\x5C\x6C\x5C\x44\x5C\x7A\x5C\x6C\x5C\x69\x5C\x6D\x22\x2C\x22\x5C\x38\x43\x5C\x4E\x5C\x4B\x5C\x6C\x5C\x76\x5C\x6A\x5C\x70\x5C\x4F\x22\x2C\x22\x5C\x69\x5C\x4C\x5C\x76\x5C\x66\x22\x2C\x22\x5C\x76\x5C\x6B\x5C\x6C\x5C\x69\x22\x2C\x22\x5C\x6E\x5C\x70\x5C\x41\x5C\x66\x5C\x54\x22\x2C\x22\x5C\x70\x5C\x44\x5C\x75\x22\x2C\x22\x5C\x47\x5C\x66\x5C\x6A\x5C\x41\x5C\x6F\x5C\x6E\x5C\x70\x5C\x66\x22\x2C\x22\x5C\x69\x5C\x6A\x5C\x6D\x5C\x48\x5C\x66\x5C\x69\x22\x2C\x22\x5C\x4E\x5C\x41\x5C\x6E\x5C\x50\x5C\x78\x5C\x73\x5C\x6F\x5C\x6A\x5C\x6C\x5C\x6C\x5C\x4A\x5C\x42\x5C\x76\x5C\x6B\x5C\x6C\x5C\x69\x5C\x78\x5C\x6E\x5C\x69\x5C\x66\x5C\x75\x5C\x72\x22\x2C\x22\x5C\x42\x5C\x4F\x5C\x4E\x5C\x6A\x5C\x78\x5C\x73\x5C\x6F\x5C\x6A\x5C\x6C\x5C\x6C\x5C\x4A\x5C\x42\x5C\x66\x5C\x70\x5C\x69\x5C\x6D\x5C\x4C\x5C\x72\x5C\x69\x5C\x47\x5C\x44\x5C\x75\x5C\x7A\x5C\x70\x5C\x6A\x5C\x6E\x5C\x6F\x22\x2C\x22\x5C\x42\x5C\x78\x5C\x47\x5C\x6D\x5C\x66\x5C\x53\x5C\x4A\x5C\x42\x22\x2C\x22\x5C\x42\x5C\x78\x5C\x69\x5C\x6E\x5C\x69\x5C\x6F\x5C\x66\x5C\x4A\x5C\x42\x22\x2C\x22\x5C\x42\x5C\x4F\x5C\x4E\x5C\x6C\x5C\x76\x5C\x6A\x5C\x70\x5C\x78\x5C\x73\x5C\x6F\x5C\x6A\x5C\x6C\x5C\x6C\x5C\x4A\x5C\x42\x5C\x69\x5C\x47\x5C\x44\x5C\x75\x5C\x7A\x5C\x70\x5C\x6A\x5C\x6E\x5C\x6F\x5C\x42\x5C\x78\x5C\x41\x5C\x6A\x5C\x69\x5C\x6A\x5C\x72\x5C\x6C\x5C\x6D\x5C\x73\x5C\x4A\x5C\x42\x22\x2C\x22\x5C\x42\x5C\x4F\x5C\x4E\x5C\x4B\x5C\x6C\x5C\x76\x5C\x6A\x5C\x70\x5C\x4F\x5C\x4E\x5C\x4B\x5C\x6A\x5C\x4F\x5C\x4E\x5C\x41\x5C\x6E\x5C\x50\x5C\x78\x5C\x73\x5C\x6F\x5C\x6A\x5C\x6C\x5C\x6C\x5C\x4A\x5C\x42\x5C\x66\x5C\x70\x5C\x69\x5C\x6D\x5C\x4C\x5C\x72\x5C\x47\x5C\x66\x5C\x6A\x5C\x41\x5C\x66\x5C\x6D\x5C\x42\x5C\x4F\x5C\x4E\x5C\x47\x5C\x31\x61\x5C\x78\x5C\x73\x5C\x6F\x5C\x6A\x5C\x6C\x5C\x6C\x5C\x4A\x5C\x42\x5C\x66\x5C\x70\x5C\x69\x5C\x6D\x5C\x4C\x5C\x72\x5C\x69\x5C\x6E\x5C\x69\x5C\x6F\x5C\x66\x5C\x42\x5C\x4F\x5C\x4E\x5C\x6A\x5C\x78\x5C\x47\x5C\x6D\x5C\x66\x5C\x53\x5C\x4A\x5C\x42\x22\x2C\x22\x5C\x4E\x5C\x4B\x5C\x6A\x5C\x4F\x5C\x4E\x5C\x4B\x5C\x47\x5C\x31\x61\x5C\x4F\x22\x2C\x22\x5C\x4E\x5C\x4B\x5C\x41\x5C\x6E\x5C\x50\x5C\x4F\x5C\x4E\x5C\x4B\x5C\x41\x5C\x6E\x5C\x50\x5C\x4F\x22\x2C\x22\x5C\x6D\x5C\x66\x5C\x6F\x5C\x6A\x5C\x69\x5C\x66\x5C\x41\x22\x2C\x22\x5C\x6D\x5C\x66\x5C\x6C\x5C\x76\x5C\x6B\x5C\x70\x5C\x6C\x5C\x66\x5C\x31\x6F\x5C\x66\x5C\x54\x5C\x69\x22\x2C\x22\x5C\x32\x6D\x5C\x31\x42\x5C\x31\x6F\x22\x2C\x22\x5C\x6A\x5C\x31\x48\x5C\x6A\x5C\x54\x22\x2C\x22\x5C\x69\x5C\x66\x5C\x54\x5C\x69\x22\x2C\x22\x5C\x31\x74\x5C\x41\x5C\x6A\x5C\x69\x5C\x6A\x22\x2C\x22\x5C\x53\x5C\x6E\x5C\x70\x5C\x41\x22\x2C\x22\x5C\x76\x5C\x6A\x5C\x6D\x5C\x6C\x5C\x66\x22\x2C\x22\x5C\x76\x5C\x6B\x5C\x6C\x5C\x69\x5C\x6C\x22\x2C\x22\x5C\x69\x22\x2C\x22\x5C\x6F\x5C\x6A\x5C\x7A\x5C\x66\x5C\x6F\x22\x2C\x22\x5C\x6D\x5C\x66\x5C\x75\x5C\x6B\x5C\x50\x5C\x66\x22\x2C\x22\x5C\x45\x5C\x50\x5C\x6E\x5C\x66\x5C\x52\x5C\x72\x5C\x6A\x5C\x6F\x5C\x6F\x22\x2C\x22\x5C\x4E\x5C\x41\x5C\x6E\x5C\x50\x5C\x78\x5C\x73\x5C\x6F\x5C\x6A\x5C\x6C\x5C\x6C\x5C\x4A\x5C\x42\x22\x2C\x22\x5C\x72\x5C\x6E\x5C\x69\x5C\x66\x5C\x75\x5C\x6C\x5C\x42\x5C\x4F\x22\x2C\x22\x5C\x6C\x5C\x76\x5C\x6F\x5C\x6E\x5C\x73\x5C\x66\x22\x2C\x22\x5C\x4E\x5C\x6A\x5C\x78\x5C\x73\x5C\x6F\x5C\x6A\x5C\x6C\x5C\x6C\x5C\x4A\x5C\x42\x5C\x50\x5C\x6E\x5C\x66\x5C\x52\x5C\x72\x5C\x6A\x5C\x6F\x5C\x6F\x5C\x78\x5C\x7A\x5C\x69\x5C\x70\x5C\x42\x5C\x78\x5C\x47\x5C\x6D\x5C\x66\x5C\x53\x5C\x4A\x5C\x42\x5C\x4B\x5C\x6C\x5C\x66\x5C\x6A\x5C\x6D\x5C\x73\x5C\x47\x5C\x32\x79\x5C\x31\x78\x5C\x4A\x22\x2C\x22\x5C\x31\x4D\x5C\x7A\x5C\x4C\x5C\x72\x5C\x41\x5C\x6A\x5C\x69\x5C\x66\x5C\x4A\x5C\x69\x5C\x6D\x5C\x44\x5C\x66\x5C\x42\x5C\x4F\x22\x2C\x22\x5C\x50\x5C\x6E\x5C\x66\x5C\x52\x5C\x31\x58\x5C\x6F\x5C\x6F\x22\x2C\x22\x5C\x4E\x5C\x4B\x5C\x6A\x5C\x4F\x22\x2C\x22\x5C\x6A\x5C\x76\x5C\x76\x5C\x66\x5C\x70\x5C\x41\x22\x2C\x22\x5C\x6C\x5C\x76\x5C\x6A\x5C\x70\x5C\x45\x5C\x69\x5C\x47\x5C\x44\x5C\x75\x5C\x7A\x5C\x70\x5C\x6A\x5C\x6E\x5C\x6F\x22\x2C\x22\x5C\x4B\x5C\x6C\x5C\x66\x5C\x6A\x5C\x6D\x5C\x73\x5C\x47\x5C\x4B\x5C\x32\x79\x5C\x31\x78\x5C\x4A\x22\x2C\x22\x5C\x31\x4D\x5C\x7A\x5C\x4C\x5C\x72\x5C\x41\x5C\x6A\x5C\x69\x5C\x66\x5C\x4A\x5C\x69\x5C\x6D\x5C\x44\x5C\x66\x5C\x31\x4D\x5C\x75\x5C\x6A\x5C\x54\x5C\x72\x5C\x6D\x5C\x66\x5C\x6C\x5C\x44\x5C\x6F\x5C\x69\x5C\x6C\x5C\x4A\x5C\x31\x67\x5C\x31\x4D\x5C\x6A\x5C\x75\x5C\x76\x5C\x4A\x5C\x31\x69\x22\x2C\x22\x5C\x6C\x5C\x69\x5C\x6E\x5C\x73\x5C\x57\x5C\x4C\x5C\x31\x75\x5C\x6E\x5C\x41\x5C\x66\x5C\x7A\x5C\x6A\x5C\x6D\x22\x2C\x22\x5C\x6C\x5C\x69\x5C\x6E\x5C\x73\x5C\x57\x5C\x4C\x5C\x32\x65\x5C\x66\x5C\x70\x5C\x44\x22\x2C\x22\x5C\x45\x5C\x47\x5C\x66\x5C\x6A\x5C\x41\x5C\x66\x5C\x6D\x5C\x72\x5C\x6E\x5C\x70\x5C\x70\x5C\x66\x5C\x6D\x22\x2C\x22\x5C\x45\x5C\x73\x5C\x6B\x5C\x70\x5C\x69\x5C\x66\x5C\x70\x5C\x69\x5C\x72\x5C\x52\x5C\x6D\x5C\x6A\x5C\x76\x5C\x78\x5C\x4F\x5C\x78\x5C\x45\x5C\x73\x5C\x6B\x5C\x70\x5C\x69\x5C\x6A\x5C\x6E\x5C\x70\x5C\x66\x5C\x6D\x22\x2C\x22\x5C\x76\x5C\x7A\x5C\x69\x5C\x31\x75\x5C\x69\x5C\x6E\x5C\x73\x5C\x57\x5C\x4C\x5C\x31\x75\x5C\x6E\x5C\x41\x5C\x66\x5C\x7A\x5C\x6A\x5C\x6D\x22\x2C\x22\x5C\x4B\x5C\x4B\x5C\x7A\x5C\x6F\x5C\x6B\x5C\x48\x5C\x48\x5C\x66\x5C\x6D\x5C\x45\x5C\x48\x5C\x6B\x5C\x6B\x5C\x48\x5C\x6F\x5C\x66\x5C\x44\x5C\x6C\x5C\x66\x5C\x6D\x5C\x73\x5C\x6B\x5C\x70\x5C\x69\x5C\x66\x5C\x70\x5C\x69\x5C\x45\x5C\x73\x5C\x6B\x5C\x75\x5C\x4B\x5C\x6E\x5C\x75\x5C\x48\x5C\x4B\x5C\x7A\x5C\x4B\x5C\x32\x77\x5C\x31\x61\x5C\x32\x67\x5C\x50\x5C\x32\x4A\x5C\x31\x61\x5C\x54\x5C\x6F\x5C\x4B\x5C\x31\x58\x5C\x31\x4A\x5C\x50\x5C\x34\x74\x5C\x6C\x5C\x31\x42\x5C\x6E\x5C\x31\x6E\x5C\x54\x5C\x54\x5C\x69\x5C\x31\x66\x5C\x70\x5C\x31\x4F\x5C\x7A\x5C\x31\x66\x5C\x31\x55\x5C\x31\x4C\x5C\x47\x5C\x31\x55\x5C\x31\x4B\x5C\x31\x42\x5C\x32\x70\x5C\x53\x5C\x72\x5C\x31\x79\x5C\x31\x67\x5C\x31\x6F\x5C\x31\x61\x5C\x31\x61\x5C\x31\x4B\x5C\x31\x4C\x5C\x54\x5C\x31\x6E\x5C\x57\x5C\x72\x5C\x32\x6F\x5C\x6C\x5C\x32\x6D\x5C\x31\x61\x5C\x31\x78\x5C\x7A\x5C\x53\x5C\x31\x4A\x5C\x31\x4B\x5C\x32\x65\x5C\x31\x50\x5C\x32\x65\x5C\x32\x62\x5C\x41\x5C\x69\x5C\x31\x61\x5C\x69\x5C\x31\x6C\x5C\x6E\x5C\x31\x48\x5C\x34\x68\x5C\x31\x4F\x5C\x31\x78\x5C\x31\x6B\x5C\x72\x5C\x72\x5C\x31\x67\x5C\x31\x4B\x5C\x31\x50\x5C\x48\x5C\x31\x4F\x5C\x31\x6C\x5C\x31\x78\x5C\x32\x70\x5C\x31\x55\x5C\x31\x4A\x5C\x31\x4E\x5C\x31\x4F\x5C\x31\x6B\x5C\x31\x4C\x5C\x44\x5C\x32\x6F\x5C\x31\x50\x5C\x66\x5C\x31\x71\x5C\x31\x6B\x5C\x31\x4F\x5C\x31\x4A\x5C\x34\x4B\x5C\x70\x5C\x44\x5C\x66\x5C\x31\x56\x5C\x7A\x5C\x31\x56\x5C\x31\x6C\x5C\x34\x74\x5C\x32\x62\x5C\x32\x6F\x5C\x32\x6E\x5C\x57\x5C\x31\x6E\x5C\x32\x6C\x5C\x32\x61\x5C\x75\x5C\x31\x56\x5C\x34\x4D\x5C\x31\x78\x5C\x53\x5C\x75\x5C\x31\x6C\x5C\x32\x77\x5C\x75\x5C\x54\x5C\x31\x6C\x5C\x69\x5C\x76\x5C\x31\x50\x5C\x34\x68\x5C\x57\x5C\x31\x71\x5C\x31\x55\x5C\x31\x79\x5C\x32\x6D\x5C\x31\x52\x5C\x32\x4A\x5C\x6D\x5C\x31\x4B\x5C\x31\x42\x5C\x48\x5C\x32\x6D\x5C\x70\x5C\x32\x6C\x5C\x31\x56\x5C\x31\x61\x5C\x72\x5C\x31\x4A\x5C\x31\x52\x5C\x6D\x5C\x31\x6B\x5C\x6F\x5C\x57\x5C\x32\x4A\x5C\x31\x75\x5C\x31\x4A\x5C\x4C\x5C\x32\x6C\x5C\x6C\x5C\x31\x61\x5C\x6C\x5C\x32\x64\x5C\x31\x48\x5C\x69\x5C\x6E\x5C\x31\x6E\x5C\x4C\x5C\x69\x5C\x6D\x5C\x31\x42\x5C\x31\x48\x5C\x6C\x5C\x52\x5C\x31\x61\x5C\x31\x6C\x5C\x6B\x5C\x31\x4C\x5C\x31\x4C\x5C\x41\x5C\x31\x78\x5C\x4C\x5C\x31\x67\x5C\x75\x5C\x41\x5C\x31\x48\x5C\x52\x5C\x31\x66\x5C\x32\x62\x5C\x32\x61\x5C\x52\x5C\x34\x4B\x5C\x44\x5C\x4C\x5C\x31\x75\x5C\x31\x4A\x5C\x31\x58\x5C\x31\x71\x5C\x6E\x5C\x32\x64\x5C\x53\x5C\x41\x5C\x32\x70\x5C\x32\x6E\x5C\x32\x64\x5C\x76\x5C\x48\x5C\x6C\x5C\x44\x5C\x34\x4D\x5C\x4B\x5C\x6C\x5C\x31\x6C\x5C\x31\x67\x5C\x4B\x5C\x6A\x5C\x50\x5C\x6A\x5C\x69\x5C\x6A\x5C\x6D\x5C\x45\x5C\x52\x5C\x66\x5C\x7A\x5C\x76\x22\x2C\x22\x5C\x4A\x5C\x6C\x5C\x31\x6C\x5C\x31\x67\x22\x2C\x22\x5C\x4A\x5C\x6C\x5C\x31\x6C\x5C\x32\x67\x5C\x72\x5C\x6D\x5C\x52\x22\x2C\x22\x5C\x4B\x5C\x6C\x5C\x31\x6C\x5C\x31\x67\x22\x2C\x22\x5C\x4B\x5C\x6C\x5C\x31\x6C\x5C\x32\x67\x5C\x72\x5C\x6D\x5C\x52\x22\x2C\x22\x5C\x4B\x5C\x4B\x5C\x6F\x5C\x47\x5C\x31\x6C\x5C\x45\x5C\x48\x5C\x6B\x5C\x6B\x5C\x48\x5C\x6F\x5C\x66\x5C\x44\x5C\x6C\x5C\x66\x5C\x6D\x5C\x73\x5C\x6B\x5C\x70\x5C\x69\x5C\x66\x5C\x70\x5C\x69\x5C\x45\x5C\x73\x5C\x6B\x5C\x75\x5C\x4B\x5C\x31\x6B\x5C\x31\x56\x5C\x41\x5C\x54\x5C\x32\x6D\x5C\x31\x42\x5C\x31\x71\x5C\x31\x71\x5C\x50\x5C\x50\x5C\x31\x52\x5C\x31\x61\x5C\x52\x5C\x31\x67\x5C\x54\x5C\x32\x70\x5C\x4C\x5C\x31\x4F\x5C\x31\x48\x5C\x57\x5C\x31\x4A\x5C\x44\x5C\x31\x42\x5C\x6F\x5C\x32\x62\x5C\x50\x5C\x72\x5C\x31\x4B\x5C\x32\x67\x5C\x31\x4E\x5C\x32\x67\x5C\x31\x78\x5C\x31\x79\x5C\x57\x5C\x32\x77\x5C\x32\x64\x5C\x32\x62\x5C\x31\x4C\x5C\x34\x68\x5C\x70\x5C\x7A\x5C\x31\x52\x5C\x66\x5C\x32\x6C\x5C\x32\x61\x5C\x69\x5C\x31\x48\x5C\x31\x75\x5C\x32\x4A\x5C\x31\x4C\x5C\x31\x61\x5C\x31\x4B\x5C\x32\x61\x5C\x31\x78\x5C\x31\x67\x5C\x52\x5C\x31\x4F\x5C\x47\x5C\x32\x6C\x5C\x72\x5C\x31\x75\x5C\x31\x58\x5C\x4A\x5C\x6C\x5C\x31\x6C\x5C\x31\x67\x22\x2C\x22\x5C\x4B\x5C\x4B\x5C\x6D\x5C\x66\x5C\x6C\x5C\x6B\x5C\x44\x5C\x6D\x5C\x73\x5C\x66\x5C\x6C\x5C\x45\x5C\x7A\x5C\x6F\x5C\x6B\x5C\x48\x5C\x7A\x5C\x6F\x5C\x6B\x5C\x48\x5C\x45\x5C\x73\x5C\x6B\x5C\x75\x5C\x4B\x5C\x6E\x5C\x75\x5C\x48\x5C\x4B\x5C\x7A\x5C\x6F\x5C\x6A\x5C\x70\x5C\x57\x5C\x45\x5C\x48\x5C\x6E\x5C\x53\x22\x2C\x22\x5C\x76\x5C\x7A\x5C\x69\x5C\x32\x65\x5C\x66\x5C\x70\x5C\x44\x22\x2C\x22\x5C\x31\x74\x5C\x75\x5C\x6A\x5C\x6E\x5C\x70\x5C\x72\x5C\x75\x5C\x66\x5C\x70\x5C\x44\x22\x2C\x22\x5C\x45\x5C\x6C\x5C\x66\x5C\x6A\x5C\x6D\x5C\x73\x5C\x47\x5C\x72\x5C\x69\x5C\x6B\x5C\x48\x5C\x48\x5C\x6F\x5C\x66\x22\x2C\x22\x5C\x73\x5C\x69\x5C\x6D\x5C\x6F\x5C\x32\x62\x5C\x66\x5C\x4C\x22\x2C\x22\x5C\x76\x5C\x6D\x5C\x66\x5C\x50\x5C\x66\x5C\x70\x5C\x69\x5C\x31\x52\x5C\x66\x5C\x53\x5C\x6A\x5C\x44\x5C\x6F\x5C\x69\x22\x2C\x22\x5C\x31\x74\x22\x2C\x22\x5C\x4E\x5C\x6C\x5C\x76\x5C\x6A\x5C\x70\x5C\x78\x5C\x73\x5C\x6F\x5C\x6A\x5C\x6C\x5C\x6C\x5C\x4A\x5C\x42\x5C\x69\x5C\x66\x5C\x54\x5C\x69\x5C\x42\x5C\x4F\x22\x2C\x22\x5C\x45\x5C\x6C\x5C\x6B\x5C\x73\x5C\x6E\x5C\x6A\x5C\x6F\x5C\x72\x5C\x6E\x5C\x73\x5C\x6B\x5C\x70\x5C\x6C\x5C\x78\x5C\x6A\x22\x2C\x22\x5C\x6C\x5C\x47\x5C\x6B\x5C\x6D\x5C\x69\x5C\x73\x5C\x6B\x5C\x41\x5C\x66\x22\x2C\x22\x5C\x45\x5C\x75\x5C\x6A\x5C\x6E\x5C\x6F\x5C\x73\x5C\x47\x5C\x6E\x5C\x75\x5C\x76\x5C\x72\x5C\x69\x5C\x6E\x5C\x69\x5C\x6F\x5C\x66\x22\x2C\x22\x5C\x45\x5C\x75\x5C\x6A\x5C\x6E\x5C\x6F\x5C\x73\x5C\x47\x5C\x6E\x5C\x75\x5C\x76\x5C\x72\x5C\x69\x5C\x66\x5C\x54\x5C\x69\x22\x2C\x22\x5C\x45\x5C\x32\x65\x5C\x6A\x5C\x6E\x5C\x6F\x5C\x31\x6E\x5C\x47\x5C\x6E\x5C\x75\x5C\x76\x5C\x78\x5C\x45\x5C\x52\x5C\x6E\x5C\x41\x5C\x48\x5C\x66\x5C\x69\x5C\x72\x5C\x73\x5C\x6B\x5C\x70\x5C\x69\x5C\x66\x5C\x70\x5C\x69\x22\x2C\x22\x5C\x6E\x5C\x6C\x5C\x72\x5C\x6D\x5C\x6E\x5C\x48\x5C\x47\x5C\x69\x22\x2C\x22\x5C\x6E\x5C\x6C\x5C\x72\x5C\x6F\x5C\x66\x5C\x53\x5C\x69\x22\x2C\x22\x5C\x31\x43\x5C\x73\x5C\x6B\x5C\x70\x5C\x69\x5C\x6A\x5C\x73\x5C\x69\x5C\x31\x56\x5C\x6B\x5C\x6D\x5C\x75\x5C\x31\x45\x22\x2C\x22\x5C\x4E\x5C\x41\x5C\x6E\x5C\x50\x5C\x78\x5C\x73\x5C\x6F\x5C\x6A\x5C\x6C\x5C\x6C\x5C\x4A\x5C\x42\x5C\x73\x5C\x6B\x5C\x70\x5C\x69\x5C\x6A\x5C\x73\x5C\x69\x5C\x72\x5C\x53\x5C\x6B\x5C\x6D\x5C\x75\x5C\x72\x5C\x52\x5C\x6E\x5C\x41\x5C\x48\x5C\x66\x5C\x69\x5C\x42\x5C\x4B\x5C\x4F\x22\x2C\x22\x5C\x6D\x5C\x66\x5C\x76\x5C\x6F\x5C\x6A\x5C\x73\x5C\x66\x5C\x32\x6E\x5C\x6E\x5C\x69\x5C\x47\x22\x2C\x22\x5C\x31\x74\x5C\x31\x6E\x5C\x6B\x5C\x70\x5C\x69\x5C\x6A\x5C\x73\x5C\x69\x5C\x31\x56\x5C\x6B\x5C\x6D\x5C\x75\x5C\x31\x69\x5C\x78\x5C\x53\x5C\x6B\x5C\x6D\x5C\x75\x22\x2C\x22\x5C\x45\x5C\x76\x5C\x6B\x5C\x6C\x5C\x69\x5C\x72\x5C\x7A\x5C\x6B\x5C\x41\x5C\x4C\x5C\x78\x5C\x45\x5C\x73\x5C\x6B\x5C\x70\x5C\x69\x5C\x6A\x5C\x73\x5C\x69\x5C\x72\x5C\x53\x5C\x6B\x5C\x6D\x5C\x75\x5C\x72\x5C\x52\x5C\x6E\x5C\x41\x5C\x48\x5C\x66\x5C\x69\x22\x2C\x22\x5C\x31\x43\x5C\x6F\x5C\x66\x5C\x53\x5C\x69\x5C\x31\x75\x5C\x6E\x5C\x41\x5C\x66\x5C\x7A\x5C\x6A\x5C\x6D\x5C\x31\x45\x22\x2C\x22\x5C\x31\x43\x5C\x6D\x5C\x6E\x5C\x48\x5C\x47\x5C\x69\x5C\x31\x75\x5C\x6E\x5C\x41\x5C\x66\x5C\x7A\x5C\x6A\x5C\x6D\x5C\x31\x45\x22\x2C\x22\x5C\x31\x43\x5C\x53\x5C\x44\x5C\x6F\x5C\x6F\x5C\x32\x6E\x5C\x6E\x5C\x41\x5C\x69\x5C\x47\x5C\x31\x45\x22\x2C\x22\x5C\x70\x5C\x6B\x5C\x72\x5C\x6C\x5C\x6E\x5C\x41\x5C\x66\x5C\x7A\x5C\x6A\x5C\x6D\x22\x2C\x22\x5C\x6C\x5C\x47\x5C\x73\x22\x2C\x22\x5C\x73\x5C\x6F\x5C\x6C\x22\x2C\x22\x5C\x45\x5C\x76\x5C\x6B\x5C\x6C\x5C\x69\x5C\x72\x5C\x7A\x5C\x6B\x5C\x41\x5C\x4C\x5C\x78\x5C\x7A\x22\x2C\x22\x5C\x48\x5C\x66\x5C\x69\x5C\x31\x50\x5C\x44\x5C\x69\x5C\x69\x5C\x6B\x5C\x70\x22\x2C\x22\x5C\x4E\x5C\x66\x5C\x75\x5C\x4F\x5C\x32\x43\x5C\x31\x69\x5C\x4E\x5C\x4B\x5C\x66\x5C\x75\x5C\x4F\x22\x2C\x22\x5C\x6D\x5C\x66\x5C\x76\x5C\x6F\x5C\x6A\x5C\x73\x5C\x66\x5C\x31\x6F\x5C\x66\x5C\x54\x5C\x69\x22\x2C\x22\x5C\x33\x4A\x5C\x6C\x22\x2C\x22\x5C\x66\x5C\x75\x22\x2C\x22\x5C\x6E\x5C\x73\x5C\x6B\x5C\x70\x22\x2C\x22\x5C\x73\x5C\x6B\x5C\x6F\x5C\x6B\x5C\x6D\x22\x2C\x22\x5C\x6C\x5C\x6E\x5C\x31\x6B\x5C\x66\x22\x2C\x22\x5C\x6E\x5C\x70\x5C\x53\x5C\x6B\x22\x2C\x22\x5C\x7A\x5C\x44\x5C\x69\x5C\x69\x5C\x6B\x5C\x70\x5C\x78\x5C\x7A\x5C\x69\x5C\x70\x5C\x78\x5C\x54\x5C\x31\x61\x22\x2C\x22\x5C\x7A\x5C\x44\x5C\x69\x5C\x69\x5C\x6B\x5C\x70\x5C\x78\x5C\x7A\x5C\x69\x5C\x70\x22\x2C\x22\x5C\x7A\x5C\x6A\x5C\x73\x5C\x57\x5C\x48\x5C\x6D\x5C\x6B\x5C\x44\x5C\x70\x5C\x41\x5C\x31\x62\x22\x2C\x22\x5C\x31\x65\x22\x2C\x22\x5C\x73\x5C\x66\x5C\x70\x5C\x69\x5C\x66\x5C\x6D\x22\x2C\x22\x5C\x6E\x5C\x6C\x5C\x72\x5C\x73\x22\x2C\x22\x5C\x54\x5C\x31\x61\x5C\x78\x22\x2C\x22\x5C\x54\x5C\x31\x61\x22\x2C\x22\x5C\x4E\x5C\x6C\x5C\x76\x5C\x6A\x5C\x70\x5C\x78\x5C\x73\x5C\x6F\x5C\x6A\x5C\x6C\x5C\x6C\x5C\x4A\x5C\x42\x5C\x7A\x5C\x69\x5C\x70\x5C\x72\x5C\x6E\x5C\x70\x5C\x53\x5C\x6B\x5C\x42\x5C\x4F\x22\x2C\x22\x5C\x45\x5C\x76\x5C\x6B\x5C\x6C\x5C\x69\x5C\x72\x5C\x7A\x5C\x6B\x5C\x41\x5C\x4C\x5C\x78\x5C\x6A\x22\x2C\x22\x5C\x31\x43\x5C\x6A\x5C\x6F\x5C\x66\x5C\x6D\x5C\x69\x5C\x31\x75\x5C\x44\x5C\x73\x5C\x73\x5C\x66\x5C\x6C\x5C\x6C\x5C\x31\x45\x22\x2C\x22\x5C\x6C\x5C\x44\x5C\x73\x5C\x73\x5C\x66\x5C\x6C\x5C\x6C\x22\x2C\x22\x5C\x31\x43\x5C\x6A\x5C\x6F\x5C\x66\x5C\x6D\x5C\x69\x5C\x32\x6F\x5C\x70\x5C\x53\x5C\x6B\x5C\x31\x45\x22\x2C\x22\x5C\x31\x43\x5C\x6A\x5C\x6F\x5C\x66\x5C\x6D\x5C\x69\x5C\x32\x6E\x5C\x6A\x5C\x6D\x5C\x70\x5C\x6E\x5C\x70\x5C\x48\x5C\x31\x45\x22\x2C\x22\x5C\x52\x5C\x6A\x5C\x6D\x5C\x70\x5C\x6E\x5C\x70\x5C\x48\x22\x2C\x22\x5C\x31\x43\x5C\x6A\x5C\x6F\x5C\x66\x5C\x6D\x5C\x69\x5C\x31\x42\x5C\x6D\x5C\x6D\x5C\x6B\x5C\x6D\x5C\x31\x45\x22\x2C\x22\x5C\x66\x5C\x6D\x5C\x6D\x5C\x6B\x5C\x6D\x22\x2C\x22\x5C\x31\x43\x5C\x73\x5C\x6B\x5C\x41\x5C\x66\x5C\x31\x50\x5C\x6B\x5C\x54\x5C\x31\x45\x22\x2C\x22\x5C\x73\x5C\x6B\x5C\x41\x5C\x66\x22\x2C\x22\x5C\x4E\x5C\x41\x5C\x6E\x5C\x50\x5C\x78\x5C\x73\x5C\x6F\x5C\x6A\x5C\x6C\x5C\x6C\x5C\x4A\x5C\x42\x5C\x6A\x5C\x6F\x5C\x66\x5C\x6D\x5C\x69\x5C\x72\x5C\x75\x5C\x66\x5C\x6C\x5C\x6C\x5C\x6A\x5C\x48\x5C\x66\x5C\x78\x5C\x6A\x5C\x6F\x5C\x66\x5C\x6D\x5C\x69\x5C\x72\x22\x2C\x22\x5C\x4E\x5C\x76\x5C\x6D\x5C\x66\x5C\x78\x5C\x73\x5C\x6F\x5C\x6A\x5C\x6C\x5C\x6C\x5C\x4A\x5C\x42\x5C\x73\x5C\x6B\x5C\x41\x5C\x66\x5C\x72\x5C\x7A\x5C\x6B\x5C\x54\x5C\x42\x5C\x4F\x22\x2C\x22\x5C\x4E\x5C\x4B\x5C\x76\x5C\x6D\x5C\x66\x5C\x4F\x22\x2C\x22\x5C\x45\x5C\x76\x5C\x6B\x5C\x6C\x5C\x69\x5C\x72\x5C\x7A\x5C\x6B\x5C\x41\x5C\x4C\x5C\x78\x5C\x7A\x5C\x6F\x5C\x6B\x5C\x73\x5C\x57\x5C\x31\x78\x5C\x44\x5C\x6B\x5C\x69\x5C\x66\x22\x2C\x22\x5C\x31\x4E\x5C\x7A\x5C\x6F\x5C\x6A\x5C\x70\x5C\x57\x22\x2C\x22\x5C\x6C\x5C\x73\x5C\x6D\x5C\x6B\x5C\x6F\x5C\x6F\x5C\x7A\x5C\x6A\x5C\x6D\x5C\x6C\x5C\x4A\x5C\x4C\x5C\x66\x5C\x6C\x5C\x31\x77\x5C\x6D\x5C\x66\x5C\x6C\x5C\x6E\x5C\x31\x6B\x5C\x6A\x5C\x7A\x5C\x6F\x5C\x66\x5C\x4A\x5C\x4C\x5C\x66\x5C\x6C\x5C\x31\x77\x5C\x69\x5C\x6B\x5C\x6B\x5C\x6F\x5C\x7A\x5C\x6A\x5C\x6D\x5C\x4A\x5C\x31\x66\x5C\x31\x77\x5C\x52\x5C\x6E\x5C\x41\x5C\x69\x5C\x47\x5C\x4A\x5C\x31\x4C\x5C\x31\x4F\x5C\x31\x66\x5C\x31\x77\x5C\x47\x5C\x66\x5C\x6E\x5C\x48\x5C\x47\x5C\x69\x5C\x4A\x5C\x31\x67\x5C\x31\x55\x5C\x31\x66\x5C\x31\x77\x5C\x69\x5C\x6B\x5C\x76\x5C\x4A\x5C\x31\x67\x5C\x31\x66\x5C\x31\x77\x5C\x6F\x5C\x66\x5C\x53\x5C\x69\x5C\x4A\x5C\x31\x67\x5C\x31\x66\x22\x2C\x22\x5C\x45\x5C\x76\x5C\x7A\x5C\x69\x5C\x72\x5C\x52\x5C\x6B\x22\x2C\x22\x5C\x6E\x5C\x6C\x5C\x32\x61\x5C\x6B\x5C\x6C\x5C\x69\x22\x2C\x22\x5C\x45\x5C\x76\x5C\x6B\x5C\x6C\x5C\x69\x5C\x72\x5C\x6C\x5C\x47\x5C\x6A\x5C\x6D\x5C\x66\x5C\x78\x5C\x45\x5C\x6C\x5C\x47\x5C\x6B\x5C\x52\x5C\x72\x5C\x75\x5C\x6B\x5C\x6D\x5C\x66\x5C\x78\x5C\x45\x5C\x7A\x5C\x69\x5C\x70\x5C\x31\x77\x5C\x78\x5C\x45\x5C\x6C\x5C\x47\x5C\x6A\x5C\x6D\x5C\x66\x5C\x72\x5C\x69\x5C\x6B\x5C\x48\x5C\x48\x5C\x6F\x5C\x66\x22\x2C\x22\x5C\x6E\x5C\x70\x5C\x76\x5C\x44\x5C\x69\x22\x2C\x22\x5C\x73\x5C\x47\x5C\x6E\x5C\x6F\x5C\x41\x5C\x6D\x5C\x66\x5C\x70\x22\x2C\x22\x5C\x6C\x5C\x66\x5C\x6F\x5C\x66\x5C\x73\x5C\x69\x22\x2C\x22\x5C\x52\x5C\x6D\x5C\x6E\x5C\x69\x5C\x66\x5C\x31\x6F\x5C\x66\x5C\x54\x5C\x69\x22\x2C\x22\x5C\x73\x5C\x6F\x5C\x6E\x5C\x76\x5C\x7A\x5C\x6B\x5C\x6A\x5C\x6D\x5C\x41\x22\x2C\x22\x5C\x73\x5C\x6B\x5C\x76\x5C\x6E\x5C\x66\x5C\x41\x22\x2C\x22\x5C\x73\x5C\x6B\x5C\x76\x5C\x6E\x5C\x66\x5C\x41\x5C\x72\x5C\x6B\x5C\x53\x5C\x53\x22\x2C\x22\x5C\x7A\x5C\x44\x5C\x69\x5C\x69\x5C\x6B\x5C\x70\x22\x2C\x22\x5C\x45\x5C\x73\x5C\x6B\x5C\x76\x5C\x4C\x5C\x72\x5C\x6F\x5C\x6E\x5C\x70\x5C\x57\x22\x2C\x22\x5C\x6A\x22\x2C\x22\x5C\x66\x5C\x54\x5C\x69\x5C\x66\x5C\x6D\x5C\x70\x5C\x6A\x5C\x6F\x5C\x72\x5C\x6F\x5C\x6E\x5C\x70\x5C\x57\x22\x2C\x22\x5C\x52\x5C\x66\x5C\x7A\x5C\x6C\x5C\x6E\x5C\x69\x5C\x66\x22\x2C\x22\x5C\x4E\x5C\x6F\x5C\x6E\x5C\x78\x5C\x73\x5C\x6F\x5C\x6A\x5C\x6C\x5C\x6C\x5C\x4A\x5C\x42\x22\x2C\x22\x5C\x42\x5C\x4F\x5C\x4E\x5C\x6A\x5C\x78\x5C\x73\x5C\x6F\x5C\x6A\x5C\x6C\x5C\x6C\x5C\x4A\x5C\x42\x5C\x7A\x5C\x6E\x5C\x72\x22\x2C\x22\x5C\x42\x5C\x78\x5C\x6D\x5C\x66\x5C\x6F\x5C\x4A\x5C\x42\x5C\x70\x5C\x6B\x5C\x53\x5C\x6B\x5C\x6F\x5C\x6F\x5C\x6B\x5C\x52\x5C\x78\x5C\x70\x5C\x6B\x5C\x6B\x5C\x76\x5C\x66\x5C\x70\x5C\x66\x5C\x6D\x5C\x42\x5C\x78\x5C\x69\x5C\x6A\x5C\x6D\x5C\x48\x5C\x66\x5C\x69\x5C\x4A\x5C\x42\x5C\x31\x4E\x5C\x7A\x5C\x6F\x5C\x6A\x5C\x70\x5C\x57\x5C\x42\x5C\x4F\x5C\x4E\x5C\x4B\x5C\x6A\x5C\x4F\x5C\x4E\x5C\x4B\x5C\x6F\x5C\x6E\x5C\x4F\x22\x2C\x22\x5C\x4E\x5C\x44\x5C\x6F\x5C\x78\x5C\x73\x5C\x6F\x5C\x6A\x5C\x6C\x5C\x6C\x5C\x4A\x5C\x42\x5C\x6A\x5C\x44\x5C\x69\x5C\x47\x5C\x6B\x5C\x6D\x5C\x72\x5C\x6F\x5C\x6E\x5C\x70\x5C\x57\x5C\x6C\x5C\x78\x5C\x6C\x5C\x6B\x5C\x73\x5C\x6E\x5C\x6A\x5C\x6F\x5C\x78\x5C\x73\x5C\x6B\x5C\x6F\x5C\x6B\x5C\x6D\x5C\x42\x5C\x4F\x5C\x4E\x5C\x4B\x5C\x44\x5C\x6F\x5C\x4F\x22\x2C\x22\x5C\x45\x5C\x6A\x5C\x44\x5C\x69\x5C\x47\x5C\x6B\x5C\x6D\x5C\x72\x5C\x6F\x5C\x6E\x5C\x70\x5C\x57\x5C\x6C\x22\x2C\x22\x5C\x6A\x5C\x76\x5C\x76\x5C\x66\x5C\x70\x5C\x41\x5C\x31\x6F\x5C\x6B\x22\x2C\x22\x5C\x6F\x5C\x6E\x22\x2C\x22\x5C\x45\x5C\x6A\x5C\x7A\x5C\x6B\x5C\x44\x5C\x69\x5C\x72\x5C\x6A\x5C\x44\x5C\x69\x5C\x47\x5C\x6B\x5C\x6D\x5C\x78\x5C\x45\x5C\x6A\x5C\x44\x5C\x69\x5C\x47\x5C\x6B\x5C\x6D\x5C\x72\x5C\x69\x5C\x66\x5C\x54\x5C\x69\x22\x2C\x22\x5C\x6E\x5C\x6C\x5C\x32\x77\x5C\x31\x6F\x5C\x31\x79\x22\x2C\x22\x5C\x45\x5C\x76\x5C\x6B\x5C\x6C\x5C\x69\x5C\x72\x5C\x70\x5C\x6A\x5C\x50\x5C\x72\x5C\x6B\x5C\x6F\x5C\x41\x5C\x66\x5C\x6D\x5C\x72\x5C\x6F\x5C\x6E\x5C\x70\x5C\x57\x22\x2C\x22\x5C\x45\x5C\x76\x5C\x6B\x5C\x6C\x5C\x69\x5C\x72\x5C\x70\x5C\x6A\x5C\x50\x5C\x72\x5C\x70\x5C\x66\x5C\x52\x5C\x66\x5C\x6D\x5C\x72\x5C\x6F\x5C\x6E\x5C\x70\x5C\x57\x22\x2C\x22\x5C\x45\x5C\x75\x5C\x6A\x5C\x6E\x5C\x70\x5C\x72\x5C\x6C\x5C\x66\x5C\x6A\x5C\x6D\x5C\x73\x5C\x47\x22\x2C\x22\x5C\x45\x5C\x6D\x5C\x66\x5C\x6F\x5C\x6A\x5C\x69\x5C\x66\x5C\x41\x5C\x72\x5C\x69\x5C\x6A\x5C\x48\x22\x2C\x22\x5C\x45\x5C\x52\x5C\x6E\x5C\x41\x5C\x48\x5C\x66\x5C\x69\x5C\x72\x5C\x73\x5C\x6B\x5C\x70\x5C\x69\x5C\x66\x5C\x70\x5C\x69\x22\x2C\x22\x5C\x6D\x5C\x66\x5C\x6C\x5C\x44\x5C\x6F\x5C\x69\x5C\x6C\x22\x2C\x22\x5C\x45\x5C\x69\x5C\x6E\x5C\x69\x5C\x6F\x5C\x66\x5C\x72\x5C\x6F\x5C\x6E\x5C\x70\x5C\x57\x22\x2C\x22\x5C\x45\x5C\x6D\x5C\x66\x5C\x6F\x5C\x6A\x5C\x69\x5C\x66\x5C\x41\x5C\x72\x5C\x52\x5C\x6D\x5C\x6A\x5C\x76\x22\x2C\x22\x5C\x31\x74\x5C\x6D\x5C\x66\x5C\x6F\x5C\x6A\x5C\x69\x5C\x66\x5C\x41\x5C\x72\x5C\x76\x5C\x6B\x5C\x6C\x5C\x69\x5C\x6C\x5C\x78\x5C\x45\x5C\x32\x70\x5C\x31\x6F\x5C\x32\x65\x5C\x31\x79\x22\x2C\x22\x5C\x7A\x5C\x6F\x5C\x6B\x5C\x48\x5C\x48\x5C\x66\x5C\x6D\x5C\x72\x5C\x73\x5C\x6B\x5C\x75\x5C\x75\x5C\x66\x5C\x70\x5C\x69\x5C\x6C\x5C\x78\x5C\x50\x5C\x6E\x5C\x6C\x5C\x6E\x5C\x7A\x5C\x6F\x5C\x66\x22\x2C\x22\x5C\x7A\x5C\x69\x5C\x70\x22\x2C\x22\x5C\x31\x74\x5C\x69\x5C\x6B\x5C\x76\x5C\x72\x5C\x73\x5C\x6B\x5C\x70\x5C\x69\x5C\x6E\x5C\x70\x5C\x44\x5C\x66\x5C\x78\x5C\x45\x5C\x73\x5C\x6B\x5C\x75\x5C\x75\x5C\x66\x5C\x70\x5C\x69\x5C\x72\x5C\x6D\x5C\x66\x5C\x76\x5C\x6F\x5C\x4C\x22\x2C\x22\x5C\x45\x5C\x6A\x5C\x50\x5C\x6A\x5C\x69\x5C\x6A\x5C\x6D\x5C\x72\x5C\x6E\x5C\x75\x5C\x6A\x5C\x48\x5C\x66\x5C\x72\x5C\x73\x5C\x6B\x5C\x70\x5C\x69\x5C\x6A\x5C\x6E\x5C\x70\x5C\x66\x5C\x6D\x5C\x78\x5C\x6E\x5C\x75\x5C\x48\x22\x2C\x22\x5C\x45\x5C\x73\x5C\x6B\x5C\x75\x5C\x75\x5C\x66\x5C\x70\x5C\x69\x5C\x6C\x5C\x78\x5C\x45\x5C\x73\x5C\x6B\x5C\x75\x5C\x75\x5C\x66\x5C\x70\x5C\x69\x5C\x72\x5C\x6D\x5C\x66\x5C\x76\x5C\x6F\x5C\x4C\x22\x2C\x22\x5C\x45\x5C\x73\x5C\x6B\x5C\x75\x5C\x75\x5C\x66\x5C\x70\x5C\x69\x5C\x6C\x5C\x78\x5C\x31\x74\x5C\x69\x5C\x6B\x5C\x76\x5C\x72\x5C\x73\x5C\x6B\x5C\x70\x5C\x69\x5C\x6E\x5C\x70\x5C\x44\x5C\x66\x22\x2C\x22\x5C\x45\x5C\x6C\x5C\x47\x5C\x6B\x5C\x52\x5C\x72\x5C\x73\x5C\x53\x22\x2C\x22\x5C\x73\x5C\x53\x5C\x72\x5C\x6B\x5C\x70\x22\x2C\x22\x5C\x6C\x5C\x47\x5C\x6B\x5C\x52\x22\x2C\x22\x5C\x47\x5C\x6E\x5C\x41\x5C\x66\x22\x2C\x22\x5C\x45\x5C\x75\x5C\x6A\x5C\x6E\x5C\x70\x5C\x72\x5C\x52\x5C\x6D\x5C\x6A\x5C\x76\x5C\x31\x77\x5C\x78\x5C\x45\x5C\x6C\x5C\x6E\x5C\x41\x5C\x66\x5C\x7A\x5C\x6A\x5C\x6D\x5C\x72\x5C\x52\x5C\x6D\x5C\x6A\x5C\x76\x22\x2C\x22\x5C\x45\x5C\x7A\x5C\x6F\x5C\x6B\x5C\x48\x5C\x72\x5C\x76\x5C\x6B\x5C\x6C\x5C\x69\x5C\x72\x5C\x73\x5C\x6B\x5C\x75\x5C\x75\x5C\x66\x5C\x70\x5C\x69\x5C\x6C\x22\x2C\x22\x5C\x50\x5C\x6E\x5C\x6C\x5C\x6E\x5C\x7A\x5C\x6E\x5C\x6F\x5C\x6E\x5C\x69\x5C\x4C\x5C\x31\x62\x5C\x50\x5C\x6E\x5C\x6C\x5C\x6E\x5C\x7A\x5C\x6F\x5C\x66\x5C\x31\x6A\x5C\x6E\x5C\x75\x5C\x76\x5C\x6B\x5C\x6D\x5C\x69\x5C\x6A\x5C\x70\x5C\x69\x5C\x31\x65\x5C\x6B\x5C\x76\x5C\x6A\x5C\x73\x5C\x6E\x5C\x69\x5C\x4C\x5C\x31\x62\x5C\x31\x69\x5C\x31\x6A\x5C\x6E\x5C\x75\x5C\x76\x5C\x6B\x5C\x6D\x5C\x69\x5C\x6A\x5C\x70\x5C\x69\x5C\x31\x65\x5C\x76\x5C\x6B\x5C\x6C\x5C\x6E\x5C\x69\x5C\x6E\x5C\x6B\x5C\x70\x5C\x31\x62\x5C\x6D\x5C\x66\x5C\x6F\x5C\x6A\x5C\x69\x5C\x6E\x5C\x50\x5C\x66\x5C\x31\x6A\x5C\x6E\x5C\x75\x5C\x76\x5C\x6B\x5C\x6D\x5C\x69\x5C\x6A\x5C\x70\x5C\x69\x5C\x31\x65\x5C\x31\x6B\x5C\x72\x5C\x6E\x5C\x70\x5C\x41\x5C\x66\x5C\x54\x5C\x31\x62\x5C\x31\x69\x5C\x31\x6A\x5C\x6E\x5C\x75\x5C\x76\x5C\x6B\x5C\x6D\x5C\x69\x5C\x6A\x5C\x70\x5C\x69\x5C\x31\x65\x5C\x53\x5C\x6B\x5C\x70\x5C\x69\x5C\x72\x5C\x6C\x5C\x6E\x5C\x31\x6B\x5C\x66\x5C\x31\x62\x5C\x31\x69\x5C\x31\x55\x5C\x76\x5C\x54\x5C\x31\x6A\x5C\x6E\x5C\x75\x5C\x76\x5C\x6B\x5C\x6D\x5C\x69\x5C\x6A\x5C\x70\x5C\x69\x5C\x31\x65\x5C\x73\x5C\x6B\x5C\x6F\x5C\x6B\x5C\x6D\x5C\x31\x62\x5C\x50\x5C\x6A\x5C\x6D\x5C\x34\x6E\x5C\x72\x5C\x72\x5C\x53\x5C\x6B\x5C\x6B\x5C\x69\x5C\x66\x5C\x6D\x5C\x7A\x5C\x6A\x5C\x6D\x5C\x72\x5C\x73\x5C\x6B\x5C\x6F\x5C\x6B\x5C\x6D\x5C\x34\x65\x5C\x31\x6A\x5C\x6E\x5C\x75\x5C\x76\x5C\x6B\x5C\x6D\x5C\x69\x5C\x6A\x5C\x70\x5C\x69\x5C\x31\x65\x5C\x75\x5C\x6A\x5C\x6D\x5C\x48\x5C\x6E\x5C\x70\x5C\x31\x62\x5C\x31\x66\x5C\x31\x6A\x5C\x6E\x5C\x75\x5C\x76\x5C\x6B\x5C\x6D\x5C\x69\x5C\x6A\x5C\x70\x5C\x69\x5C\x31\x65\x5C\x69\x5C\x66\x5C\x54\x5C\x69\x5C\x72\x5C\x6E\x5C\x70\x5C\x41\x5C\x66\x5C\x70\x5C\x69\x5C\x31\x62\x5C\x31\x66\x5C\x31\x6A\x5C\x6E\x5C\x75\x5C\x76\x5C\x6B\x5C\x6D\x5C\x69\x5C\x6A\x5C\x70\x5C\x69\x5C\x31\x65\x22\x2C\x22\x5C\x50\x5C\x6E\x5C\x6C\x5C\x6E\x5C\x7A\x5C\x6E\x5C\x6F\x5C\x6E\x5C\x69\x5C\x4C\x5C\x31\x62\x5C\x50\x5C\x6E\x5C\x6C\x5C\x6E\x5C\x7A\x5C\x6F\x5C\x66\x5C\x31\x6A\x5C\x6E\x5C\x75\x5C\x76\x5C\x6B\x5C\x6D\x5C\x69\x5C\x6A\x5C\x70\x5C\x69\x5C\x31\x65\x5C\x6B\x5C\x76\x5C\x6A\x5C\x73\x5C\x6E\x5C\x69\x5C\x4C\x5C\x31\x62\x5C\x31\x69\x5C\x31\x6A\x5C\x6E\x5C\x75\x5C\x76\x5C\x6B\x5C\x6D\x5C\x69\x5C\x6A\x5C\x70\x5C\x69\x5C\x31\x65\x5C\x76\x5C\x6B\x5C\x6C\x5C\x6E\x5C\x69\x5C\x6E\x5C\x6B\x5C\x70\x5C\x31\x62\x5C\x6D\x5C\x66\x5C\x6F\x5C\x6A\x5C\x69\x5C\x6E\x5C\x50\x5C\x66\x5C\x31\x6A\x5C\x6E\x5C\x75\x5C\x76\x5C\x6B\x5C\x6D\x5C\x69\x5C\x6A\x5C\x70\x5C\x69\x5C\x31\x65\x5C\x31\x6B\x5C\x72\x5C\x6E\x5C\x70\x5C\x41\x5C\x66\x5C\x54\x5C\x31\x62\x5C\x31\x69\x5C\x31\x6A\x5C\x6E\x5C\x75\x5C\x76\x5C\x6B\x5C\x6D\x5C\x69\x5C\x6A\x5C\x70\x5C\x69\x5C\x31\x65\x5C\x53\x5C\x6B\x5C\x70\x5C\x69\x5C\x72\x5C\x6C\x5C\x6E\x5C\x31\x6B\x5C\x66\x5C\x31\x62\x5C\x31\x69\x5C\x31\x55\x5C\x76\x5C\x54\x5C\x31\x6A\x5C\x6E\x5C\x75\x5C\x76\x5C\x6B\x5C\x6D\x5C\x69\x5C\x6A\x5C\x70\x5C\x69\x5C\x31\x65\x5C\x73\x5C\x6B\x5C\x6F\x5C\x6B\x5C\x6D\x5C\x31\x62\x5C\x50\x5C\x6A\x5C\x6D\x5C\x34\x6E\x5C\x72\x5C\x72\x5C\x6A\x5C\x73\x5C\x73\x5C\x66\x5C\x70\x5C\x69\x5C\x72\x5C\x73\x5C\x6B\x5C\x6F\x5C\x6B\x5C\x6D\x5C\x34\x65\x5C\x31\x6A\x5C\x6E\x5C\x75\x5C\x76\x5C\x6B\x5C\x6D\x5C\x69\x5C\x6A\x5C\x70\x5C\x69\x5C\x31\x65\x5C\x75\x5C\x6A\x5C\x6D\x5C\x48\x5C\x6E\x5C\x70\x5C\x31\x62\x5C\x31\x66\x5C\x31\x6A\x5C\x6E\x5C\x75\x5C\x76\x5C\x6B\x5C\x6D\x5C\x69\x5C\x6A\x5C\x70\x5C\x69\x5C\x31\x65\x5C\x69\x5C\x66\x5C\x54\x5C\x69\x5C\x72\x5C\x6E\x5C\x70\x5C\x41\x5C\x66\x5C\x70\x5C\x69\x5C\x31\x62\x5C\x31\x66\x5C\x31\x6A\x5C\x6E\x5C\x75\x5C\x76\x5C\x6B\x5C\x6D\x5C\x69\x5C\x6A\x5C\x70\x5C\x69\x5C\x31\x65\x22\x2C\x22\x5C\x32\x61\x5C\x6D\x5C\x66\x5C\x75\x5C\x6E\x5C\x44\x5C\x75\x5C\x78\x5C\x31\x50\x5C\x6F\x5C\x6B\x5C\x48\x5C\x48\x5C\x66\x5C\x6D\x5C\x78\x5C\x31\x6F\x5C\x66\x5C\x75\x5C\x76\x5C\x6F\x5C\x6A\x5C\x69\x5C\x66\x5C\x6C\x22\x2C\x22\x5C\x47\x5C\x69\x5C\x69\x5C\x76\x5C\x6C\x5C\x31\x62\x5C\x4B\x5C\x4B\x5C\x76\x5C\x6D\x5C\x6B\x5C\x7A\x5C\x6F\x5C\x6B\x5C\x48\x5C\x48\x5C\x66\x5C\x6D\x5C\x69\x5C\x66\x5C\x75\x5C\x76\x5C\x6F\x5C\x6A\x5C\x69\x5C\x66\x5C\x6C\x5C\x45\x5C\x73\x5C\x6B\x5C\x75\x5C\x4B\x22\x2C\x22\x5C\x6A\x5C\x31\x74\x5C\x76\x5C\x6D\x5C\x6B\x5C\x7A\x5C\x69\x5C\x66\x5C\x75\x5C\x76\x5C\x6F\x5C\x6A\x5C\x69\x5C\x66\x5C\x6C\x22\x2C\x22\x5C\x6A\x5C\x31\x74\x5C\x76\x5C\x6D\x5C\x6B\x5C\x7A\x5C\x69\x5C\x66\x5C\x75\x5C\x76\x5C\x6F\x5C\x6A\x5C\x69\x5C\x66\x5C\x6C\x5C\x31\x62\x5C\x50\x5C\x6E\x5C\x6C\x5C\x6E\x5C\x7A\x5C\x6F\x5C\x66\x22\x2C\x22\x5C\x6F\x5C\x6B\x5C\x73\x5C\x6A\x5C\x69\x5C\x6E\x5C\x6B\x5C\x70\x22\x2C\x22\x5C\x45\x5C\x76\x5C\x7A\x5C\x69\x5C\x72\x5C\x6F\x5C\x6A\x5C\x31\x6B\x5C\x4C\x22\x2C\x22\x5C\x70\x5C\x6B\x5C\x69\x22\x2C\x22\x5C\x45\x5C\x66\x5C\x70\x5C\x69\x5C\x6D\x5C\x4C\x5C\x72\x5C\x69\x5C\x47\x5C\x44\x5C\x75\x5C\x7A\x5C\x70\x5C\x6A\x5C\x6E\x5C\x6F\x5C\x78\x5C\x45\x5C\x69\x5C\x47\x5C\x44\x5C\x75\x5C\x7A\x5C\x70\x5C\x6A\x5C\x6E\x5C\x6F\x5C\x31\x77\x5C\x78\x5C\x45\x5C\x66\x5C\x70\x5C\x69\x5C\x6D\x5C\x4C\x5C\x72\x5C\x6A\x5C\x50\x5C\x6A\x5C\x69\x5C\x6A\x5C\x6D\x5C\x78\x5C\x45\x5C\x6A\x5C\x50\x5C\x6A\x5C\x69\x5C\x6A\x5C\x6D\x22\x2C\x22\x5C\x45\x5C\x75\x5C\x6A\x5C\x6E\x5C\x70\x5C\x72\x5C\x47\x5C\x66\x5C\x6A\x5C\x41\x5C\x66\x5C\x6D\x22\x2C\x22\x5C\x6E\x5C\x6C\x5C\x72\x5C\x53\x5C\x6E\x5C\x54\x5C\x66\x5C\x41\x22\x2C\x22\x5C\x73\x5C\x6F\x5C\x6B\x5C\x70\x5C\x66\x22\x2C\x22\x5C\x45\x5C\x75\x5C\x6A\x5C\x6E\x5C\x70\x5C\x72\x5C\x6F\x5C\x6B\x5C\x48\x5C\x6B\x5C\x78\x5C\x6A\x22\x2C\x22\x5C\x47\x5C\x31\x69\x22\x2C\x22\x5C\x45\x5C\x75\x5C\x6B\x5C\x7A\x5C\x6E\x5C\x6F\x5C\x66\x5C\x72\x5C\x6F\x5C\x6B\x5C\x48\x5C\x6B\x22\x2C\x22\x5C\x45\x5C\x75\x5C\x6A\x5C\x6E\x5C\x70\x5C\x72\x5C\x70\x5C\x6A\x5C\x50\x22\x2C\x22\x5C\x75\x5C\x6B\x5C\x7A\x5C\x6E\x5C\x6F\x5C\x66\x5C\x72\x5C\x70\x5C\x6A\x5C\x50\x22\x2C\x22\x5C\x73\x5C\x6F\x5C\x6A\x5C\x6C\x5C\x6C\x22\x2C\x22\x5C\x75\x5C\x66\x5C\x70\x5C\x44\x5C\x72\x5C\x6B\x5C\x70\x22\x2C\x22\x5C\x69\x5C\x6B\x5C\x48\x5C\x48\x5C\x6F\x5C\x66\x5C\x31\x6E\x5C\x6F\x5C\x6A\x5C\x6C\x5C\x6C\x22\x2C\x22\x5C\x45\x5C\x75\x5C\x66\x5C\x70\x5C\x44\x5C\x72\x5C\x6B\x5C\x70\x5C\x78\x5C\x45\x5C\x6B\x5C\x50\x5C\x66\x5C\x6D\x5C\x6F\x5C\x6A\x5C\x4C\x5C\x72\x5C\x7A\x5C\x48\x22\x2C\x22\x5C\x45\x5C\x75\x5C\x6B\x5C\x7A\x5C\x6E\x5C\x6F\x5C\x66\x5C\x72\x5C\x75\x5C\x66\x5C\x70\x5C\x44\x5C\x72\x5C\x69\x5C\x6B\x5C\x48\x5C\x48\x5C\x6F\x5C\x66\x5C\x31\x77\x5C\x78\x5C\x45\x5C\x47\x5C\x6E\x5C\x41\x5C\x66\x5C\x72\x5C\x75\x5C\x6B\x5C\x7A\x5C\x6E\x5C\x6F\x5C\x66\x5C\x72\x5C\x75\x5C\x66\x5C\x70\x5C\x44\x22\x2C\x22\x5C\x66\x5C\x54\x5C\x76\x5C\x6A\x5C\x70\x5C\x41\x5C\x66\x5C\x41\x22\x2C\x22\x5C\x47\x5C\x6A\x5C\x6C\x5C\x31\x6E\x5C\x6F\x5C\x6A\x5C\x6C\x5C\x6C\x22\x2C\x22\x5C\x6C\x5C\x6F\x5C\x6E\x5C\x41\x5C\x66\x5C\x31\x6F\x5C\x6B\x5C\x48\x5C\x48\x5C\x6F\x5C\x66\x22\x2C\x22\x5C\x45\x5C\x6C\x5C\x44\x5C\x7A\x5C\x72\x5C\x75\x5C\x66\x5C\x70\x5C\x44\x22\x2C\x22\x5C\x45\x5C\x75\x5C\x6B\x5C\x7A\x5C\x6E\x5C\x6F\x5C\x66\x5C\x72\x5C\x75\x5C\x66\x5C\x70\x5C\x44\x5C\x78\x5C\x45\x5C\x47\x5C\x6A\x5C\x6C\x5C\x72\x5C\x6C\x5C\x44\x5C\x7A\x5C\x78\x5C\x4F\x5C\x78\x5C\x6A\x22\x2C\x22\x5C\x31\x74\x5C\x75\x5C\x6B\x5C\x7A\x5C\x6E\x5C\x6F\x5C\x66\x5C\x72\x5C\x75\x5C\x66\x5C\x70\x5C\x44\x22\x2C\x22\x5C\x45\x5C\x6A\x5C\x7A\x5C\x6B\x5C\x44\x5C\x69\x5C\x72\x5C\x6C\x5C\x66\x5C\x73\x5C\x69\x5C\x6E\x5C\x6B\x5C\x70\x5C\x78\x5C\x45\x5C\x31\x79\x5C\x6E\x5C\x70\x5C\x57\x5C\x31\x79\x5C\x6E\x5C\x6C\x5C\x69\x5C\x78\x5C\x45\x5C\x6C\x5C\x6B\x5C\x73\x5C\x6E\x5C\x6A\x5C\x6F\x5C\x72\x5C\x6E\x5C\x73\x5C\x6B\x5C\x70\x5C\x6C\x22\x2C\x22\x5C\x31\x74\x5C\x53\x5C\x6B\x5C\x6B\x5C\x69\x5C\x66\x5C\x6D\x5C\x72\x5C\x75\x5C\x66\x5C\x70\x5C\x44\x5C\x78\x5C\x45\x5C\x6F\x5C\x6E\x5C\x70\x5C\x57\x5C\x72\x5C\x6F\x5C\x6E\x5C\x6C\x5C\x69\x22\x2C\x22\x5C\x45\x5C\x69\x5C\x66\x5C\x54\x5C\x69\x22\x2C\x22\x5C\x6C\x5C\x6B\x5C\x73\x5C\x6E\x5C\x6A\x5C\x6F\x5C\x72\x5C\x6E\x5C\x73\x5C\x6B\x5C\x70\x5C\x6C\x5C\x78\x5C\x6C\x5C\x6B\x5C\x73\x5C\x6E\x5C\x6A\x5C\x6F\x5C\x78\x5C\x73\x5C\x6B\x5C\x6F\x5C\x6B\x5C\x6D\x22\x2C\x22\x5C\x45\x5C\x75\x5C\x75\x5C\x72\x5C\x53\x5C\x6B\x5C\x6B\x5C\x69\x5C\x66\x5C\x6D\x22\x2C\x22\x5C\x45\x5C\x7A\x5C\x6F\x5C\x6B\x5C\x48\x5C\x72\x5C\x76\x5C\x6A\x5C\x48\x5C\x66\x5C\x6D\x5C\x78\x5C\x45\x5C\x6F\x5C\x6B\x5C\x6A\x5C\x41\x5C\x6E\x5C\x70\x5C\x48\x22\x2C\x22\x5C\x44\x5C\x6D\x5C\x6F\x22\x2C\x22\x5C\x45\x5C\x7A\x5C\x6F\x5C\x6B\x5C\x48\x5C\x72\x5C\x76\x5C\x6B\x5C\x6C\x5C\x69\x5C\x6C\x22\x2C\x22\x5C\x53\x5C\x6A\x5C\x41\x5C\x66\x5C\x32\x6F\x5C\x70\x5C\x31\x4B\x5C\x76\x22\x2C\x22\x5C\x45\x5C\x76\x5C\x6B\x5C\x6C\x5C\x69\x22\x2C\x22\x5C\x31\x74\x5C\x6F\x5C\x6B\x5C\x6A\x5C\x41\x5C\x72\x5C\x75\x5C\x6B\x5C\x6D\x5C\x66\x22\x2C\x22\x5C\x45\x5C\x7A\x5C\x6F\x5C\x6B\x5C\x48\x5C\x72\x5C\x76\x5C\x6A\x5C\x48\x5C\x66\x5C\x6D\x5C\x78\x5C\x45\x5C\x70\x5C\x6B\x5C\x72\x5C\x75\x5C\x6B\x5C\x6D\x5C\x66\x22\x2C\x22\x5C\x45\x5C\x7A\x5C\x6F\x5C\x6B\x5C\x48\x5C\x72\x5C\x76\x5C\x6B\x5C\x6C\x5C\x69\x5C\x6C\x5C\x78\x5C\x45\x5C\x69\x5C\x47\x5C\x44\x5C\x75\x5C\x7A\x5C\x70\x5C\x6A\x5C\x6E\x5C\x6F\x22\x2C\x22\x5C\x4E\x5C\x6E\x5C\x75\x5C\x48\x5C\x78\x5C\x6C\x5C\x6D\x5C\x73\x5C\x4A\x5C\x42\x5C\x32\x43\x5C\x31\x69\x5C\x42\x5C\x78\x5C\x6A\x5C\x6F\x5C\x69\x5C\x4A\x5C\x42\x5C\x31\x6E\x5C\x6B\x5C\x75\x5C\x75\x5C\x66\x5C\x70\x5C\x69\x5C\x78\x5C\x6E\x5C\x75\x5C\x6A\x5C\x48\x5C\x66\x5C\x42\x5C\x4B\x5C\x4F\x22\x2C\x22\x5C\x4E\x5C\x6C\x5C\x76\x5C\x6A\x5C\x70\x5C\x78\x5C\x73\x5C\x6F\x5C\x6A\x5C\x6C\x5C\x6C\x5C\x4A\x5C\x42\x5C\x73\x5C\x6B\x5C\x75\x5C\x75\x5C\x66\x5C\x70\x5C\x69\x5C\x72\x5C\x50\x5C\x6E\x5C\x41\x5C\x66\x5C\x6B\x5C\x72\x5C\x44\x5C\x6D\x5C\x6F\x5C\x42\x5C\x4F\x5C\x32\x43\x5C\x31\x69\x5C\x4E\x5C\x4B\x5C\x6C\x5C\x76\x5C\x6A\x5C\x70\x5C\x4F\x22\x2C\x22\x5C\x4C\x5C\x6B\x5C\x44\x5C\x69\x5C\x44\x5C\x7A\x5C\x66\x5C\x45\x5C\x73\x5C\x6B\x5C\x75\x22\x2C\x22\x5C\x50\x22\x2C\x22\x5C\x48\x5C\x66\x5C\x69\x22\x2C\x22\x5C\x4C\x5C\x6B\x5C\x44\x5C\x69\x5C\x44\x5C\x45\x5C\x7A\x5C\x66\x22\x2C\x22\x5C\x76\x5C\x6A\x5C\x69\x5C\x47\x5C\x70\x5C\x6A\x5C\x75\x5C\x66\x22\x2C\x22\x5C\x4E\x5C\x41\x5C\x6E\x5C\x50\x5C\x78\x5C\x73\x5C\x6F\x5C\x6A\x5C\x6C\x5C\x6C\x5C\x4A\x5C\x42\x5C\x73\x5C\x6B\x5C\x75\x5C\x75\x5C\x66\x5C\x70\x5C\x69\x5C\x72\x5C\x50\x5C\x6E\x5C\x41\x5C\x66\x5C\x6B\x5C\x78\x5C\x4C\x5C\x69\x5C\x72\x5C\x6E\x5C\x75\x5C\x48\x5C\x42\x5C\x78\x5C\x41\x5C\x6A\x5C\x69\x5C\x6A\x5C\x72\x5C\x6E\x5C\x41\x5C\x4A\x5C\x42\x22\x2C\x22\x5C\x42\x5C\x4F\x5C\x4E\x5C\x6E\x5C\x75\x5C\x48\x5C\x78\x5C\x52\x5C\x6E\x5C\x41\x5C\x69\x5C\x47\x5C\x4A\x5C\x42\x5C\x31\x69\x5C\x31\x66\x5C\x31\x66\x5C\x33\x4A\x5C\x42\x5C\x78\x5C\x47\x5C\x66\x5C\x6E\x5C\x48\x5C\x47\x5C\x69\x5C\x4A\x5C\x42\x5C\x31\x6C\x5C\x31\x69\x5C\x31\x67\x5C\x42\x5C\x78\x5C\x6C\x5C\x6D\x5C\x73\x5C\x4A\x5C\x42\x5C\x47\x5C\x69\x5C\x69\x5C\x76\x5C\x6C\x5C\x31\x62\x5C\x4B\x5C\x4B\x5C\x6E\x5C\x45\x5C\x4C\x5C\x69\x5C\x6E\x5C\x75\x5C\x48\x5C\x45\x5C\x73\x5C\x6B\x5C\x75\x5C\x4B\x5C\x50\x5C\x6E\x5C\x4B\x22\x2C\x22\x5C\x4B\x5C\x47\x5C\x31\x78\x5C\x41\x5C\x66\x5C\x53\x5C\x6A\x5C\x44\x5C\x6F\x5C\x69\x5C\x45\x5C\x31\x48\x5C\x76\x5C\x48\x5C\x42\x5C\x78\x5C\x6A\x5C\x6F\x5C\x69\x5C\x4A\x5C\x42\x5C\x32\x64\x5C\x6B\x5C\x44\x5C\x31\x6F\x5C\x44\x5C\x7A\x5C\x66\x5C\x78\x5C\x50\x5C\x6E\x5C\x41\x5C\x66\x5C\x6B\x5C\x78\x5C\x69\x5C\x47\x5C\x44\x5C\x75\x5C\x7A\x5C\x70\x5C\x6A\x5C\x6E\x5C\x6F\x5C\x42\x5C\x4B\x5C\x4F\x5C\x4E\x5C\x4B\x5C\x41\x5C\x6E\x5C\x50\x5C\x4F\x22\x2C\x22\x5C\x31\x42\x5C\x6D\x5C\x6D\x5C\x6B\x5C\x6D\x5C\x31\x62\x5C\x78\x22\x2C\x22\x5C\x45\x5C\x73\x5C\x6B\x5C\x75\x5C\x75\x5C\x66\x5C\x70\x5C\x69\x5C\x72\x5C\x50\x5C\x6E\x5C\x41\x5C\x66\x5C\x6B\x5C\x72\x5C\x44\x5C\x6D\x5C\x6F\x22\x2C\x22\x5C\x4E\x5C\x6E\x5C\x53\x5C\x6D\x5C\x6A\x5C\x75\x5C\x66\x5C\x78\x5C\x52\x5C\x6E\x5C\x41\x5C\x69\x5C\x47\x5C\x4A\x5C\x42\x5C\x31\x69\x5C\x31\x66\x5C\x31\x66\x5C\x33\x4A\x5C\x42\x5C\x78\x5C\x47\x5C\x66\x5C\x6E\x5C\x48\x5C\x47\x5C\x69\x5C\x4A\x5C\x42\x5C\x31\x6C\x5C\x31\x69\x5C\x31\x67\x5C\x42\x5C\x78\x5C\x6C\x5C\x6D\x5C\x73\x5C\x4A\x5C\x42\x5C\x47\x5C\x69\x5C\x69\x5C\x76\x5C\x6C\x5C\x31\x62\x5C\x4B\x5C\x4B\x5C\x52\x5C\x52\x5C\x52\x5C\x45\x5C\x4C\x5C\x6B\x5C\x44\x5C\x69\x5C\x44\x5C\x7A\x5C\x66\x5C\x45\x5C\x73\x5C\x6B\x5C\x75\x5C\x4B\x5C\x66\x5C\x75\x5C\x7A\x5C\x66\x5C\x41\x5C\x4B\x22\x2C\x22\x5C\x42\x5C\x78\x5C\x69\x5C\x6E\x5C\x69\x5C\x6F\x5C\x66\x5C\x4A\x5C\x42\x5C\x32\x64\x5C\x6B\x5C\x44\x5C\x31\x6F\x5C\x44\x5C\x7A\x5C\x66\x5C\x78\x5C\x50\x5C\x6E\x5C\x41\x5C\x66\x5C\x6B\x5C\x78\x5C\x76\x5C\x6F\x5C\x6A\x5C\x4C\x5C\x66\x5C\x6D\x5C\x42\x5C\x78\x5C\x53\x5C\x6D\x5C\x6A\x5C\x75\x5C\x66\x5C\x7A\x5C\x6B\x5C\x6D\x5C\x41\x5C\x66\x5C\x6D\x5C\x4A\x5C\x42\x5C\x31\x66\x5C\x42\x5C\x78\x5C\x6A\x5C\x6F\x5C\x6F\x5C\x6B\x5C\x52\x5C\x4A\x5C\x42\x5C\x6A\x5C\x73\x5C\x73\x5C\x66\x5C\x6F\x5C\x66\x5C\x6D\x5C\x6B\x5C\x75\x5C\x66\x5C\x69\x5C\x66\x5C\x6D\x5C\x31\x65\x5C\x78\x5C\x6A\x5C\x44\x5C\x69\x5C\x6B\x5C\x76\x5C\x6F\x5C\x6A\x5C\x4C\x5C\x31\x65\x5C\x78\x5C\x73\x5C\x6F\x5C\x6E\x5C\x76\x5C\x7A\x5C\x6B\x5C\x6A\x5C\x6D\x5C\x41\x5C\x72\x5C\x52\x5C\x6D\x5C\x6E\x5C\x69\x5C\x66\x5C\x31\x65\x5C\x78\x5C\x66\x5C\x70\x5C\x73\x5C\x6D\x5C\x4C\x5C\x76\x5C\x69\x5C\x66\x5C\x41\x5C\x72\x5C\x75\x5C\x66\x5C\x41\x5C\x6E\x5C\x6A\x5C\x31\x65\x5C\x78\x5C\x48\x5C\x4C\x5C\x6D\x5C\x6B\x5C\x6C\x5C\x73\x5C\x6B\x5C\x76\x5C\x66\x5C\x31\x65\x5C\x78\x5C\x76\x5C\x6E\x5C\x73\x5C\x69\x5C\x44\x5C\x6D\x5C\x66\x5C\x72\x5C\x6E\x5C\x70\x5C\x72\x5C\x76\x5C\x6E\x5C\x73\x5C\x69\x5C\x44\x5C\x6D\x5C\x66\x5C\x42\x5C\x78\x5C\x6A\x5C\x6F\x5C\x6F\x5C\x6B\x5C\x52\x5C\x53\x5C\x44\x5C\x6F\x5C\x6F\x5C\x6C\x5C\x73\x5C\x6D\x5C\x66\x5C\x66\x5C\x70\x5C\x4F\x5C\x4E\x5C\x4B\x5C\x6E\x5C\x53\x5C\x6D\x5C\x6A\x5C\x75\x5C\x66\x5C\x4F\x22\x2C\x22\x5C\x45\x5C\x73\x5C\x6B\x5C\x75\x5C\x75\x5C\x66\x5C\x70\x5C\x69\x5C\x72\x5C\x50\x5C\x6E\x5C\x41\x5C\x66\x5C\x6B\x22\x2C\x22\x5C\x76\x5C\x45\x5C\x73\x5C\x6B\x5C\x75\x5C\x75\x5C\x66\x5C\x70\x5C\x69\x5C\x72\x5C\x73\x5C\x6B\x5C\x70\x5C\x69\x5C\x66\x5C\x70\x5C\x69\x22\x2C\x22\x5C\x45\x5C\x6C\x5C\x6E\x5C\x69\x5C\x66\x5C\x72\x5C\x53\x5C\x6B\x5C\x6B\x5C\x69\x5C\x66\x5C\x6D\x22\x2C\x22\x5C\x6B\x5C\x70\x5C\x72\x5C\x53\x5C\x6B\x5C\x6B\x5C\x69\x5C\x66\x5C\x6D\x22\x2C\x22\x5C\x6A\x5C\x70\x5C\x6E\x5C\x75\x5C\x6A\x5C\x69\x5C\x66\x22\x2C\x22\x5C\x47\x5C\x69\x5C\x75\x5C\x6F\x5C\x31\x77\x5C\x78\x5C\x7A\x5C\x6B\x5C\x41\x5C\x4C\x22\x2C\x22\x5C\x45\x5C\x7A\x5C\x6A\x5C\x73\x5C\x57\x5C\x72\x5C\x69\x5C\x6B\x5C\x76\x22\x5D\x3B\x32\x7A\x20\x61\x24\x63\x3D\x5B\x61\x24\x65\x5B\x30\x5D\x2C\x61\x24\x65\x5B\x31\x5D\x2C\x61\x24\x65\x5B\x32\x5D\x2C\x61\x24\x65\x5B\x33\x5D\x2C\x61\x24\x65\x5B\x34\x5D\x2C\x61\x24\x65\x5B\x35\x5D\x2C\x61\x24\x65\x5B\x36\x5D\x2C\x61\x24\x65\x5B\x37\x5D\x2C\x61\x24\x65\x5B\x38\x5D\x2C\x61\x24\x65\x5B\x39\x5D\x2C\x61\x24\x65\x5B\x31\x30\x5D\x2C\x61\x24\x65\x5B\x31\x31\x5D\x2C\x61\x24\x65\x5B\x31\x32\x5D\x2C\x61\x24\x65\x5B\x31\x33\x5D\x2C\x61\x24\x65\x5B\x31\x34\x5D\x2C\x61\x24\x65\x5B\x31\x35\x5D\x2C\x61\x24\x65\x5B\x31\x36\x5D\x2C\x61\x24\x65\x5B\x31\x37\x5D\x2C\x61\x24\x65\x5B\x31\x38\x5D\x2C\x61\x24\x65\x5B\x31\x39\x5D\x2C\x61\x24\x65\x5B\x32\x30\x5D\x2C\x61\x24\x65\x5B\x32\x31\x5D\x2C\x61\x24\x65\x5B\x32\x32\x5D\x2C\x61\x24\x65\x5B\x32\x33\x5D\x2C\x61\x24\x65\x5B\x32\x34\x5D\x2C\x61\x24\x65\x5B\x32\x35\x5D\x2C\x61\x24\x65\x5B\x32\x36\x5D\x2C\x61\x24\x65\x5B\x32\x37\x5D\x2C\x61\x24\x65\x5B\x32\x38\x5D\x2C\x61\x24\x65\x5B\x32\x39\x5D\x2C\x61\x24\x65\x5B\x33\x30\x5D\x2C\x61\x24\x65\x5B\x33\x31\x5D\x2C\x61\x24\x65\x5B\x33\x32\x5D\x2C\x61\x24\x65\x5B\x33\x33\x5D\x2C\x61\x24\x65\x5B\x33\x34\x5D\x2C\x61\x24\x65\x5B\x33\x35\x5D\x2C\x61\x24\x65\x5B\x33\x36\x5D\x2C\x61\x24\x65\x5B\x33\x37\x5D\x2C\x61\x24\x65\x5B\x33\x38\x5D\x2C\x61\x24\x65\x5B\x33\x39\x5D\x2C\x61\x24\x65\x5B\x34\x30\x5D\x2C\x61\x24\x65\x5B\x34\x31\x5D\x2C\x61\x24\x65\x5B\x34\x32\x5D\x2C\x61\x24\x65\x5B\x34\x33\x5D\x2C\x61\x24\x65\x5B\x34\x34\x5D\x2C\x61\x24\x65\x5B\x34\x35\x5D\x2C\x61\x24\x65\x5B\x34\x36\x5D\x2C\x61\x24\x65\x5B\x34\x37\x5D\x2C\x61\x24\x65\x5B\x34\x38\x5D\x2C\x61\x24\x65\x5B\x34\x39\x5D\x2C\x61\x24\x65\x5B\x35\x30\x5D\x2C\x61\x24\x65\x5B\x35\x31\x5D\x2C\x61\x24\x65\x5B\x35\x32\x5D\x2C\x61\x24\x65\x5B\x35\x33\x5D\x2C\x61\x24\x65\x5B\x35\x34\x5D\x2C\x61\x24\x65\x5B\x35\x35\x5D\x2C\x61\x24\x65\x5B\x35\x36\x5D\x2C\x61\x24\x65\x5B\x35\x37\x5D\x2C\x61\x24\x65\x5B\x35\x38\x5D\x2C\x61\x24\x65\x5B\x35\x39\x5D\x2C\x61\x24\x65\x5B\x36\x30\x5D\x2C\x61\x24\x65\x5B\x36\x31\x5D\x2C\x61\x24\x65\x5B\x36\x32\x5D\x2C\x61\x24\x65\x5B\x36\x33\x5D\x2C\x61\x24\x65\x5B\x36\x34\x5D\x2C\x61\x24\x65\x5B\x36\x35\x5D\x2C\x61\x24\x65\x5B\x36\x36\x5D\x2C\x61\x24\x65\x5B\x36\x37\x5D\x2C\x61\x24\x65\x5B\x36\x38\x5D\x2C\x61\x24\x65\x5B\x36\x39\x5D\x2C\x61\x24\x65\x5B\x37\x30\x5D\x2C\x61\x24\x65\x5B\x37\x31\x5D\x2C\x61\x24\x65\x5B\x37\x32\x5D\x2C\x61\x24\x65\x5B\x37\x33\x5D\x2C\x61\x24\x65\x5B\x37\x34\x5D\x2C\x61\x24\x65\x5B\x37\x35\x5D\x2C\x61\x24\x65\x5B\x37\x36\x5D\x2C\x61\x24\x65\x5B\x37\x37\x5D\x2C\x61\x24\x65\x5B\x37\x38\x5D\x2C\x61\x24\x65\x5B\x37\x39\x5D\x2C\x61\x24\x65\x5B\x38\x30\x5D\x2C\x61\x24\x65\x5B\x38\x31\x5D\x2C\x61\x24\x65\x5B\x38\x32\x5D\x2C\x61\x24\x65\x5B\x38\x33\x5D\x2C\x61\x24\x65\x5B\x38\x34\x5D\x2C\x61\x24\x65\x5B\x38\x35\x5D\x2C\x61\x24\x65\x5B\x38\x36\x5D\x2C\x61\x24\x65\x5B\x38\x37\x5D\x2C\x61\x24\x65\x5B\x38\x38\x5D\x2C\x61\x24\x65\x5B\x38\x39\x5D\x2C\x61\x24\x65\x5B\x33\x7A\x5D\x2C\x61\x24\x65\x5B\x33\x64\x5D\x2C\x61\x24\x65\x5B\x33\x4D\x5D\x2C\x61\x24\x65\x5B\x32\x41\x5D\x2C\x61\x24\x65\x5B\x35\x70\x5D\x2C\x61\x24\x65\x5B\x35\x41\x5D\x2C\x61\x24\x65\x5B\x35\x42\x5D\x2C\x61\x24\x65\x5B\x35\x43\x5D\x2C\x61\x24\x65\x5B\x34\x66\x5D\x2C\x61\x24\x65\x5B\x35\x44\x5D\x2C\x61\x24\x65\x5B\x32\x4D\x5D\x2C\x61\x24\x65\x5B\x35\x45\x5D\x2C\x61\x24\x65\x5B\x32\x6B\x5D\x2C\x61\x24\x65\x5B\x35\x46\x5D\x2C\x61\x24\x65\x5B\x35\x47\x5D\x2C\x61\x24\x65\x5B\x32\x63\x5D\x2C\x61\x24\x65\x5B\x34\x6A\x5D\x2C\x61\x24\x65\x5B\x34\x59\x5D\x2C\x61\x24\x65\x5B\x34\x6D\x5D\x2C\x61\x24\x65\x5B\x32\x68\x5D\x2C\x61\x24\x65\x5B\x34\x6B\x5D\x2C\x61\x24\x65\x5B\x35\x65\x5D\x2C\x61\x24\x65\x5B\x35\x66\x5D\x2C\x61\x24\x65\x5B\x35\x67\x5D\x2C\x61\x24\x65\x5B\x35\x69\x5D\x2C\x61\x24\x65\x5B\x35\x6A\x5D\x2C\x61\x24\x65\x5B\x33\x6E\x5D\x2C\x61\x24\x65\x5B\x35\x72\x5D\x2C\x61\x24\x65\x5B\x34\x52\x5D\x2C\x61\x24\x65\x5B\x32\x52\x5D\x2C\x61\x24\x65\x5B\x35\x6C\x5D\x2C\x61\x24\x65\x5B\x35\x6B\x5D\x2C\x61\x24\x65\x5B\x35\x68\x5D\x2C\x61\x24\x65\x5B\x35\x63\x5D\x2C\x61\x24\x65\x5B\x32\x46\x5D\x2C\x61\x24\x65\x5B\x34\x55\x5D\x2C\x61\x24\x65\x5B\x35\x62\x5D\x2C\x61\x24\x65\x5B\x33\x41\x5D\x2C\x61\x24\x65\x5B\x33\x79\x5D\x2C\x61\x24\x65\x5B\x33\x78\x5D\x2C\x61\x24\x65\x5B\x32\x4F\x5D\x2C\x61\x24\x65\x5B\x32\x51\x5D\x2C\x61\x24\x65\x5B\x32\x47\x5D\x2C\x61\x24\x65\x5B\x32\x42\x5D\x2C\x61\x24\x65\x5B\x33\x62\x5D\x2C\x61\x24\x65\x5B\x33\x71\x5D\x2C\x61\x24\x65\x5B\x33\x44\x5D\x2C\x61\x24\x65\x5B\x33\x43\x5D\x2C\x61\x24\x65\x5B\x31\x57\x5D\x2C\x61\x24\x65\x5B\x35\x7A\x5D\x2C\x61\x24\x65\x5B\x33\x76\x5D\x2C\x61\x24\x65\x5B\x32\x48\x5D\x2C\x61\x24\x65\x5B\x31\x6D\x5D\x2C\x61\x24\x65\x5B\x33\x70\x5D\x2C\x61\x24\x65\x5B\x59\x5D\x2C\x61\x24\x65\x5B\x33\x6F\x5D\x2C\x61\x24\x65\x5B\x33\x6D\x5D\x2C\x61\x24\x65\x5B\x35\x78\x5D\x2C\x61\x24\x65\x5B\x32\x66\x5D\x2C\x61\x24\x65\x5B\x31\x49\x5D\x2C\x61\x24\x65\x5B\x34\x53\x5D\x2C\x61\x24\x65\x5B\x35\x71\x5D\x2C\x61\x24\x65\x5B\x35\x6F\x5D\x2C\x61\x24\x65\x5B\x34\x43\x5D\x2C\x61\x24\x65\x5B\x34\x4F\x5D\x2C\x61\x24\x65\x5B\x34\x50\x5D\x2C\x61\x24\x65\x5B\x34\x51\x5D\x2C\x61\x24\x65\x5B\x34\x44\x5D\x2C\x61\x24\x65\x5B\x31\x44\x5D\x2C\x61\x24\x65\x5B\x33\x69\x5D\x2C\x61\x24\x65\x5B\x34\x49\x5D\x2C\x61\x24\x65\x5B\x34\x48\x5D\x2C\x61\x24\x65\x5B\x34\x47\x5D\x2C\x61\x24\x65\x5B\x33\x56\x5D\x2C\x61\x24\x65\x5B\x33\x53\x5D\x2C\x61\x24\x65\x5B\x34\x45\x5D\x2C\x61\x24\x65\x5B\x34\x46\x5D\x2C\x61\x24\x65\x5B\x34\x71\x5D\x2C\x61\x24\x65\x5B\x34\x41\x5D\x2C\x61\x24\x65\x5B\x34\x72\x5D\x2C\x61\x24\x65\x5B\x31\x46\x5D\x2C\x61\x24\x65\x5B\x34\x73\x5D\x2C\x61\x24\x65\x5B\x34\x77\x5D\x2C\x61\x24\x65\x5B\x34\x78\x5D\x2C\x61\x24\x65\x5B\x34\x79\x5D\x2C\x61\x24\x65\x5B\x34\x75\x5D\x2C\x61\x24\x65\x5B\x35\x4A\x5D\x2C\x61\x24\x65\x5B\x32\x75\x5D\x2C\x61\x24\x65\x5B\x31\x41\x5D\x2C\x61\x24\x65\x5B\x37\x54\x5D\x2C\x61\x24\x65\x5B\x37\x4D\x5D\x2C\x61\x24\x65\x5B\x35\x52\x5D\x2C\x61\x24\x65\x5B\x32\x44\x5D\x2C\x61\x24\x65\x5B\x37\x41\x5D\x2C\x61\x24\x65\x5B\x37\x42\x5D\x2C\x61\x24\x65\x5B\x37\x77\x5D\x2C\x61\x24\x65\x5B\x33\x67\x5D\x2C\x61\x24\x65\x5B\x33\x65\x5D\x2C\x61\x24\x65\x5B\x38\x69\x5D\x2C\x61\x24\x65\x5B\x37\x6F\x5D\x2C\x61\x24\x65\x5B\x31\x59\x5D\x2C\x61\x24\x65\x5B\x37\x49\x5D\x2C\x61\x24\x65\x5B\x37\x4A\x5D\x2C\x61\x24\x65\x5B\x37\x48\x5D\x2C\x61\x24\x65\x5B\x35\x49\x5D\x2C\x61\x24\x65\x5B\x37\x46\x5D\x2C\x61\x24\x65\x5B\x37\x6C\x5D\x2C\x61\x24\x65\x5B\x33\x74\x5D\x2C\x61\x24\x65\x5B\x33\x75\x5D\x2C\x61\x24\x65\x5B\x37\x45\x5D\x2C\x61\x24\x65\x5B\x38\x61\x5D\x2C\x61\x24\x65\x5B\x38\x65\x5D\x2C\x61\x24\x65\x5B\x32\x74\x5D\x2C\x61\x24\x65\x5B\x32\x4E\x5D\x2C\x61\x24\x65\x5B\x37\x56\x5D\x2C\x61\x24\x65\x5B\x37\x4F\x5D\x2C\x61\x24\x65\x5B\x33\x6B\x5D\x2C\x61\x24\x65\x5B\x37\x47\x5D\x2C\x61\x24\x65\x5B\x33\x63\x5D\x2C\x61\x24\x65\x5B\x37\x6B\x5D\x2C\x61\x24\x65\x5B\x37\x51\x5D\x2C\x61\x24\x65\x5B\x37\x58\x5D\x2C\x61\x24\x65\x5B\x37\x57\x5D\x2C\x61\x24\x65\x5B\x38\x67\x5D\x2C\x61\x24\x65\x5B\x38\x66\x5D\x2C\x61\x24\x65\x5B\x37\x5A\x5D\x2C\x61\x24\x65\x5B\x38\x64\x5D\x2C\x61\x24\x65\x5B\x38\x63\x5D\x2C\x61\x24\x65\x5B\x37\x76\x5D\x2C\x61\x24\x65\x5B\x37\x44\x5D\x2C\x61\x24\x65\x5B\x37\x43\x5D\x2C\x61\x24\x65\x5B\x37\x78\x5D\x2C\x61\x24\x65\x5B\x37\x74\x5D\x2C\x61\x24\x65\x5B\x37\x73\x5D\x2C\x61\x24\x65\x5B\x37\x72\x5D\x2C\x61\x24\x65\x5B\x37\x71\x5D\x2C\x61\x24\x65\x5B\x37\x70\x5D\x2C\x61\x24\x65\x5B\x33\x73\x5D\x2C\x61\x24\x65\x5B\x37\x4C\x5D\x2C\x61\x24\x65\x5B\x37\x6E\x5D\x2C\x61\x24\x65\x5B\x37\x6D\x5D\x2C\x61\x24\x65\x5B\x37\x75\x5D\x2C\x61\x24\x65\x5B\x37\x55\x5D\x2C\x61\x24\x65\x5B\x38\x62\x5D\x2C\x61\x24\x65\x5B\x37\x79\x5D\x2C\x61\x24\x65\x5B\x32\x59\x5D\x2C\x61\x24\x65\x5B\x38\x68\x5D\x2C\x61\x24\x65\x5B\x32\x54\x5D\x2C\x61\x24\x65\x5B\x32\x76\x5D\x2C\x61\x24\x65\x5B\x37\x4E\x5D\x2C\x61\x24\x65\x5B\x37\x52\x5D\x2C\x61\x24\x65\x5B\x37\x53\x5D\x2C\x61\x24\x65\x5B\x32\x5A\x5D\x2C\x61\x24\x65\x5B\x32\x50\x5D\x2C\x61\x24\x65\x5B\x32\x53\x5D\x2C\x61\x24\x65\x5B\x37\x59\x5D\x2C\x61\x24\x65\x5B\x37\x7A\x5D\x2C\x61\x24\x65\x5B\x36\x77\x5D\x2C\x61\x24\x65\x5B\x37\x69\x5D\x2C\x61\x24\x65\x5B\x36\x65\x5D\x2C\x61\x24\x65\x5B\x36\x66\x5D\x2C\x61\x24\x65\x5B\x36\x67\x5D\x2C\x61\x24\x65\x5B\x36\x68\x5D\x2C\x61\x24\x65\x5B\x36\x6A\x5D\x2C\x61\x24\x65\x5B\x32\x49\x5D\x2C\x61\x24\x65\x5B\x36\x69\x5D\x2C\x61\x24\x65\x5B\x37\x50\x5D\x2C\x61\x24\x65\x5B\x32\x57\x5D\x2C\x61\x24\x65\x5B\x32\x56\x5D\x2C\x61\x24\x65\x5B\x32\x55\x5D\x2C\x61\x24\x65\x5B\x36\x6B\x5D\x2C\x61\x24\x65\x5B\x36\x6E\x5D\x2C\x61\x24\x65\x5B\x36\x6F\x5D\x2C\x61\x24\x65\x5B\x36\x70\x5D\x2C\x61\x24\x65\x5B\x36\x71\x5D\x2C\x61\x24\x65\x5B\x36\x6C\x5D\x2C\x61\x24\x65\x5B\x36\x64\x5D\x2C\x61\x24\x65\x5B\x36\x74\x5D\x2C\x61\x24\x65\x5B\x36\x62\x5D\x2C\x61\x24\x65\x5B\x36\x6D\x5D\x2C\x61\x24\x65\x5B\x36\x61\x5D\x2C\x61\x24\x65\x5B\x35\x4C\x5D\x2C\x61\x24\x65\x5B\x35\x4D\x5D\x2C\x61\x24\x65\x5B\x35\x4E\x5D\x2C\x61\x24\x65\x5B\x33\x4B\x5D\x2C\x61\x24\x65\x5B\x31\x53\x5D\x2C\x61\x24\x65\x5B\x35\x4F\x5D\x2C\x61\x24\x65\x5B\x32\x4C\x5D\x2C\x61\x24\x65\x5B\x36\x73\x5D\x2C\x61\x24\x65\x5B\x35\x50\x5D\x2C\x61\x24\x65\x5B\x35\x4B\x5D\x2C\x61\x24\x65\x5B\x35\x51\x5D\x2C\x61\x24\x65\x5B\x33\x48\x5D\x2C\x61\x24\x65\x5B\x33\x51\x5D\x2C\x61\x24\x65\x5B\x35\x54\x5D\x2C\x61\x24\x65\x5B\x35\x55\x5D\x2C\x61\x24\x65\x5B\x33\x4C\x5D\x2C\x61\x24\x65\x5B\x33\x50\x5D\x2C\x61\x24\x65\x5B\x35\x56\x5D\x2C\x61\x24\x65\x5B\x35\x57\x5D\x2C\x61\x24\x65\x5B\x33\x58\x5D\x2C\x61\x24\x65\x5B\x32\x73\x5D\x2C\x61\x24\x65\x5B\x35\x59\x5D\x2C\x61\x24\x65\x5B\x35\x5A\x5D\x2C\x61\x24\x65\x5B\x35\x58\x5D\x2C\x61\x24\x65\x5B\x36\x63\x5D\x2C\x61\x24\x65\x5B\x33\x59\x5D\x2C\x61\x24\x65\x5B\x34\x64\x5D\x2C\x61\x24\x65\x5B\x33\x5A\x5D\x2C\x61\x24\x65\x5B\x36\x51\x5D\x2C\x61\x24\x65\x5B\x36\x53\x5D\x2C\x61\x24\x65\x5B\x36\x76\x5D\x2C\x61\x24\x65\x5B\x32\x45\x5D\x2C\x61\x24\x65\x5B\x36\x55\x5D\x2C\x61\x24\x65\x5B\x34\x62\x5D\x2C\x61\x24\x65\x5B\x34\x61\x5D\x2C\x61\x24\x65\x5B\x36\x54\x5D\x2C\x61\x24\x65\x5B\x36\x75\x5D\x2C\x61\x24\x65\x5B\x36\x57\x5D\x2C\x61\x24\x65\x5B\x36\x58\x5D\x2C\x61\x24\x65\x5B\x36\x52\x5D\x2C\x61\x24\x65\x5B\x36\x59\x5D\x2C\x61\x24\x65\x5B\x36\x56\x5D\x2C\x61\x24\x65\x5B\x36\x5A\x5D\x2C\x61\x24\x65\x5B\x33\x52\x5D\x2C\x61\x24\x65\x5B\x34\x63\x5D\x2C\x61\x24\x65\x5B\x37\x64\x5D\x2C\x61\x24\x65\x5B\x37\x63\x5D\x2C\x61\x24\x65\x5B\x33\x55\x5D\x2C\x61\x24\x65\x5B\x37\x65\x5D\x2C\x61\x24\x65\x5B\x37\x66\x5D\x2C\x61\x24\x65\x5B\x37\x61\x5D\x2C\x61\x24\x65\x5B\x36\x47\x5D\x2C\x61\x24\x65\x5B\x36\x79\x5D\x2C\x61\x24\x65\x5B\x36\x41\x5D\x2C\x61\x24\x65\x5B\x36\x7A\x5D\x2C\x61\x24\x65\x5B\x36\x42\x5D\x2C\x61\x24\x65\x5B\x36\x43\x5D\x2C\x61\x24\x65\x5B\x36\x44\x5D\x2C\x61\x24\x65\x5B\x36\x45\x5D\x2C\x61\x24\x65\x5B\x36\x78\x5D\x2C\x61\x24\x65\x5B\x36\x46\x5D\x2C\x61\x24\x65\x5B\x36\x4F\x5D\x2C\x61\x24\x65\x5B\x36\x49\x5D\x2C\x61\x24\x65\x5B\x36\x4A\x5D\x2C\x61\x24\x65\x5B\x36\x48\x5D\x2C\x61\x24\x65\x5B\x37\x67\x5D\x2C\x61\x24\x65\x5B\x36\x4C\x5D\x2C\x61\x24\x65\x5B\x34\x6C\x5D\x2C\x61\x24\x65\x5B\x36\x4E\x5D\x2C\x61\x24\x65\x5B\x36\x4D\x5D\x2C\x61\x24\x65\x5B\x36\x4B\x5D\x5D\x3B\x61\x24\x63\x5B\x30\x5D\x3B\x21\x43\x28\x71\x29\x7B\x71\x5B\x61\x24\x63\x5B\x32\x5D\x5D\x5B\x61\x24\x63\x5B\x31\x5D\x5D\x3D\x43\x28\x79\x29\x7B\x31\x64\x20\x79\x3D\x71\x5B\x61\x24\x63\x5B\x33\x5D\x5D\x28\x7B\x34\x42\x3A\x21\x30\x7D\x2C\x79\x29\x2C\x56\x5B\x61\x24\x63\x5B\x35\x31\x5D\x5D\x28\x43\x28\x29\x7B\x4D\x20\x46\x3D\x71\x28\x56\x29\x2C\x49\x3D\x71\x28\x32\x6A\x29\x2C\x51\x3D\x46\x5B\x61\x24\x63\x5B\x34\x5D\x5D\x28\x29\x3E\x3D\x31\x3F\x46\x5B\x61\x24\x63\x5B\x34\x5D\x5D\x28\x29\x3A\x31\x2C\x58\x3D\x46\x5B\x61\x24\x63\x5B\x35\x5D\x5D\x28\x29\x3E\x3D\x31\x3F\x46\x5B\x61\x24\x63\x5B\x35\x5D\x5D\x28\x29\x3A\x31\x2C\x5A\x3D\x61\x24\x63\x5B\x36\x5D\x2B\x35\x76\x5B\x61\x24\x63\x5B\x37\x5D\x5D\x28\x51\x2B\x51\x2F\x31\x30\x29\x2B\x61\x24\x63\x5B\x38\x5D\x2B\x35\x76\x5B\x61\x24\x63\x5B\x37\x5D\x5D\x28\x58\x2B\x58\x2F\x31\x30\x29\x2B\x61\x24\x63\x5B\x39\x5D\x2C\x55\x3D\x46\x5B\x61\x24\x63\x5B\x31\x31\x5D\x5D\x28\x61\x24\x63\x5B\x31\x30\x5D\x29\x2C\x31\x72\x3D\x55\x5B\x61\x24\x63\x5B\x31\x34\x5D\x5D\x28\x29\x5B\x61\x24\x63\x5B\x31\x33\x5D\x5D\x28\x61\x24\x63\x5B\x31\x32\x5D\x29\x3F\x61\x24\x63\x5B\x31\x35\x5D\x3A\x61\x24\x63\x5B\x31\x36\x5D\x3B\x55\x5B\x61\x24\x63\x5B\x31\x33\x5D\x5D\x28\x61\x24\x63\x5B\x31\x37\x5D\x29\x26\x26\x28\x55\x3D\x61\x24\x63\x5B\x31\x38\x5D\x21\x3D\x38\x6C\x20\x35\x77\x3F\x35\x77\x3A\x31\x63\x5B\x61\x24\x63\x5B\x31\x39\x5D\x5D\x29\x2C\x28\x55\x5B\x61\x24\x63\x5B\x31\x33\x5D\x5D\x28\x61\x24\x63\x5B\x32\x30\x5D\x29\x7C\x7C\x55\x5B\x61\x24\x63\x5B\x31\x33\x5D\x5D\x28\x61\x24\x63\x5B\x32\x31\x5D\x29\x29\x26\x26\x55\x5B\x61\x24\x63\x5B\x31\x33\x5D\x5D\x28\x61\x24\x63\x5B\x32\x32\x5D\x29\x26\x26\x28\x55\x3D\x55\x5B\x61\x24\x63\x5B\x32\x33\x5D\x5D\x28\x61\x24\x63\x5B\x32\x32\x5D\x29\x5B\x30\x5D\x2B\x61\x24\x63\x5B\x32\x34\x5D\x29\x2C\x28\x55\x5B\x61\x24\x63\x5B\x31\x33\x5D\x5D\x28\x61\x24\x63\x5B\x32\x30\x5D\x29\x7C\x7C\x55\x5B\x61\x24\x63\x5B\x31\x33\x5D\x5D\x28\x61\x24\x63\x5B\x32\x31\x5D\x29\x29\x26\x26\x21\x55\x5B\x61\x24\x63\x5B\x31\x33\x5D\x5D\x28\x61\x24\x63\x5B\x32\x32\x5D\x29\x26\x26\x28\x55\x2B\x3D\x61\x24\x63\x5B\x32\x34\x5D\x29\x2C\x55\x5B\x61\x24\x63\x5B\x31\x33\x5D\x5D\x28\x61\x24\x63\x5B\x32\x31\x5D\x29\x26\x26\x55\x5B\x61\x24\x63\x5B\x31\x33\x5D\x5D\x28\x61\x24\x63\x5B\x32\x35\x5D\x29\x26\x26\x28\x55\x3D\x55\x5B\x61\x24\x63\x5B\x32\x38\x5D\x5D\x28\x61\x24\x63\x5B\x32\x36\x5D\x2C\x61\x24\x63\x5B\x32\x37\x5D\x29\x29\x3B\x4D\x20\x31\x68\x3B\x43\x20\x31\x70\x28\x29\x7B\x4D\x20\x71\x3D\x33\x49\x20\x38\x72\x3B\x71\x5B\x61\x24\x63\x5B\x32\x39\x5D\x5D\x3D\x43\x28\x29\x7B\x46\x5B\x61\x24\x63\x5B\x33\x35\x5D\x5D\x28\x61\x24\x63\x5B\x33\x32\x5D\x2C\x61\x24\x63\x5B\x33\x33\x5D\x2B\x56\x5B\x61\x24\x63\x5B\x31\x30\x5D\x5D\x2B\x61\x24\x63\x5B\x33\x34\x5D\x29\x5B\x61\x24\x63\x5B\x33\x31\x5D\x5D\x28\x61\x24\x63\x5B\x33\x30\x5D\x29\x7D\x2C\x71\x5B\x61\x24\x63\x5B\x31\x30\x5D\x5D\x3D\x31\x68\x7D\x31\x68\x3D\x55\x5B\x61\x24\x63\x5B\x31\x33\x5D\x5D\x28\x61\x24\x63\x5B\x33\x36\x5D\x29\x3F\x55\x5B\x61\x24\x63\x5B\x32\x38\x5D\x5D\x28\x61\x24\x63\x5B\x33\x36\x5D\x2C\x61\x24\x63\x5B\x33\x37\x5D\x2B\x5A\x2B\x31\x72\x29\x3A\x55\x5B\x61\x24\x63\x5B\x31\x33\x5D\x5D\x28\x61\x24\x63\x5B\x33\x38\x5D\x29\x3F\x55\x5B\x61\x24\x63\x5B\x32\x38\x5D\x5D\x28\x61\x24\x63\x5B\x33\x39\x5D\x2C\x61\x24\x63\x5B\x33\x37\x5D\x2B\x5A\x2B\x31\x72\x29\x3A\x55\x5B\x61\x24\x63\x5B\x31\x33\x5D\x5D\x28\x61\x24\x63\x5B\x34\x30\x5D\x29\x3F\x55\x5B\x61\x24\x63\x5B\x32\x38\x5D\x5D\x28\x61\x24\x63\x5B\x32\x34\x5D\x2C\x61\x24\x63\x5B\x32\x32\x5D\x2B\x5A\x2B\x31\x72\x29\x3A\x55\x2C\x21\x30\x3D\x3D\x79\x5B\x61\x24\x63\x5B\x34\x31\x5D\x5D\x3F\x49\x5B\x61\x24\x63\x5B\x34\x39\x5D\x5D\x28\x61\x24\x63\x5B\x34\x34\x5D\x2C\x43\x20\x71\x28\x29\x7B\x49\x5B\x61\x24\x63\x5B\x34\x35\x5D\x5D\x28\x29\x2B\x49\x5B\x61\x24\x63\x5B\x35\x5D\x5D\x28\x29\x3E\x3D\x46\x5B\x61\x24\x63\x5B\x34\x37\x5D\x5D\x28\x29\x5B\x61\x24\x63\x5B\x34\x36\x5D\x5D\x26\x26\x28\x49\x5B\x61\x24\x63\x5B\x34\x38\x5D\x5D\x28\x61\x24\x63\x5B\x34\x34\x5D\x2C\x71\x29\x2C\x31\x70\x28\x29\x29\x7D\x29\x5B\x61\x24\x63\x5B\x34\x33\x5D\x5D\x28\x61\x24\x63\x5B\x34\x32\x5D\x29\x3A\x49\x5B\x61\x24\x63\x5B\x34\x39\x5D\x5D\x28\x61\x24\x63\x5B\x35\x30\x5D\x2C\x43\x20\x71\x28\x29\x7B\x49\x5B\x61\x24\x63\x5B\x34\x38\x5D\x5D\x28\x61\x24\x63\x5B\x35\x30\x5D\x2C\x71\x29\x2C\x31\x70\x28\x29\x7D\x29\x5B\x61\x24\x63\x5B\x34\x33\x5D\x5D\x28\x61\x24\x63\x5B\x35\x30\x5D\x29\x7D\x29\x7D\x7D\x28\x38\x7A\x29\x3B\x38\x41\x20\x24\x77\x3D\x24\x28\x32\x6A\x29\x2C\x24\x64\x3D\x24\x28\x33\x57\x29\x2C\x24\x68\x3D\x24\x28\x61\x24\x63\x5B\x35\x32\x5D\x29\x2C\x24\x62\x3D\x24\x28\x61\x24\x63\x5B\x35\x33\x5D\x29\x3B\x43\x20\x31\x76\x28\x71\x2C\x79\x29\x7B\x4D\x20\x46\x3D\x71\x5B\x61\x24\x63\x5B\x32\x33\x5D\x5D\x28\x61\x24\x63\x5B\x35\x34\x5D\x29\x2C\x49\x3D\x2F\x28\x5B\x5E\x7B\x5C\x7D\x5D\x2B\x28\x3F\x3D\x7D\x29\x29\x2F\x67\x2C\x51\x3D\x46\x5B\x61\x24\x63\x5B\x35\x35\x5D\x5D\x3B\x32\x69\x28\x4D\x20\x58\x3D\x30\x3B\x58\x3C\x51\x3B\x58\x2B\x2B\x29\x7B\x4D\x20\x5A\x3D\x46\x5B\x58\x5D\x5B\x61\x24\x63\x5B\x32\x33\x5D\x5D\x28\x61\x24\x63\x5B\x32\x32\x5D\x29\x3B\x31\x7A\x28\x5A\x5B\x30\x5D\x5B\x61\x24\x63\x5B\x35\x36\x5D\x5D\x28\x29\x3D\x3D\x79\x29\x7B\x4D\x20\x55\x3D\x5A\x5B\x31\x5D\x3B\x31\x7A\x28\x55\x26\x26\x38\x77\x21\x3D\x55\x5B\x61\x24\x63\x5B\x31\x33\x5D\x5D\x28\x49\x29\x29\x7B\x31\x64\x20\x38\x78\x28\x55\x5B\x61\x24\x63\x5B\x31\x33\x5D\x5D\x28\x49\x29\x29\x5B\x61\x24\x63\x5B\x35\x36\x5D\x5D\x28\x29\x7D\x3B\x33\x6C\x7D\x7D\x3B\x31\x64\x21\x31\x7D\x43\x20\x33\x4E\x28\x29\x7B\x33\x66\x5B\x61\x24\x63\x5B\x35\x37\x5D\x5D\x3D\x61\x24\x63\x5B\x31\x35\x5D\x2C\x24\x28\x61\x24\x63\x5B\x35\x39\x5D\x29\x5B\x61\x24\x63\x5B\x33\x31\x5D\x5D\x28\x61\x24\x63\x5B\x35\x38\x5D\x29\x2C\x24\x62\x5B\x61\x24\x63\x5B\x33\x31\x5D\x5D\x28\x61\x24\x63\x5B\x36\x30\x5D\x29\x2C\x31\x54\x28\x43\x28\x29\x7B\x24\x28\x61\x24\x63\x5B\x36\x32\x5D\x29\x5B\x61\x24\x63\x5B\x36\x31\x5D\x5D\x28\x29\x7D\x2C\x31\x46\x29\x7D\x43\x20\x33\x4F\x28\x29\x7B\x31\x54\x28\x43\x28\x29\x7B\x24\x28\x61\x24\x63\x5B\x36\x32\x5D\x29\x5B\x61\x24\x63\x5B\x36\x34\x5D\x5D\x28\x29\x5B\x61\x24\x63\x5B\x36\x33\x5D\x5D\x28\x61\x24\x63\x5B\x31\x35\x5D\x29\x2C\x24\x28\x61\x24\x63\x5B\x36\x38\x5D\x29\x5B\x61\x24\x63\x5B\x35\x32\x5D\x5D\x28\x61\x24\x63\x5B\x31\x35\x5D\x29\x5B\x61\x24\x63\x5B\x36\x36\x5D\x5D\x28\x61\x24\x63\x5B\x34\x32\x5D\x29\x5B\x61\x24\x63\x5B\x36\x37\x5D\x5D\x28\x29\x5B\x61\x24\x63\x5B\x36\x36\x5D\x5D\x28\x61\x24\x63\x5B\x36\x35\x5D\x29\x2C\x24\x28\x61\x24\x63\x5B\x35\x39\x5D\x29\x5B\x61\x24\x63\x5B\x36\x36\x5D\x5D\x28\x61\x24\x63\x5B\x35\x38\x5D\x29\x7D\x2C\x31\x46\x29\x7D\x43\x20\x33\x61\x28\x29\x7B\x24\x28\x61\x24\x63\x5B\x37\x30\x5D\x29\x5B\x61\x24\x63\x5B\x34\x39\x5D\x5D\x28\x61\x24\x63\x5B\x36\x39\x5D\x2C\x43\x28\x29\x7B\x24\x62\x5B\x61\x24\x63\x5B\x36\x36\x5D\x5D\x28\x61\x24\x63\x5B\x36\x30\x5D\x29\x2C\x33\x4F\x28\x29\x7D\x29\x2C\x24\x77\x5B\x61\x24\x63\x5B\x34\x39\x5D\x5D\x28\x61\x24\x63\x5B\x37\x31\x5D\x2C\x43\x28\x71\x29\x7B\x32\x37\x3D\x3D\x71\x5B\x61\x24\x63\x5B\x37\x32\x5D\x5D\x26\x26\x28\x24\x62\x5B\x61\x24\x63\x5B\x36\x36\x5D\x5D\x28\x61\x24\x63\x5B\x36\x30\x5D\x29\x2C\x33\x4F\x28\x29\x29\x7D\x29\x7D\x43\x20\x33\x46\x28\x29\x7B\x24\x62\x5B\x61\x24\x63\x5B\x36\x36\x5D\x5D\x28\x61\x24\x63\x5B\x37\x33\x5D\x29\x2C\x31\x54\x28\x43\x28\x29\x7B\x24\x28\x61\x24\x63\x5B\x35\x39\x5D\x29\x5B\x61\x24\x63\x5B\x36\x36\x5D\x5D\x28\x61\x24\x63\x5B\x35\x38\x5D\x29\x7D\x2C\x31\x46\x29\x7D\x43\x20\x33\x42\x28\x29\x7B\x24\x28\x61\x24\x63\x5B\x35\x39\x5D\x29\x5B\x61\x24\x63\x5B\x33\x31\x5D\x5D\x28\x61\x24\x63\x5B\x35\x38\x5D\x29\x2C\x24\x62\x5B\x61\x24\x63\x5B\x33\x31\x5D\x5D\x28\x61\x24\x63\x5B\x37\x33\x5D\x29\x2C\x24\x28\x61\x24\x63\x5B\x37\x34\x5D\x29\x5B\x61\x24\x63\x5B\x34\x39\x5D\x5D\x28\x61\x24\x63\x5B\x36\x39\x5D\x2C\x43\x28\x29\x7B\x33\x46\x28\x29\x7D\x29\x2C\x24\x77\x5B\x61\x24\x63\x5B\x34\x39\x5D\x5D\x28\x61\x24\x63\x5B\x37\x31\x5D\x2C\x43\x28\x71\x29\x7B\x32\x37\x3D\x3D\x71\x5B\x61\x24\x63\x5B\x37\x32\x5D\x5D\x26\x26\x33\x46\x28\x29\x7D\x29\x7D\x43\x20\x32\x58\x28\x71\x29\x7B\x24\x28\x71\x29\x5B\x61\x24\x63\x5B\x35\x31\x5D\x5D\x28\x43\x28\x29\x7B\x4D\x20\x71\x3D\x24\x28\x56\x29\x5B\x61\x24\x63\x5B\x33\x35\x5D\x5D\x28\x61\x24\x63\x5B\x37\x35\x5D\x29\x3B\x71\x26\x26\x32\x6A\x5B\x61\x24\x63\x5B\x37\x37\x5D\x5D\x28\x71\x2C\x61\x24\x63\x5B\x37\x36\x5D\x29\x7D\x29\x7D\x43\x20\x33\x68\x28\x71\x29\x7B\x31\x64\x60\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x61\x24\x63\x5B\x37\x38\x5D\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x28\x61\x24\x63\x5B\x37\x39\x5D\x21\x3D\x71\x3F\x61\x24\x63\x5B\x38\x30\x5D\x3A\x61\x24\x63\x5B\x31\x35\x5D\x29\x2B\x31\x63\x5B\x61\x24\x63\x5B\x38\x31\x5D\x5D\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x61\x24\x63\x5B\x38\x32\x5D\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x60\x7D\x43\x20\x33\x72\x28\x29\x7B\x31\x64\x20\x61\x24\x63\x5B\x38\x33\x5D\x7D\x43\x20\x33\x77\x28\x71\x2C\x79\x29\x7B\x4D\x20\x46\x3B\x31\x64\x20\x46\x3D\x61\x24\x63\x5B\x38\x34\x5D\x3D\x3D\x3D\x79\x3F\x60\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x61\x24\x63\x5B\x38\x35\x5D\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x71\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x61\x24\x63\x5B\x38\x36\x5D\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x60\x3A\x60\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x61\x24\x63\x5B\x38\x37\x5D\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x79\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x61\x24\x63\x5B\x38\x38\x5D\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x71\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x61\x24\x63\x5B\x38\x36\x5D\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x60\x7D\x43\x20\x34\x76\x28\x71\x29\x7B\x31\x64\x20\x71\x5B\x61\x24\x63\x5B\x38\x39\x5D\x5D\x7D\x43\x20\x34\x56\x28\x71\x29\x7B\x31\x64\x20\x71\x5B\x61\x24\x63\x5B\x33\x7A\x5D\x5D\x7D\x43\x20\x34\x57\x28\x71\x29\x7B\x31\x64\x20\x71\x5B\x61\x24\x63\x5B\x33\x64\x5D\x5D\x7D\x43\x20\x34\x5A\x28\x71\x29\x7B\x61\x24\x63\x5B\x31\x35\x5D\x21\x3D\x31\x63\x5B\x61\x24\x63\x5B\x33\x4D\x5D\x5D\x26\x26\x31\x63\x5B\x61\x24\x63\x5B\x33\x4D\x5D\x5D\x3B\x4D\x20\x79\x3D\x31\x63\x5B\x61\x24\x63\x5B\x32\x41\x5D\x5D\x3F\x60\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x61\x24\x63\x5B\x35\x70\x5D\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x71\x5B\x61\x24\x63\x5B\x35\x41\x5D\x5D\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x61\x24\x63\x5B\x35\x42\x5D\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x60\x3A\x61\x24\x63\x5B\x31\x35\x5D\x3B\x31\x64\x20\x79\x7D\x43\x20\x35\x61\x28\x71\x29\x7B\x4D\x20\x79\x3D\x71\x5B\x61\x24\x63\x5B\x34\x66\x5D\x5D\x5B\x61\x24\x63\x5B\x35\x43\x5D\x5D\x2C\x46\x3D\x71\x5B\x61\x24\x63\x5B\x34\x66\x5D\x5D\x5B\x61\x24\x63\x5B\x35\x44\x5D\x5D\x2C\x49\x3D\x31\x63\x5B\x61\x24\x63\x5B\x32\x41\x5D\x5D\x26\x26\x61\x24\x63\x5B\x31\x35\x5D\x21\x3D\x31\x63\x5B\x61\x24\x63\x5B\x32\x4D\x5D\x5D\x3F\x60\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x61\x24\x63\x5B\x35\x45\x5D\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x31\x63\x5B\x61\x24\x63\x5B\x32\x4D\x5D\x5D\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x61\x24\x63\x5B\x38\x32\x5D\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x60\x3A\x61\x24\x63\x5B\x31\x35\x5D\x2C\x51\x3D\x21\x30\x3D\x3D\x31\x63\x5B\x61\x24\x63\x5B\x32\x6B\x5D\x5D\x3F\x60\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x61\x24\x63\x5B\x35\x46\x5D\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x49\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x61\x24\x63\x5B\x35\x47\x5D\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x46\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x61\x24\x63\x5B\x32\x63\x5D\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x79\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x61\x24\x63\x5B\x34\x6A\x5D\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x60\x3A\x61\x24\x63\x5B\x31\x35\x5D\x2C\x58\x3D\x21\x30\x3D\x3D\x31\x63\x5B\x61\x24\x63\x5B\x32\x6B\x5D\x5D\x3F\x60\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x61\x24\x63\x5B\x34\x59\x5D\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x46\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x61\x24\x63\x5B\x32\x63\x5D\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x79\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x61\x24\x63\x5B\x34\x6A\x5D\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x60\x3A\x61\x24\x63\x5B\x31\x35\x5D\x3B\x31\x64\x5B\x51\x2C\x58\x5D\x7D\x43\x20\x35\x6E\x28\x71\x2C\x79\x29\x7B\x4D\x20\x46\x3D\x21\x30\x3D\x3D\x31\x63\x5B\x61\x24\x63\x5B\x32\x41\x5D\x5D\x7C\x7C\x21\x30\x3D\x3D\x31\x63\x5B\x61\x24\x63\x5B\x32\x6B\x5D\x5D\x3F\x60\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x61\x24\x63\x5B\x34\x6D\x5D\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x71\x2B\x79\x5B\x30\x5D\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x61\x24\x63\x5B\x32\x68\x5D\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x60\x3A\x61\x24\x63\x5B\x31\x35\x5D\x2C\x49\x3D\x21\x30\x3D\x3D\x31\x63\x5B\x61\x24\x63\x5B\x32\x6B\x5D\x5D\x3F\x60\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x61\x24\x63\x5B\x34\x6D\x5D\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x79\x5B\x31\x5D\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x61\x24\x63\x5B\x32\x68\x5D\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x60\x3A\x61\x24\x63\x5B\x31\x35\x5D\x3B\x31\x64\x5B\x46\x2C\x49\x5D\x7D\x43\x20\x35\x6D\x28\x71\x29\x7B\x31\x64\x20\x71\x5B\x61\x24\x63\x5B\x34\x6B\x5D\x5D\x5B\x61\x24\x63\x5B\x31\x30\x5D\x5D\x7D\x43\x20\x35\x64\x28\x71\x2C\x79\x29\x7B\x4D\x20\x46\x3D\x43\x28\x46\x29\x7B\x4D\x20\x49\x3D\x60\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x61\x24\x63\x5B\x35\x65\x5D\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x46\x3F\x61\x24\x63\x5B\x35\x66\x5D\x2B\x46\x3A\x61\x24\x63\x5B\x31\x35\x5D\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x61\x24\x63\x5B\x31\x35\x5D\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x60\x3B\x31\x64\x20\x61\x24\x63\x5B\x35\x67\x5D\x3D\x3D\x71\x5B\x61\x24\x63\x5B\x34\x6B\x5D\x5D\x5B\x61\x24\x63\x5B\x35\x69\x5D\x5D\x3F\x49\x3A\x61\x24\x63\x5B\x35\x6A\x5D\x3D\x3D\x79\x3F\x49\x3A\x61\x24\x63\x5B\x31\x35\x5D\x7D\x2C\x49\x3D\x5B\x61\x24\x63\x5B\x31\x35\x5D\x2C\x46\x28\x29\x2C\x46\x28\x32\x29\x2C\x46\x28\x33\x29\x2C\x46\x28\x34\x29\x5D\x3B\x31\x64\x20\x49\x7D\x43\x20\x34\x58\x28\x71\x29\x7B\x4D\x20\x79\x3D\x71\x5B\x61\x24\x63\x5B\x33\x6E\x5D\x5D\x26\x26\x31\x63\x5B\x61\x24\x63\x5B\x35\x72\x5D\x5D\x3F\x60\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x61\x24\x63\x5B\x34\x52\x5D\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x71\x5B\x61\x24\x63\x5B\x33\x6E\x5D\x5D\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x61\x24\x63\x5B\x38\x32\x5D\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x60\x3A\x61\x24\x63\x5B\x31\x35\x5D\x3B\x31\x64\x20\x79\x7D\x43\x20\x38\x79\x28\x71\x2C\x79\x29\x7B\x4D\x20\x46\x3D\x71\x5B\x61\x24\x63\x5B\x32\x52\x5D\x5D\x26\x26\x31\x63\x5B\x61\x24\x63\x5B\x35\x6C\x5D\x5D\x3F\x60\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x61\x24\x63\x5B\x35\x6B\x5D\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x71\x5B\x61\x24\x63\x5B\x32\x52\x5D\x5D\x5B\x61\x24\x63\x5B\x35\x68\x5D\x5D\x28\x30\x2C\x79\x29\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x61\x24\x63\x5B\x35\x63\x5D\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x60\x3A\x61\x24\x63\x5B\x31\x35\x5D\x3B\x31\x64\x20\x46\x7D\x43\x20\x34\x4A\x28\x71\x29\x7B\x4D\x20\x79\x3D\x71\x5B\x61\x24\x63\x5B\x32\x46\x5D\x5D\x2C\x46\x3D\x71\x5B\x61\x24\x63\x5B\x34\x55\x5D\x5D\x2C\x49\x3D\x71\x5B\x61\x24\x63\x5B\x35\x62\x5D\x5D\x2C\x51\x3D\x71\x5B\x61\x24\x63\x5B\x33\x41\x5D\x5D\x3B\x71\x5B\x61\x24\x63\x5B\x33\x79\x5D\x5D\x2C\x71\x5B\x61\x24\x63\x5B\x33\x78\x5D\x5D\x3B\x4D\x20\x58\x3D\x61\x24\x63\x5B\x31\x35\x5D\x2C\x5A\x3D\x35\x61\x28\x46\x29\x2C\x55\x3D\x34\x5A\x28\x46\x29\x2C\x31\x72\x3D\x28\x34\x58\x28\x46\x29\x2C\x34\x57\x28\x46\x29\x29\x2C\x31\x68\x3D\x34\x56\x28\x46\x29\x2C\x31\x70\x3D\x35\x6D\x28\x46\x29\x2C\x31\x5A\x3D\x35\x64\x28\x46\x2C\x79\x29\x2C\x31\x73\x3D\x35\x6E\x28\x55\x2C\x5A\x29\x3B\x38\x42\x28\x79\x29\x7B\x35\x79\x20\x61\x24\x63\x5B\x37\x39\x5D\x3A\x58\x3D\x49\x21\x3D\x51\x3F\x60\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x61\x24\x63\x5B\x32\x4F\x5D\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x49\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x61\x24\x63\x5B\x32\x51\x5D\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x31\x5A\x5B\x33\x5D\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x61\x24\x63\x5B\x32\x47\x5D\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x31\x68\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x61\x24\x63\x5B\x32\x42\x5D\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x31\x72\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x61\x24\x63\x5B\x33\x62\x5D\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x31\x70\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x61\x24\x63\x5B\x33\x71\x5D\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x31\x68\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x61\x24\x63\x5B\x32\x63\x5D\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x31\x72\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x61\x24\x63\x5B\x33\x44\x5D\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x31\x73\x5B\x31\x5D\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x61\x24\x63\x5B\x33\x43\x5D\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x60\x3A\x61\x24\x63\x5B\x31\x35\x5D\x3B\x33\x6C\x3B\x35\x79\x20\x61\x24\x63\x5B\x31\x57\x5D\x3A\x58\x3D\x49\x21\x3D\x51\x2D\x31\x3F\x60\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x61\x24\x63\x5B\x32\x4F\x5D\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x49\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x61\x24\x63\x5B\x32\x51\x5D\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x31\x5A\x5B\x32\x5D\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x61\x24\x63\x5B\x32\x47\x5D\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x31\x68\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x61\x24\x63\x5B\x32\x42\x5D\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x31\x72\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x61\x24\x63\x5B\x33\x62\x5D\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x31\x70\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x61\x24\x63\x5B\x33\x71\x5D\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x31\x68\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x61\x24\x63\x5B\x32\x63\x5D\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x31\x72\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x61\x24\x63\x5B\x33\x44\x5D\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x31\x73\x5B\x31\x5D\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x61\x24\x63\x5B\x33\x43\x5D\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x60\x3A\x61\x24\x63\x5B\x31\x35\x5D\x7D\x3B\x31\x64\x20\x58\x7D\x43\x20\x34\x6F\x28\x71\x29\x7B\x4D\x20\x79\x3D\x24\x5B\x61\x24\x63\x5B\x32\x48\x5D\x5D\x28\x7B\x33\x47\x3A\x33\x77\x28\x71\x2C\x61\x24\x63\x5B\x38\x34\x5D\x29\x2C\x32\x72\x3A\x61\x24\x63\x5B\x33\x76\x5D\x2C\x35\x75\x3A\x21\x31\x2C\x35\x74\x3A\x61\x24\x63\x5B\x35\x32\x5D\x2C\x35\x73\x3A\x21\x30\x2C\x33\x54\x3A\x43\x28\x71\x29\x7B\x31\x64\x20\x71\x7D\x7D\x29\x5B\x61\x24\x63\x5B\x35\x7A\x5D\x5D\x2C\x46\x3D\x34\x54\x5B\x61\x24\x63\x5B\x33\x6F\x5D\x5D\x28\x24\x28\x79\x29\x5B\x61\x24\x63\x5B\x59\x5D\x5D\x28\x61\x24\x63\x5B\x33\x70\x5D\x29\x5B\x61\x24\x63\x5B\x31\x6D\x5D\x5D\x28\x29\x29\x2C\x49\x3D\x46\x5B\x61\x24\x63\x5B\x33\x6D\x5D\x5D\x3B\x31\x64\x20\x49\x7D\x43\x20\x34\x69\x28\x71\x29\x7B\x4D\x20\x79\x3D\x71\x5B\x61\x24\x63\x5B\x35\x78\x5D\x5D\x2C\x46\x3D\x71\x5B\x61\x24\x63\x5B\x32\x46\x5D\x5D\x2C\x49\x3D\x71\x5B\x61\x24\x63\x5B\x33\x41\x5D\x5D\x2C\x51\x3D\x71\x5B\x61\x24\x63\x5B\x32\x66\x5D\x5D\x3F\x71\x5B\x61\x24\x63\x5B\x32\x66\x5D\x5D\x3A\x61\x24\x63\x5B\x38\x34\x5D\x2C\x58\x3D\x71\x5B\x61\x24\x63\x5B\x38\x39\x5D\x5D\x2C\x5A\x3D\x71\x5B\x61\x24\x63\x5B\x33\x7A\x5D\x5D\x2C\x55\x3D\x71\x5B\x61\x24\x63\x5B\x33\x79\x5D\x5D\x2C\x31\x72\x3D\x71\x5B\x61\x24\x63\x5B\x33\x78\x5D\x5D\x3B\x24\x5B\x61\x24\x63\x5B\x32\x48\x5D\x5D\x28\x7B\x33\x47\x3A\x61\x24\x63\x5B\x37\x39\x5D\x21\x3D\x46\x3F\x33\x77\x28\x49\x2C\x51\x29\x3A\x5A\x2C\x32\x72\x3A\x61\x24\x63\x5B\x33\x76\x5D\x2C\x35\x75\x3A\x21\x30\x2C\x35\x74\x3A\x61\x24\x63\x5B\x35\x32\x5D\x2C\x35\x73\x3A\x21\x30\x2C\x37\x62\x3A\x43\x28\x71\x29\x7B\x61\x24\x63\x5B\x37\x39\x5D\x3D\x3D\x3D\x46\x3F\x79\x5B\x61\x24\x63\x5B\x35\x32\x5D\x5D\x28\x33\x72\x28\x29\x29\x5B\x61\x24\x63\x5B\x36\x36\x5D\x5D\x28\x61\x24\x63\x5B\x34\x32\x5D\x29\x5B\x61\x24\x63\x5B\x36\x37\x5D\x5D\x28\x29\x5B\x61\x24\x63\x5B\x33\x31\x5D\x5D\x28\x61\x24\x63\x5B\x36\x35\x5D\x29\x5B\x61\x24\x63\x5B\x59\x5D\x5D\x28\x61\x24\x63\x5B\x34\x53\x5D\x29\x5B\x61\x24\x63\x5B\x31\x49\x5D\x5D\x28\x29\x3A\x79\x5B\x61\x24\x63\x5B\x35\x32\x5D\x5D\x28\x33\x72\x28\x29\x29\x7D\x2C\x33\x54\x3A\x43\x28\x71\x29\x7B\x4D\x20\x5A\x3D\x61\x24\x63\x5B\x31\x35\x5D\x2C\x31\x68\x3D\x30\x2C\x31\x70\x3D\x21\x31\x3B\x5A\x3D\x60\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x61\x24\x63\x5B\x35\x71\x5D\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x46\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x61\x24\x63\x5B\x35\x6F\x5D\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x60\x3B\x4D\x20\x31\x5A\x3D\x24\x28\x71\x29\x5B\x61\x24\x63\x5B\x59\x5D\x5D\x28\x61\x24\x63\x5B\x33\x70\x5D\x29\x3B\x31\x7A\x28\x31\x5A\x5B\x61\x24\x63\x5B\x35\x35\x5D\x5D\x29\x7B\x4D\x20\x31\x73\x3D\x34\x54\x5B\x61\x24\x63\x5B\x33\x6F\x5D\x5D\x28\x31\x5A\x5B\x61\x24\x63\x5B\x31\x6D\x5D\x5D\x28\x29\x29\x5B\x61\x24\x63\x5B\x33\x6D\x5D\x5D\x3B\x31\x7A\x28\x31\x73\x29\x7B\x31\x7A\x28\x61\x24\x63\x5B\x31\x57\x5D\x3D\x3D\x46\x29\x7B\x31\x3D\x3D\x31\x73\x5B\x61\x24\x63\x5B\x35\x35\x5D\x5D\x26\x26\x61\x24\x63\x5B\x38\x34\x5D\x21\x3D\x51\x26\x26\x28\x31\x73\x3D\x34\x6F\x28\x49\x29\x29\x3B\x4D\x20\x34\x70\x3D\x31\x73\x5B\x61\x24\x63\x5B\x35\x35\x5D\x5D\x3B\x32\x69\x28\x4D\x20\x32\x78\x3D\x30\x3B\x32\x78\x3C\x34\x70\x3B\x32\x78\x2B\x2B\x29\x7B\x4D\x20\x34\x7A\x3D\x31\x73\x5B\x32\x78\x5D\x3B\x31\x7A\x28\x31\x21\x3D\x31\x73\x5B\x61\x24\x63\x5B\x35\x35\x5D\x5D\x26\x26\x34\x76\x28\x34\x7A\x29\x3D\x3D\x58\x29\x7B\x31\x73\x5B\x61\x24\x63\x5B\x34\x43\x5D\x5D\x28\x32\x78\x2C\x31\x29\x3B\x33\x6C\x7D\x7D\x7D\x3B\x4D\x20\x33\x6A\x3D\x31\x73\x5B\x61\x24\x63\x5B\x35\x35\x5D\x5D\x3B\x32\x69\x28\x4D\x20\x32\x71\x3D\x30\x3B\x32\x71\x3C\x33\x6A\x3B\x32\x71\x2B\x2B\x29\x7B\x4D\x20\x34\x4C\x3D\x31\x73\x5B\x32\x71\x5D\x3B\x5A\x2B\x3D\x34\x4A\x28\x7B\x32\x72\x3A\x46\x2C\x38\x6A\x3A\x34\x4C\x2C\x38\x70\x3A\x32\x71\x2C\x34\x67\x3A\x49\x2C\x38\x6F\x3A\x55\x2C\x38\x74\x3A\x31\x72\x7D\x29\x7D\x3B\x31\x68\x3D\x33\x6A\x7D\x34\x4E\x7B\x31\x70\x3D\x21\x30\x7D\x7D\x34\x4E\x7B\x31\x70\x3D\x21\x30\x7D\x3B\x5A\x2B\x3D\x61\x24\x63\x5B\x32\x68\x5D\x2C\x5A\x3D\x31\x70\x3F\x33\x68\x28\x46\x29\x3A\x5A\x2C\x79\x5B\x61\x24\x63\x5B\x35\x32\x5D\x5D\x28\x5A\x29\x2C\x61\x24\x63\x5B\x37\x39\x5D\x3D\x3D\x46\x26\x26\x28\x49\x3C\x31\x68\x26\x26\x79\x5B\x61\x24\x63\x5B\x36\x37\x5D\x5D\x28\x29\x5B\x61\x24\x63\x5B\x31\x44\x5D\x5D\x28\x60\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x61\x24\x63\x5B\x34\x4F\x5D\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x51\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x61\x24\x63\x5B\x34\x50\x5D\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x31\x63\x5B\x61\x24\x63\x5B\x34\x51\x5D\x5D\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x61\x24\x63\x5B\x34\x44\x5D\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x60\x29\x2C\x31\x54\x28\x43\x28\x29\x7B\x79\x5B\x61\x24\x63\x5B\x33\x31\x5D\x5D\x28\x61\x24\x63\x5B\x34\x32\x5D\x29\x7D\x2C\x35\x48\x29\x29\x2C\x61\x24\x63\x5B\x37\x39\x5D\x3D\x3D\x3D\x46\x3F\x79\x5B\x61\x24\x63\x5B\x59\x5D\x5D\x28\x61\x24\x63\x5B\x33\x69\x5D\x29\x5B\x61\x24\x63\x5B\x31\x5D\x5D\x28\x7B\x34\x42\x3A\x21\x31\x7D\x29\x3A\x79\x5B\x61\x24\x63\x5B\x59\x5D\x5D\x28\x61\x24\x63\x5B\x33\x69\x5D\x29\x5B\x61\x24\x63\x5B\x31\x5D\x5D\x28\x29\x7D\x2C\x38\x6E\x3A\x43\x28\x29\x7B\x79\x5B\x61\x24\x63\x5B\x35\x32\x5D\x5D\x28\x33\x68\x28\x46\x29\x29\x7D\x7D\x29\x7D\x43\x20\x33\x45\x28\x71\x2C\x79\x29\x7B\x4D\x20\x46\x3D\x71\x5B\x61\x24\x63\x5B\x36\x33\x5D\x5D\x28\x29\x2C\x49\x3D\x46\x5B\x61\x24\x63\x5B\x35\x36\x5D\x5D\x28\x29\x3B\x61\x24\x63\x5B\x31\x35\x5D\x21\x3D\x49\x26\x26\x49\x21\x3D\x33\x66\x5B\x61\x24\x63\x5B\x35\x37\x5D\x5D\x26\x26\x28\x33\x66\x5B\x61\x24\x63\x5B\x35\x37\x5D\x5D\x3D\x49\x2C\x34\x69\x28\x7B\x74\x3A\x79\x2C\x32\x72\x3A\x61\x24\x63\x5B\x37\x39\x5D\x2C\x34\x67\x3A\x34\x2C\x36\x72\x3A\x49\x2C\x38\x76\x3A\x60\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x61\x24\x63\x5B\x34\x49\x5D\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x49\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x61\x24\x63\x5B\x34\x48\x5D\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x60\x7D\x29\x29\x7D\x43\x20\x32\x4B\x28\x71\x29\x7B\x24\x28\x71\x29\x5B\x61\x24\x63\x5B\x35\x31\x5D\x5D\x28\x43\x28\x29\x7B\x31\x7A\x28\x31\x63\x5B\x61\x24\x63\x5B\x34\x47\x5D\x5D\x29\x7B\x4D\x20\x71\x3D\x31\x63\x5B\x61\x24\x63\x5B\x33\x56\x5D\x5D\x3F\x24\x28\x61\x24\x63\x5B\x33\x53\x5D\x29\x5B\x61\x24\x63\x5B\x35\x5D\x5D\x28\x29\x2B\x33\x30\x3A\x33\x30\x3B\x24\x28\x56\x29\x5B\x61\x24\x63\x5B\x34\x46\x5D\x5D\x28\x7B\x38\x4A\x3A\x61\x24\x63\x5B\x34\x45\x5D\x2C\x38\x45\x3A\x71\x2C\x38\x46\x3A\x33\x30\x7D\x29\x7D\x7D\x29\x7D\x43\x20\x35\x53\x28\x71\x29\x7B\x24\x28\x71\x29\x5B\x61\x24\x63\x5B\x33\x35\x5D\x5D\x28\x61\x24\x63\x5B\x31\x30\x5D\x2C\x43\x28\x71\x2C\x79\x29\x7B\x4D\x20\x46\x3D\x61\x24\x63\x5B\x34\x71\x5D\x3B\x31\x64\x20\x79\x3D\x79\x5B\x61\x24\x63\x5B\x32\x38\x5D\x5D\x28\x61\x24\x63\x5B\x34\x78\x5D\x2C\x46\x29\x5B\x61\x24\x63\x5B\x32\x38\x5D\x5D\x28\x61\x24\x63\x5B\x34\x77\x5D\x2C\x46\x29\x5B\x61\x24\x63\x5B\x32\x38\x5D\x5D\x28\x61\x24\x63\x5B\x31\x46\x5D\x2C\x61\x24\x63\x5B\x34\x73\x5D\x29\x5B\x61\x24\x63\x5B\x32\x38\x5D\x5D\x28\x61\x24\x63\x5B\x34\x41\x5D\x2C\x61\x24\x63\x5B\x34\x72\x5D\x29\x7D\x29\x7D\x24\x28\x61\x24\x63\x5B\x34\x75\x5D\x29\x5B\x61\x24\x63\x5B\x34\x79\x5D\x5D\x28\x29\x2C\x24\x28\x61\x24\x63\x5B\x35\x4A\x5D\x29\x5B\x61\x24\x63\x5B\x34\x39\x5D\x5D\x28\x61\x24\x63\x5B\x36\x39\x5D\x2C\x43\x28\x71\x29\x7B\x33\x4E\x28\x29\x2C\x33\x61\x28\x29\x7D\x29\x2C\x24\x77\x5B\x61\x24\x63\x5B\x34\x39\x5D\x5D\x28\x61\x24\x63\x5B\x37\x31\x5D\x2C\x43\x28\x71\x29\x7B\x71\x5B\x61\x24\x63\x5B\x32\x75\x5D\x5D\x26\x26\x37\x35\x3D\x3D\x71\x5B\x61\x24\x63\x5B\x37\x32\x5D\x5D\x26\x26\x28\x71\x5B\x61\x24\x63\x5B\x31\x41\x5D\x5D\x28\x29\x2C\x33\x4E\x28\x29\x2C\x33\x61\x28\x29\x29\x7D\x29\x2C\x24\x28\x61\x24\x63\x5B\x35\x52\x5D\x29\x5B\x61\x24\x63\x5B\x35\x31\x5D\x5D\x28\x43\x28\x29\x7B\x4D\x20\x71\x3D\x24\x28\x56\x29\x2C\x79\x3D\x71\x5B\x61\x24\x63\x5B\x33\x35\x5D\x5D\x28\x61\x24\x63\x5B\x37\x35\x5D\x29\x2C\x46\x3D\x79\x5B\x61\x24\x63\x5B\x32\x33\x5D\x5D\x28\x61\x24\x63\x5B\x37\x54\x5D\x29\x2C\x49\x3D\x71\x5B\x61\x24\x63\x5B\x31\x31\x5D\x5D\x28\x61\x24\x63\x5B\x31\x6D\x5D\x29\x3B\x31\x7A\x28\x46\x5B\x31\x5D\x26\x26\x21\x30\x3D\x3D\x49\x29\x7B\x4D\x20\x51\x3D\x46\x5B\x31\x5D\x5B\x61\x24\x63\x5B\x35\x36\x5D\x5D\x28\x29\x3B\x61\x24\x63\x5B\x31\x35\x5D\x21\x3D\x51\x26\x26\x71\x5B\x61\x24\x63\x5B\x31\x44\x5D\x5D\x28\x60\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x61\x24\x63\x5B\x37\x4D\x5D\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x51\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x61\x24\x63\x5B\x38\x32\x5D\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x60\x29\x7D\x3B\x71\x5B\x61\x24\x63\x5B\x33\x35\x5D\x5D\x28\x61\x24\x63\x5B\x37\x35\x5D\x2C\x46\x5B\x30\x5D\x5B\x61\x24\x63\x5B\x35\x36\x5D\x5D\x28\x29\x29\x7D\x29\x2C\x24\x28\x61\x24\x63\x5B\x37\x77\x5D\x29\x5B\x61\x24\x63\x5B\x35\x31\x5D\x5D\x28\x43\x28\x29\x7B\x4D\x20\x71\x3D\x24\x28\x56\x29\x2C\x79\x3D\x71\x5B\x61\x24\x63\x5B\x31\x31\x5D\x5D\x28\x61\x24\x63\x5B\x32\x44\x5D\x29\x3B\x31\x7A\x28\x79\x29\x7B\x4D\x20\x46\x3D\x31\x76\x28\x79\x2C\x61\x24\x63\x5B\x33\x64\x5D\x29\x2C\x49\x3D\x31\x76\x28\x79\x2C\x61\x24\x63\x5B\x31\x6D\x5D\x29\x3B\x21\x31\x21\x3D\x46\x26\x26\x71\x5B\x61\x24\x63\x5B\x59\x5D\x5D\x28\x61\x24\x63\x5B\x37\x41\x5D\x29\x5B\x61\x24\x63\x5B\x35\x32\x5D\x5D\x28\x46\x29\x2C\x21\x31\x21\x3D\x49\x26\x26\x71\x5B\x61\x24\x63\x5B\x59\x5D\x5D\x28\x61\x24\x63\x5B\x37\x42\x5D\x29\x5B\x61\x24\x63\x5B\x35\x32\x5D\x5D\x28\x49\x29\x7D\x7D\x29\x2C\x24\x28\x61\x24\x63\x5B\x37\x45\x5D\x29\x5B\x61\x24\x63\x5B\x35\x31\x5D\x5D\x28\x43\x28\x29\x7B\x4D\x20\x71\x3D\x24\x28\x56\x29\x2C\x79\x3D\x71\x5B\x61\x24\x63\x5B\x31\x6D\x5D\x5D\x28\x29\x3B\x43\x20\x46\x28\x71\x29\x7B\x31\x64\x20\x79\x5B\x61\x24\x63\x5B\x35\x36\x5D\x5D\x28\x29\x5B\x61\x24\x63\x5B\x31\x33\x5D\x5D\x28\x71\x29\x7D\x43\x20\x49\x28\x79\x2C\x49\x29\x7B\x46\x28\x79\x29\x26\x26\x28\x24\x62\x5B\x61\x24\x63\x5B\x33\x31\x5D\x5D\x28\x49\x29\x2C\x71\x5B\x61\x24\x63\x5B\x31\x49\x5D\x5D\x28\x29\x2C\x61\x24\x63\x5B\x33\x67\x5D\x3D\x3D\x49\x26\x26\x24\x62\x5B\x61\x24\x63\x5B\x36\x36\x5D\x5D\x28\x61\x24\x63\x5B\x33\x65\x5D\x29\x29\x7D\x46\x28\x61\x24\x63\x5B\x38\x69\x5D\x29\x26\x26\x28\x71\x5B\x61\x24\x63\x5B\x31\x59\x5D\x5D\x28\x61\x24\x63\x5B\x37\x6F\x5D\x29\x2C\x24\x28\x61\x24\x63\x5B\x37\x4A\x5D\x29\x5B\x61\x24\x63\x5B\x31\x44\x5D\x5D\x28\x24\x28\x61\x24\x63\x5B\x37\x49\x5D\x29\x29\x29\x3B\x4D\x20\x51\x3D\x5B\x7B\x31\x47\x3A\x61\x24\x63\x5B\x37\x48\x5D\x2C\x31\x51\x3A\x61\x24\x63\x5B\x33\x65\x5D\x7D\x2C\x7B\x31\x47\x3A\x61\x24\x63\x5B\x35\x49\x5D\x2C\x31\x51\x3A\x61\x24\x63\x5B\x33\x67\x5D\x7D\x2C\x7B\x31\x47\x3A\x61\x24\x63\x5B\x37\x46\x5D\x2C\x31\x51\x3A\x61\x24\x63\x5B\x37\x6C\x5D\x7D\x5D\x3B\x32\x69\x28\x4D\x20\x58\x20\x37\x4B\x20\x51\x29\x7B\x49\x28\x51\x5B\x58\x5D\x5B\x61\x24\x63\x5B\x33\x74\x5D\x5D\x2C\x51\x5B\x58\x5D\x5B\x61\x24\x63\x5B\x33\x75\x5D\x5D\x29\x7D\x7D\x29\x2C\x24\x28\x61\x24\x63\x5B\x37\x76\x5D\x29\x5B\x61\x24\x63\x5B\x35\x31\x5D\x5D\x28\x43\x28\x29\x7B\x4D\x20\x71\x3D\x24\x28\x56\x29\x2C\x79\x3D\x71\x5B\x61\x24\x63\x5B\x31\x6D\x5D\x5D\x28\x29\x2C\x46\x3D\x31\x76\x28\x79\x2C\x61\x24\x63\x5B\x31\x6D\x5D\x29\x3B\x79\x5B\x61\x24\x63\x5B\x31\x33\x5D\x5D\x28\x61\x24\x63\x5B\x38\x61\x5D\x29\x26\x26\x46\x26\x26\x28\x71\x5B\x61\x24\x63\x5B\x32\x74\x5D\x5D\x28\x2F\x28\x5B\x5E\x7B\x5C\x7D\x5D\x2B\x28\x3F\x3D\x7D\x29\x29\x2F\x67\x2C\x61\x24\x63\x5B\x38\x65\x5D\x29\x2C\x71\x5B\x61\x24\x63\x5B\x59\x5D\x5D\x28\x61\x24\x63\x5B\x37\x56\x5D\x29\x5B\x61\x24\x63\x5B\x32\x74\x5D\x5D\x28\x61\x24\x63\x5B\x35\x34\x5D\x2C\x61\x24\x63\x5B\x32\x4E\x5D\x29\x2C\x71\x5B\x61\x24\x63\x5B\x35\x31\x5D\x5D\x28\x43\x28\x29\x7B\x4D\x20\x71\x3D\x24\x28\x56\x29\x2C\x79\x3D\x71\x5B\x61\x24\x63\x5B\x31\x6D\x5D\x5D\x28\x29\x2C\x46\x3D\x31\x76\x28\x79\x2C\x61\x24\x63\x5B\x31\x6D\x5D\x29\x2C\x49\x3D\x31\x76\x28\x79\x2C\x61\x24\x63\x5B\x37\x4F\x5D\x29\x2C\x51\x3D\x31\x76\x28\x79\x2C\x61\x24\x63\x5B\x33\x6B\x5D\x29\x2C\x58\x3D\x31\x76\x28\x79\x2C\x61\x24\x63\x5B\x37\x47\x5D\x29\x2C\x5A\x3D\x31\x76\x28\x79\x2C\x61\x24\x63\x5B\x33\x63\x5D\x29\x2C\x55\x3D\x71\x5B\x61\x24\x63\x5B\x36\x37\x5D\x5D\x28\x29\x5B\x61\x24\x63\x5B\x33\x35\x5D\x5D\x28\x61\x24\x63\x5B\x33\x32\x5D\x29\x3B\x71\x5B\x61\x24\x63\x5B\x33\x31\x5D\x5D\x28\x58\x3F\x61\x24\x63\x5B\x37\x6B\x5D\x3A\x61\x24\x63\x5B\x37\x51\x5D\x29\x5B\x61\x24\x63\x5B\x31\x6D\x5D\x5D\x28\x46\x5B\x61\x24\x63\x5B\x32\x38\x5D\x5D\x28\x61\x24\x63\x5B\x32\x4E\x5D\x2C\x61\x24\x63\x5B\x35\x34\x5D\x29\x29\x2C\x21\x31\x21\x3D\x49\x26\x26\x71\x5B\x61\x24\x63\x5B\x33\x31\x5D\x5D\x28\x49\x29\x2C\x51\x26\x26\x71\x5B\x61\x24\x63\x5B\x33\x31\x5D\x5D\x28\x61\x24\x63\x5B\x33\x6B\x5D\x29\x5B\x61\x24\x63\x5B\x33\x35\x5D\x5D\x28\x61\x24\x63\x5B\x33\x32\x5D\x2C\x60\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x61\x24\x63\x5B\x37\x58\x5D\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x51\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x61\x24\x63\x5B\x37\x57\x5D\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x60\x29\x2C\x55\x26\x26\x55\x5B\x61\x24\x63\x5B\x31\x33\x5D\x5D\x28\x61\x24\x63\x5B\x38\x67\x5D\x29\x26\x26\x71\x5B\x61\x24\x63\x5B\x33\x31\x5D\x5D\x28\x61\x24\x63\x5B\x38\x66\x5D\x29\x2C\x5A\x26\x26\x28\x71\x5B\x61\x24\x63\x5B\x33\x31\x5D\x5D\x28\x49\x3F\x61\x24\x63\x5B\x37\x5A\x5D\x2B\x49\x3A\x61\x24\x63\x5B\x38\x64\x5D\x29\x2C\x71\x5B\x61\x24\x63\x5B\x31\x44\x5D\x5D\x28\x60\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x61\x24\x63\x5B\x38\x63\x5D\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x5A\x5B\x61\x24\x63\x5B\x32\x38\x5D\x5D\x28\x61\x24\x63\x5B\x32\x4E\x5D\x2C\x61\x24\x63\x5B\x35\x34\x5D\x29\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x61\x24\x63\x5B\x38\x32\x5D\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x60\x29\x29\x7D\x29\x29\x7D\x29\x2C\x24\x28\x61\x24\x63\x5B\x37\x75\x5D\x29\x5B\x61\x24\x63\x5B\x35\x31\x5D\x5D\x28\x43\x28\x29\x7B\x4D\x20\x71\x3D\x24\x28\x56\x29\x2C\x79\x3D\x5B\x7B\x31\x47\x3A\x61\x24\x63\x5B\x37\x44\x5D\x2C\x31\x51\x3A\x61\x24\x63\x5B\x37\x43\x5D\x7D\x2C\x7B\x31\x47\x3A\x61\x24\x63\x5B\x37\x78\x5D\x2C\x31\x51\x3A\x61\x24\x63\x5B\x33\x63\x5D\x7D\x2C\x7B\x31\x47\x3A\x61\x24\x63\x5B\x37\x74\x5D\x2C\x31\x51\x3A\x61\x24\x63\x5B\x37\x73\x5D\x7D\x2C\x7B\x31\x47\x3A\x61\x24\x63\x5B\x37\x72\x5D\x2C\x31\x51\x3A\x61\x24\x63\x5B\x37\x71\x5D\x7D\x2C\x7B\x31\x47\x3A\x61\x24\x63\x5B\x37\x70\x5D\x2C\x31\x51\x3A\x61\x24\x63\x5B\x33\x73\x5D\x7D\x5D\x2C\x46\x3D\x71\x5B\x61\x24\x63\x5B\x31\x6D\x5D\x5D\x28\x29\x2C\x49\x3D\x71\x5B\x61\x24\x63\x5B\x35\x32\x5D\x5D\x28\x29\x3B\x43\x20\x51\x28\x79\x2C\x51\x29\x7B\x46\x5B\x61\x24\x63\x5B\x35\x36\x5D\x5D\x28\x29\x5B\x61\x24\x63\x5B\x31\x33\x5D\x5D\x28\x79\x29\x26\x26\x28\x49\x3D\x49\x5B\x61\x24\x63\x5B\x32\x38\x5D\x5D\x28\x79\x2C\x61\x24\x63\x5B\x31\x35\x5D\x29\x2C\x71\x5B\x61\x24\x63\x5B\x31\x59\x5D\x5D\x28\x61\x24\x63\x5B\x33\x73\x5D\x21\x3D\x51\x3F\x60\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x61\x24\x63\x5B\x37\x4C\x5D\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x51\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x61\x24\x63\x5B\x32\x63\x5D\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x49\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x61\x24\x63\x5B\x32\x68\x5D\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x60\x3A\x60\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x61\x24\x63\x5B\x37\x6E\x5D\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x49\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x61\x24\x63\x5B\x37\x6D\x5D\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x60\x29\x29\x7D\x32\x69\x28\x4D\x20\x58\x20\x37\x4B\x20\x79\x29\x7B\x51\x28\x79\x5B\x58\x5D\x5B\x61\x24\x63\x5B\x33\x74\x5D\x5D\x2C\x79\x5B\x58\x5D\x5B\x61\x24\x63\x5B\x33\x75\x5D\x5D\x29\x7D\x7D\x29\x2C\x24\x28\x61\x24\x63\x5B\x37\x79\x5D\x29\x5B\x61\x24\x63\x5B\x34\x39\x5D\x5D\x28\x61\x24\x63\x5B\x36\x39\x5D\x2C\x43\x28\x71\x29\x7B\x71\x5B\x61\x24\x63\x5B\x31\x41\x5D\x5D\x28\x29\x3B\x4D\x20\x79\x3D\x24\x28\x56\x29\x2C\x46\x3D\x79\x5B\x61\x24\x63\x5B\x33\x35\x5D\x5D\x28\x61\x24\x63\x5B\x37\x35\x5D\x29\x2C\x49\x3D\x32\x6A\x5B\x61\x24\x63\x5B\x37\x37\x5D\x5D\x28\x46\x2C\x61\x24\x63\x5B\x37\x55\x5D\x2C\x61\x24\x63\x5B\x38\x62\x5D\x29\x3B\x49\x5B\x61\x24\x63\x5B\x36\x31\x5D\x5D\x28\x29\x7D\x29\x2C\x24\x77\x5B\x61\x24\x63\x5B\x34\x39\x5D\x5D\x28\x61\x24\x63\x5B\x37\x31\x5D\x2C\x43\x28\x71\x29\x7B\x31\x63\x5B\x61\x24\x63\x5B\x32\x59\x5D\x5D\x26\x26\x71\x5B\x61\x24\x63\x5B\x32\x75\x5D\x5D\x26\x26\x38\x33\x3D\x3D\x71\x5B\x61\x24\x63\x5B\x37\x32\x5D\x5D\x26\x26\x28\x71\x5B\x61\x24\x63\x5B\x31\x41\x5D\x5D\x28\x29\x2C\x33\x42\x28\x29\x29\x7D\x29\x2C\x24\x28\x61\x24\x63\x5B\x38\x68\x5D\x29\x5B\x61\x24\x63\x5B\x34\x39\x5D\x5D\x28\x61\x24\x63\x5B\x36\x39\x5D\x2C\x43\x28\x29\x7B\x33\x42\x28\x29\x7D\x29\x2C\x24\x28\x61\x24\x63\x5B\x37\x59\x5D\x29\x5B\x61\x24\x63\x5B\x35\x31\x5D\x5D\x28\x43\x28\x29\x7B\x4D\x20\x71\x3D\x24\x28\x56\x29\x2C\x79\x3D\x71\x5B\x61\x24\x63\x5B\x32\x76\x5D\x5D\x28\x61\x24\x63\x5B\x32\x54\x5D\x29\x3B\x79\x5B\x61\x24\x63\x5B\x34\x39\x5D\x5D\x28\x61\x24\x63\x5B\x36\x39\x5D\x2C\x43\x28\x29\x7B\x56\x5B\x61\x24\x63\x5B\x37\x4E\x5D\x5D\x28\x29\x7D\x29\x2C\x71\x5B\x61\x24\x63\x5B\x32\x76\x5D\x5D\x28\x61\x24\x63\x5B\x32\x53\x5D\x29\x5B\x61\x24\x63\x5B\x34\x39\x5D\x5D\x28\x61\x24\x63\x5B\x36\x39\x5D\x2C\x43\x28\x29\x7B\x38\x4B\x5B\x61\x24\x63\x5B\x37\x53\x5D\x5D\x5B\x61\x24\x63\x5B\x37\x52\x5D\x5D\x28\x79\x5B\x61\x24\x63\x5B\x36\x33\x5D\x5D\x28\x29\x29\x2C\x71\x5B\x61\x24\x63\x5B\x36\x36\x5D\x5D\x28\x61\x24\x63\x5B\x32\x50\x5D\x29\x5B\x61\x24\x63\x5B\x33\x31\x5D\x5D\x28\x61\x24\x63\x5B\x32\x5A\x5D\x29\x2C\x31\x54\x28\x43\x28\x29\x7B\x71\x5B\x61\x24\x63\x5B\x36\x36\x5D\x5D\x28\x61\x24\x63\x5B\x32\x5A\x5D\x29\x5B\x61\x24\x63\x5B\x33\x31\x5D\x5D\x28\x61\x24\x63\x5B\x32\x50\x5D\x29\x7D\x2C\x38\x44\x29\x7D\x29\x7D\x29\x2C\x24\x28\x61\x24\x63\x5B\x37\x50\x5D\x29\x5B\x61\x24\x63\x5B\x35\x31\x5D\x5D\x28\x43\x28\x29\x7B\x4D\x20\x71\x3D\x24\x28\x56\x29\x2C\x79\x3D\x71\x5B\x61\x24\x63\x5B\x59\x5D\x5D\x28\x61\x24\x63\x5B\x37\x7A\x5D\x29\x3B\x79\x5B\x61\x24\x63\x5B\x35\x35\x5D\x5D\x26\x26\x28\x79\x5B\x61\x24\x63\x5B\x35\x31\x5D\x5D\x28\x43\x28\x29\x7B\x4D\x20\x71\x3D\x24\x28\x56\x29\x2C\x79\x3D\x71\x5B\x61\x24\x63\x5B\x31\x6D\x5D\x5D\x28\x29\x5B\x61\x24\x63\x5B\x35\x36\x5D\x5D\x28\x29\x2C\x46\x3D\x71\x5B\x61\x24\x63\x5B\x33\x35\x5D\x5D\x28\x61\x24\x63\x5B\x37\x35\x5D\x29\x2C\x49\x3D\x61\x24\x63\x5B\x36\x77\x5D\x3D\x3D\x79\x3F\x61\x24\x63\x5B\x37\x69\x5D\x3A\x79\x3B\x71\x5B\x61\x24\x63\x5B\x31\x59\x5D\x5D\x28\x60\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x61\x24\x63\x5B\x36\x65\x5D\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x49\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x61\x24\x63\x5B\x36\x66\x5D\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x49\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x61\x24\x63\x5B\x32\x47\x5D\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x46\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x61\x24\x63\x5B\x32\x42\x5D\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x49\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x61\x24\x63\x5B\x36\x67\x5D\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x60\x29\x7D\x29\x2C\x71\x5B\x61\x24\x63\x5B\x36\x37\x5D\x5D\x28\x29\x5B\x61\x24\x63\x5B\x31\x44\x5D\x5D\x28\x61\x24\x63\x5B\x36\x68\x5D\x29\x2C\x71\x5B\x61\x24\x63\x5B\x59\x5D\x5D\x28\x61\x24\x63\x5B\x36\x69\x5D\x29\x5B\x61\x24\x63\x5B\x32\x49\x5D\x5D\x28\x71\x5B\x61\x24\x63\x5B\x36\x37\x5D\x5D\x28\x29\x5B\x61\x24\x63\x5B\x59\x5D\x5D\x28\x61\x24\x63\x5B\x36\x6A\x5D\x29\x29\x29\x7D\x29\x2C\x24\x77\x5B\x61\x24\x63\x5B\x34\x39\x5D\x5D\x28\x61\x24\x63\x5B\x37\x31\x5D\x2C\x43\x28\x71\x29\x7B\x31\x63\x5B\x61\x24\x63\x5B\x32\x59\x5D\x5D\x26\x26\x28\x71\x5B\x61\x24\x63\x5B\x32\x75\x5D\x5D\x26\x26\x33\x37\x3D\x3D\x71\x5B\x61\x24\x63\x5B\x37\x32\x5D\x5D\x3F\x28\x71\x5B\x61\x24\x63\x5B\x31\x41\x5D\x5D\x28\x29\x2C\x32\x58\x28\x31\x63\x5B\x61\x24\x63\x5B\x32\x57\x5D\x5D\x3F\x61\x24\x63\x5B\x32\x56\x5D\x3A\x61\x24\x63\x5B\x32\x55\x5D\x29\x29\x3A\x71\x5B\x61\x24\x63\x5B\x32\x75\x5D\x5D\x26\x26\x33\x39\x3D\x3D\x71\x5B\x61\x24\x63\x5B\x37\x32\x5D\x5D\x26\x26\x28\x71\x5B\x61\x24\x63\x5B\x31\x41\x5D\x5D\x28\x29\x2C\x32\x58\x28\x31\x63\x5B\x61\x24\x63\x5B\x32\x57\x5D\x5D\x3F\x61\x24\x63\x5B\x32\x55\x5D\x3A\x61\x24\x63\x5B\x32\x56\x5D\x29\x29\x29\x7D\x29\x2C\x24\x28\x61\x24\x63\x5B\x36\x6B\x5D\x29\x5B\x61\x24\x63\x5B\x35\x31\x5D\x5D\x28\x43\x28\x29\x7B\x4D\x20\x71\x3D\x24\x28\x56\x29\x2C\x79\x3D\x71\x5B\x61\x24\x63\x5B\x59\x5D\x5D\x28\x61\x24\x63\x5B\x32\x54\x5D\x29\x2C\x46\x3D\x71\x5B\x61\x24\x63\x5B\x59\x5D\x5D\x28\x61\x24\x63\x5B\x32\x53\x5D\x29\x2C\x49\x3D\x71\x5B\x61\x24\x63\x5B\x59\x5D\x5D\x28\x61\x24\x63\x5B\x36\x38\x5D\x29\x3B\x46\x5B\x61\x24\x63\x5B\x34\x39\x5D\x5D\x28\x61\x24\x63\x5B\x36\x39\x5D\x2C\x43\x28\x29\x7B\x33\x45\x28\x79\x2C\x49\x29\x7D\x29\x2C\x24\x77\x5B\x61\x24\x63\x5B\x34\x39\x5D\x5D\x28\x61\x24\x63\x5B\x37\x31\x5D\x2C\x43\x28\x71\x29\x7B\x31\x33\x3D\x3D\x71\x5B\x61\x24\x63\x5B\x37\x32\x5D\x5D\x26\x26\x33\x45\x28\x79\x2C\x49\x29\x7D\x29\x7D\x29\x2C\x24\x28\x61\x24\x63\x5B\x36\x64\x5D\x29\x5B\x61\x24\x63\x5B\x35\x31\x5D\x5D\x28\x43\x28\x29\x7B\x4D\x20\x71\x3D\x24\x28\x56\x29\x2C\x79\x3D\x71\x5B\x61\x24\x63\x5B\x31\x31\x5D\x5D\x28\x61\x24\x63\x5B\x32\x44\x5D\x29\x3B\x79\x26\x26\x24\x28\x61\x24\x63\x5B\x36\x6C\x5D\x29\x5B\x61\x24\x63\x5B\x35\x31\x5D\x5D\x28\x43\x28\x29\x7B\x4D\x20\x46\x3D\x24\x28\x56\x29\x2C\x49\x3D\x46\x5B\x61\x24\x63\x5B\x59\x5D\x5D\x28\x61\x24\x63\x5B\x36\x6E\x5D\x29\x2C\x51\x3D\x49\x5B\x61\x24\x63\x5B\x31\x31\x5D\x5D\x28\x61\x24\x63\x5B\x38\x39\x5D\x29\x2C\x58\x3D\x49\x5B\x61\x24\x63\x5B\x31\x31\x5D\x5D\x28\x61\x24\x63\x5B\x32\x66\x5D\x29\x2C\x5A\x3D\x46\x5B\x61\x24\x63\x5B\x59\x5D\x5D\x28\x61\x24\x63\x5B\x36\x6F\x5D\x29\x2C\x55\x3D\x43\x20\x71\x28\x29\x7B\x4D\x20\x46\x3D\x31\x76\x28\x79\x2C\x61\x24\x63\x5B\x36\x70\x5D\x29\x2C\x49\x3D\x46\x3F\x38\x47\x28\x46\x29\x2B\x31\x3A\x34\x2C\x51\x3D\x31\x76\x28\x79\x2C\x61\x24\x63\x5B\x32\x66\x5D\x29\x3B\x31\x64\x5B\x49\x2C\x51\x5D\x7D\x28\x29\x2C\x31\x72\x3D\x55\x5B\x30\x5D\x2C\x31\x68\x3D\x55\x5B\x31\x5D\x2C\x31\x70\x3D\x31\x68\x26\x26\x31\x68\x21\x3D\x58\x26\x26\x61\x24\x63\x5B\x31\x57\x5D\x21\x3D\x31\x68\x3F\x31\x68\x3A\x58\x3B\x31\x68\x26\x26\x31\x68\x21\x3D\x58\x26\x26\x61\x24\x63\x5B\x31\x57\x5D\x21\x3D\x31\x68\x26\x26\x5A\x5B\x61\x24\x63\x5B\x36\x37\x5D\x5D\x28\x29\x5B\x61\x24\x63\x5B\x59\x5D\x5D\x28\x61\x24\x63\x5B\x36\x71\x5D\x29\x5B\x61\x24\x63\x5B\x33\x35\x5D\x5D\x28\x61\x24\x63\x5B\x37\x35\x5D\x2C\x61\x24\x63\x5B\x38\x37\x5D\x2B\x31\x70\x29\x2C\x24\x77\x5B\x61\x24\x63\x5B\x34\x39\x5D\x5D\x28\x61\x24\x63\x5B\x34\x34\x5D\x2C\x43\x20\x79\x28\x29\x7B\x24\x77\x5B\x61\x24\x63\x5B\x34\x35\x5D\x5D\x28\x29\x2B\x24\x77\x5B\x61\x24\x63\x5B\x35\x5D\x5D\x28\x29\x3E\x3D\x5A\x5B\x61\x24\x63\x5B\x34\x37\x5D\x5D\x28\x29\x5B\x61\x24\x63\x5B\x34\x36\x5D\x5D\x26\x26\x28\x24\x77\x5B\x61\x24\x63\x5B\x34\x38\x5D\x5D\x28\x61\x24\x63\x5B\x34\x34\x5D\x2C\x79\x29\x2C\x34\x69\x28\x7B\x74\x3A\x5A\x2C\x32\x72\x3A\x61\x24\x63\x5B\x31\x57\x5D\x2C\x34\x67\x3A\x31\x72\x2C\x36\x72\x3A\x31\x70\x2C\x38\x49\x3A\x51\x7D\x29\x2C\x71\x5B\x61\x24\x63\x5B\x36\x37\x5D\x5D\x28\x29\x5B\x61\x24\x63\x5B\x31\x49\x5D\x5D\x28\x29\x29\x7D\x29\x5B\x61\x24\x63\x5B\x34\x33\x5D\x5D\x28\x61\x24\x63\x5B\x34\x32\x5D\x29\x7D\x29\x7D\x29\x2C\x24\x28\x61\x24\x63\x5B\x36\x73\x5D\x29\x5B\x61\x24\x63\x5B\x35\x31\x5D\x5D\x28\x43\x28\x29\x7B\x4D\x20\x71\x3D\x24\x28\x56\x29\x2C\x79\x3D\x71\x5B\x61\x24\x63\x5B\x31\x31\x5D\x5D\x28\x61\x24\x63\x5B\x32\x44\x5D\x29\x3B\x31\x76\x28\x79\x2C\x61\x24\x63\x5B\x32\x46\x5D\x29\x2C\x71\x5B\x61\x24\x63\x5B\x33\x31\x5D\x5D\x28\x61\x24\x63\x5B\x36\x74\x5D\x29\x2C\x71\x5B\x61\x24\x63\x5B\x59\x5D\x5D\x28\x61\x24\x63\x5B\x36\x6D\x5D\x29\x5B\x61\x24\x63\x5B\x33\x31\x5D\x5D\x28\x61\x24\x63\x5B\x36\x62\x5D\x29\x2C\x35\x53\x28\x61\x24\x63\x5B\x36\x61\x5D\x29\x3B\x4D\x20\x46\x3D\x71\x5B\x61\x24\x63\x5B\x59\x5D\x5D\x28\x61\x24\x63\x5B\x35\x4C\x5D\x29\x2C\x49\x3D\x71\x5B\x61\x24\x63\x5B\x59\x5D\x5D\x28\x61\x24\x63\x5B\x35\x4D\x5D\x29\x2C\x51\x3D\x71\x5B\x61\x24\x63\x5B\x59\x5D\x5D\x28\x61\x24\x63\x5B\x35\x4E\x5D\x29\x3B\x46\x5B\x61\x24\x63\x5B\x34\x39\x5D\x5D\x28\x61\x24\x63\x5B\x36\x39\x5D\x2C\x43\x28\x79\x29\x7B\x79\x5B\x61\x24\x63\x5B\x31\x41\x5D\x5D\x28\x29\x2C\x71\x5B\x61\x24\x63\x5B\x33\x31\x5D\x5D\x28\x61\x24\x63\x5B\x33\x4B\x5D\x29\x2C\x49\x5B\x61\x24\x63\x5B\x31\x53\x5D\x5D\x28\x29\x2C\x51\x5B\x61\x24\x63\x5B\x31\x49\x5D\x5D\x28\x29\x7D\x29\x2C\x49\x5B\x61\x24\x63\x5B\x34\x39\x5D\x5D\x28\x61\x24\x63\x5B\x36\x39\x5D\x2C\x43\x28\x71\x29\x7B\x71\x5B\x61\x24\x63\x5B\x31\x41\x5D\x5D\x28\x29\x2C\x49\x5B\x61\x24\x63\x5B\x35\x4F\x5D\x5D\x28\x29\x7D\x29\x2C\x51\x5B\x61\x24\x63\x5B\x34\x39\x5D\x5D\x28\x61\x24\x63\x5B\x36\x39\x5D\x2C\x43\x28\x29\x7B\x71\x5B\x61\x24\x63\x5B\x33\x31\x5D\x5D\x28\x61\x24\x63\x5B\x33\x4B\x5D\x29\x2C\x51\x5B\x61\x24\x63\x5B\x31\x49\x5D\x5D\x28\x29\x2C\x32\x4B\x28\x61\x24\x63\x5B\x32\x4C\x5D\x29\x7D\x29\x7D\x29\x2C\x24\x28\x43\x28\x29\x7B\x24\x28\x61\x24\x63\x5B\x33\x51\x5D\x29\x5B\x61\x24\x63\x5B\x35\x31\x5D\x5D\x28\x43\x28\x29\x7B\x32\x7A\x20\x71\x3D\x24\x28\x56\x29\x2C\x79\x3D\x61\x24\x63\x5B\x35\x50\x5D\x3B\x71\x5B\x61\x24\x63\x5B\x33\x35\x5D\x5D\x28\x61\x24\x63\x5B\x37\x35\x5D\x2C\x61\x24\x63\x5B\x33\x48\x5D\x29\x5B\x61\x24\x63\x5B\x31\x6D\x5D\x5D\x28\x61\x24\x63\x5B\x35\x51\x5D\x29\x5B\x61\x24\x63\x5B\x33\x35\x5D\x5D\x28\x61\x24\x63\x5B\x33\x32\x5D\x2C\x61\x24\x63\x5B\x35\x4B\x5D\x29\x2C\x71\x5B\x61\x24\x63\x5B\x36\x37\x5D\x5D\x28\x29\x5B\x61\x24\x63\x5B\x33\x35\x5D\x5D\x28\x61\x24\x63\x5B\x33\x32\x5D\x2C\x79\x29\x5B\x61\x24\x63\x5B\x36\x37\x5D\x5D\x28\x29\x5B\x61\x24\x63\x5B\x33\x35\x5D\x5D\x28\x61\x24\x63\x5B\x33\x32\x5D\x2C\x79\x29\x7D\x29\x2C\x38\x6D\x28\x43\x28\x29\x7B\x24\x28\x61\x24\x63\x5B\x33\x51\x5D\x29\x5B\x61\x24\x63\x5B\x35\x35\x5D\x5D\x26\x26\x24\x28\x61\x24\x63\x5B\x35\x54\x5D\x29\x5B\x61\x24\x63\x5B\x35\x35\x5D\x5D\x7C\x7C\x28\x32\x6A\x5B\x61\x24\x63\x5B\x35\x55\x5D\x5D\x5B\x61\x24\x63\x5B\x37\x35\x5D\x5D\x3D\x61\x24\x63\x5B\x33\x48\x5D\x29\x7D\x2C\x38\x75\x29\x2C\x24\x28\x61\x24\x63\x5B\x35\x56\x5D\x29\x5B\x61\x24\x63\x5B\x33\x50\x5D\x5D\x28\x61\x24\x63\x5B\x33\x4C\x5D\x29\x5B\x61\x24\x63\x5B\x31\x5D\x5D\x28\x29\x2C\x24\x28\x61\x24\x63\x5B\x33\x53\x5D\x29\x5B\x61\x24\x63\x5B\x35\x31\x5D\x5D\x28\x43\x28\x29\x7B\x4D\x20\x71\x3D\x24\x28\x56\x29\x3B\x31\x7A\x28\x21\x30\x3D\x3D\x31\x63\x5B\x61\x24\x63\x5B\x33\x56\x5D\x5D\x26\x26\x71\x5B\x61\x24\x63\x5B\x35\x35\x5D\x5D\x3E\x30\x29\x7B\x4D\x20\x79\x3D\x24\x28\x33\x57\x29\x5B\x61\x24\x63\x5B\x34\x35\x5D\x5D\x28\x29\x2C\x46\x3D\x71\x5B\x61\x24\x63\x5B\x34\x37\x5D\x5D\x28\x29\x5B\x61\x24\x63\x5B\x34\x36\x5D\x5D\x2C\x49\x3D\x71\x5B\x61\x24\x63\x5B\x35\x5D\x5D\x28\x29\x2C\x51\x3D\x46\x2B\x32\x2A\x49\x3B\x24\x77\x5B\x61\x24\x63\x5B\x34\x32\x5D\x5D\x28\x43\x28\x29\x7B\x4D\x20\x46\x3D\x24\x28\x33\x57\x29\x5B\x61\x24\x63\x5B\x34\x35\x5D\x5D\x28\x29\x2C\x49\x3D\x71\x5B\x61\x24\x63\x5B\x34\x37\x5D\x5D\x28\x29\x5B\x61\x24\x63\x5B\x34\x36\x5D\x5D\x2C\x58\x3D\x24\x28\x61\x24\x63\x5B\x35\x57\x5D\x29\x5B\x61\x24\x63\x5B\x34\x37\x5D\x5D\x28\x29\x5B\x61\x24\x63\x5B\x34\x36\x5D\x5D\x2B\x31\x3B\x46\x3E\x51\x3F\x71\x5B\x61\x24\x63\x5B\x33\x31\x5D\x5D\x28\x61\x24\x63\x5B\x33\x58\x5D\x29\x3A\x49\x3C\x3D\x58\x26\x26\x71\x5B\x61\x24\x63\x5B\x36\x36\x5D\x5D\x28\x61\x24\x63\x5B\x33\x58\x5D\x29\x5B\x61\x24\x63\x5B\x36\x36\x5D\x5D\x28\x61\x24\x63\x5B\x31\x53\x5D\x29\x2C\x46\x3C\x79\x3F\x31\x54\x28\x43\x28\x29\x7B\x49\x3E\x3D\x58\x26\x26\x71\x5B\x61\x24\x63\x5B\x33\x31\x5D\x5D\x28\x61\x24\x63\x5B\x31\x53\x5D\x29\x7D\x2C\x31\x46\x29\x3A\x31\x54\x28\x43\x28\x29\x7B\x71\x5B\x61\x24\x63\x5B\x36\x36\x5D\x5D\x28\x61\x24\x63\x5B\x31\x53\x5D\x29\x7D\x2C\x31\x46\x29\x2C\x79\x3D\x46\x7D\x29\x7D\x7D\x29\x2C\x24\x28\x61\x24\x63\x5B\x35\x58\x5D\x29\x5B\x61\x24\x63\x5B\x35\x31\x5D\x5D\x28\x43\x28\x29\x7B\x4D\x20\x71\x3D\x24\x28\x56\x29\x2C\x79\x3D\x24\x28\x61\x24\x63\x5B\x35\x59\x5D\x29\x5B\x61\x24\x63\x5B\x32\x73\x5D\x5D\x28\x29\x3B\x79\x5B\x61\x24\x63\x5B\x59\x5D\x5D\x28\x61\x24\x63\x5B\x35\x5A\x5D\x29\x5B\x61\x24\x63\x5B\x31\x49\x5D\x5D\x28\x29\x2C\x79\x5B\x61\x24\x63\x5B\x32\x49\x5D\x5D\x28\x71\x29\x7D\x29\x2C\x24\x28\x61\x24\x63\x5B\x36\x75\x5D\x29\x5B\x61\x24\x63\x5B\x35\x31\x5D\x5D\x28\x43\x28\x29\x7B\x4D\x20\x71\x3D\x24\x28\x56\x29\x2C\x79\x3D\x24\x28\x61\x24\x63\x5B\x36\x63\x5D\x29\x5B\x61\x24\x63\x5B\x32\x73\x5D\x5D\x28\x29\x3B\x79\x5B\x61\x24\x63\x5B\x33\x35\x5D\x5D\x28\x61\x24\x63\x5B\x34\x64\x5D\x2C\x61\x24\x63\x5B\x33\x59\x5D\x29\x5B\x61\x24\x63\x5B\x33\x35\x5D\x5D\x28\x61\x24\x63\x5B\x38\x39\x5D\x2C\x61\x24\x63\x5B\x33\x59\x5D\x29\x2C\x79\x5B\x61\x24\x63\x5B\x32\x49\x5D\x5D\x28\x71\x29\x2C\x24\x28\x61\x24\x63\x5B\x36\x76\x5D\x29\x5B\x61\x24\x63\x5B\x34\x39\x5D\x5D\x28\x61\x24\x63\x5B\x36\x39\x5D\x2C\x43\x28\x29\x7B\x24\x62\x5B\x61\x24\x63\x5B\x36\x51\x5D\x5D\x28\x61\x24\x63\x5B\x33\x5A\x5D\x29\x2C\x24\x28\x61\x24\x63\x5B\x36\x53\x5D\x29\x5B\x61\x24\x63\x5B\x34\x39\x5D\x5D\x28\x61\x24\x63\x5B\x36\x39\x5D\x2C\x43\x28\x29\x7B\x24\x62\x5B\x61\x24\x63\x5B\x36\x36\x5D\x5D\x28\x61\x24\x63\x5B\x33\x5A\x5D\x29\x7D\x29\x7D\x29\x2C\x24\x28\x61\x24\x63\x5B\x36\x54\x5D\x29\x5B\x61\x24\x63\x5B\x34\x39\x5D\x5D\x28\x61\x24\x63\x5B\x36\x39\x5D\x2C\x43\x28\x71\x29\x7B\x71\x5B\x61\x24\x63\x5B\x31\x41\x5D\x5D\x28\x29\x3B\x4D\x20\x79\x3D\x24\x28\x56\x29\x3B\x79\x5B\x61\x24\x63\x5B\x36\x37\x5D\x5D\x28\x29\x5B\x61\x24\x63\x5B\x36\x55\x5D\x5D\x28\x61\x24\x63\x5B\x32\x45\x5D\x29\x3F\x79\x5B\x61\x24\x63\x5B\x36\x37\x5D\x5D\x28\x29\x5B\x61\x24\x63\x5B\x36\x36\x5D\x5D\x28\x61\x24\x63\x5B\x32\x45\x5D\x29\x5B\x61\x24\x63\x5B\x32\x76\x5D\x5D\x28\x61\x24\x63\x5B\x34\x61\x5D\x29\x5B\x61\x24\x63\x5B\x34\x62\x5D\x5D\x28\x31\x46\x29\x3A\x79\x5B\x61\x24\x63\x5B\x36\x37\x5D\x5D\x28\x29\x5B\x61\x24\x63\x5B\x33\x31\x5D\x5D\x28\x61\x24\x63\x5B\x32\x45\x5D\x29\x5B\x61\x24\x63\x5B\x32\x76\x5D\x5D\x28\x61\x24\x63\x5B\x34\x61\x5D\x29\x5B\x61\x24\x63\x5B\x34\x62\x5D\x5D\x28\x31\x46\x29\x7D\x29\x7D\x29\x2C\x24\x28\x61\x24\x63\x5B\x36\x56\x5D\x29\x5B\x61\x24\x63\x5B\x35\x31\x5D\x5D\x28\x43\x28\x29\x7B\x4D\x20\x71\x3D\x24\x28\x56\x29\x2C\x79\x3D\x24\x28\x61\x24\x63\x5B\x36\x57\x5D\x29\x2C\x46\x3D\x24\x28\x61\x24\x63\x5B\x36\x58\x5D\x29\x2C\x49\x3D\x21\x21\x79\x5B\x61\x24\x63\x5B\x35\x35\x5D\x5D\x26\x26\x79\x5B\x61\x24\x63\x5B\x32\x73\x5D\x5D\x28\x29\x3B\x21\x31\x21\x3D\x49\x26\x26\x28\x49\x5B\x61\x24\x63\x5B\x33\x35\x5D\x5D\x28\x61\x24\x63\x5B\x34\x64\x5D\x2C\x61\x24\x63\x5B\x36\x59\x5D\x29\x5B\x61\x24\x63\x5B\x59\x5D\x5D\x28\x61\x24\x63\x5B\x36\x52\x5D\x29\x5B\x61\x24\x63\x5B\x31\x49\x5D\x5D\x28\x29\x2C\x71\x5B\x61\x24\x63\x5B\x31\x44\x5D\x5D\x28\x49\x29\x29\x3B\x4D\x20\x51\x3D\x21\x21\x46\x5B\x61\x24\x63\x5B\x35\x35\x5D\x5D\x26\x26\x46\x5B\x61\x24\x63\x5B\x32\x73\x5D\x5D\x28\x29\x3B\x21\x31\x21\x3D\x51\x26\x26\x71\x5B\x61\x24\x63\x5B\x31\x44\x5D\x5D\x28\x51\x29\x7D\x29\x2C\x24\x28\x61\x24\x63\x5B\x33\x55\x5D\x29\x5B\x61\x24\x63\x5B\x35\x31\x5D\x5D\x28\x43\x28\x29\x7B\x4D\x20\x71\x3D\x24\x28\x56\x29\x2C\x79\x3D\x24\x28\x61\x24\x63\x5B\x36\x5A\x5D\x29\x2C\x46\x3D\x61\x24\x63\x5B\x36\x35\x5D\x2C\x49\x3D\x71\x5B\x61\x24\x63\x5B\x31\x31\x5D\x5D\x28\x61\x24\x63\x5B\x33\x52\x5D\x29\x3B\x71\x5B\x61\x24\x63\x5B\x34\x39\x5D\x5D\x28\x61\x24\x63\x5B\x36\x39\x5D\x2C\x43\x28\x51\x29\x7B\x51\x5B\x61\x24\x63\x5B\x31\x41\x5D\x5D\x28\x29\x2C\x71\x5B\x61\x24\x63\x5B\x36\x36\x5D\x5D\x28\x46\x29\x2C\x24\x5B\x61\x24\x63\x5B\x32\x48\x5D\x5D\x28\x7B\x33\x47\x3A\x49\x2C\x37\x62\x3A\x43\x28\x29\x7B\x79\x5B\x61\x24\x63\x5B\x33\x31\x5D\x5D\x28\x46\x29\x7D\x2C\x33\x54\x3A\x43\x28\x79\x29\x7B\x4D\x20\x51\x3D\x24\x28\x79\x29\x5B\x61\x24\x63\x5B\x59\x5D\x5D\x28\x61\x24\x63\x5B\x34\x63\x5D\x29\x3B\x51\x5B\x61\x24\x63\x5B\x59\x5D\x5D\x28\x61\x24\x63\x5B\x37\x63\x5D\x29\x5B\x61\x24\x63\x5B\x33\x31\x5D\x5D\x28\x61\x24\x63\x5B\x37\x64\x5D\x29\x2C\x24\x28\x61\x24\x63\x5B\x34\x63\x5D\x29\x5B\x61\x24\x63\x5B\x31\x44\x5D\x5D\x28\x51\x5B\x61\x24\x63\x5B\x35\x32\x5D\x5D\x28\x29\x29\x2C\x28\x49\x3D\x24\x28\x79\x29\x5B\x61\x24\x63\x5B\x59\x5D\x5D\x28\x61\x24\x63\x5B\x33\x55\x5D\x29\x5B\x61\x24\x63\x5B\x31\x31\x5D\x5D\x28\x61\x24\x63\x5B\x33\x52\x5D\x29\x29\x3F\x71\x5B\x61\x24\x63\x5B\x33\x31\x5D\x5D\x28\x46\x29\x3A\x28\x71\x5B\x61\x24\x63\x5B\x36\x36\x5D\x5D\x28\x46\x29\x2C\x24\x28\x61\x24\x63\x5B\x37\x65\x5D\x29\x5B\x61\x24\x63\x5B\x33\x31\x5D\x5D\x28\x46\x29\x29\x7D\x2C\x38\x6B\x3A\x43\x28\x29\x7B\x79\x5B\x61\x24\x63\x5B\x36\x36\x5D\x5D\x28\x46\x29\x2C\x32\x4B\x28\x61\x24\x63\x5B\x32\x4C\x5D\x29\x2C\x24\x28\x61\x24\x63\x5B\x37\x66\x5D\x29\x5B\x61\x24\x63\x5B\x33\x50\x5D\x5D\x28\x61\x24\x63\x5B\x33\x4C\x5D\x29\x5B\x61\x24\x63\x5B\x31\x5D\x5D\x28\x29\x7D\x7D\x29\x7D\x29\x7D\x29\x2C\x24\x28\x61\x24\x63\x5B\x37\x67\x5D\x29\x5B\x61\x24\x63\x5B\x35\x31\x5D\x5D\x28\x43\x28\x29\x7B\x4D\x20\x71\x3D\x24\x28\x56\x29\x3B\x24\x77\x5B\x61\x24\x63\x5B\x34\x39\x5D\x5D\x28\x61\x24\x63\x5B\x34\x34\x5D\x2C\x43\x20\x79\x28\x29\x7B\x24\x77\x5B\x61\x24\x63\x5B\x34\x35\x5D\x5D\x28\x29\x2B\x24\x77\x5B\x61\x24\x63\x5B\x35\x5D\x5D\x28\x29\x3E\x3D\x71\x5B\x61\x24\x63\x5B\x34\x37\x5D\x5D\x28\x29\x5B\x61\x24\x63\x5B\x34\x36\x5D\x5D\x26\x26\x28\x24\x77\x5B\x61\x24\x63\x5B\x34\x38\x5D\x5D\x28\x61\x24\x63\x5B\x34\x34\x5D\x2C\x79\x29\x2C\x71\x5B\x61\x24\x63\x5B\x32\x74\x5D\x5D\x28\x2F\x5C\x7B\x37\x68\x5C\x7D\x28\x5B\x5E\x5C\x7D\x5D\x2A\x29\x5C\x7B\x5C\x2F\x37\x68\x5C\x7D\x2F\x67\x2C\x61\x24\x63\x5B\x37\x61\x5D\x29\x2C\x71\x5B\x61\x24\x63\x5B\x32\x74\x5D\x5D\x28\x2F\x5C\x7B\x36\x50\x5C\x7D\x28\x5B\x5E\x5C\x7D\x5D\x2A\x29\x5C\x7B\x5C\x2F\x36\x50\x5C\x7D\x2F\x67\x2C\x61\x24\x63\x5B\x36\x47\x5D\x29\x2C\x71\x5B\x61\x24\x63\x5B\x59\x5D\x5D\x28\x61\x24\x63\x5B\x36\x4F\x5D\x29\x5B\x61\x24\x63\x5B\x35\x31\x5D\x5D\x28\x43\x28\x29\x7B\x32\x7A\x20\x71\x3B\x4D\x20\x79\x3D\x24\x28\x56\x29\x2C\x46\x3D\x79\x5B\x61\x24\x63\x5B\x31\x6D\x5D\x5D\x28\x29\x2C\x49\x2C\x51\x2C\x58\x2C\x5A\x3B\x79\x5B\x61\x24\x63\x5B\x31\x59\x5D\x5D\x28\x28\x71\x3D\x46\x2C\x49\x3D\x33\x49\x20\x38\x71\x28\x71\x29\x2C\x51\x3D\x33\x49\x20\x38\x73\x28\x49\x5B\x61\x24\x63\x5B\x37\x39\x5D\x5D\x29\x2C\x28\x5A\x3D\x28\x58\x3D\x21\x21\x71\x5B\x61\x24\x63\x5B\x31\x33\x5D\x5D\x28\x61\x24\x63\x5B\x36\x79\x5D\x29\x26\x26\x51\x5B\x61\x24\x63\x5B\x36\x7A\x5D\x5D\x28\x61\x24\x63\x5B\x36\x41\x5D\x29\x29\x7C\x7C\x21\x21\x71\x5B\x61\x24\x63\x5B\x31\x33\x5D\x5D\x28\x61\x24\x63\x5B\x36\x42\x5D\x29\x26\x26\x49\x5B\x61\x24\x63\x5B\x36\x43\x5D\x5D\x5B\x61\x24\x63\x5B\x32\x38\x5D\x5D\x28\x61\x24\x63\x5B\x33\x37\x5D\x2C\x61\x24\x63\x5B\x31\x35\x5D\x29\x29\x3F\x60\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x61\x24\x63\x5B\x36\x44\x5D\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x5A\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x61\x24\x63\x5B\x36\x45\x5D\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x5A\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x61\x24\x63\x5B\x36\x78\x5D\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x60\x3A\x61\x24\x63\x5B\x36\x46\x5D\x2B\x31\x63\x5B\x61\x24\x63\x5B\x38\x31\x5D\x5D\x29\x29\x7D\x29\x2C\x71\x5B\x61\x24\x63\x5B\x59\x5D\x5D\x28\x61\x24\x63\x5B\x36\x48\x5D\x29\x5B\x61\x24\x63\x5B\x35\x31\x5D\x5D\x28\x43\x28\x29\x7B\x4D\x20\x71\x3D\x24\x28\x56\x29\x2C\x79\x3D\x71\x5B\x61\x24\x63\x5B\x31\x31\x5D\x5D\x28\x61\x24\x63\x5B\x38\x39\x5D\x29\x3B\x71\x5B\x61\x24\x63\x5B\x34\x39\x5D\x5D\x28\x61\x24\x63\x5B\x36\x39\x5D\x2C\x43\x28\x29\x7B\x71\x5B\x61\x24\x63\x5B\x31\x59\x5D\x5D\x28\x60\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x61\x24\x63\x5B\x36\x49\x5D\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x79\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x24\x7B\x61\x24\x63\x5B\x36\x4A\x5D\x7D\x24\x7B\x61\x24\x65\x5B\x31\x35\x5D\x7D\x60\x29\x7D\x29\x7D\x29\x29\x7D\x29\x5B\x61\x24\x63\x5B\x34\x33\x5D\x5D\x28\x61\x24\x63\x5B\x34\x32\x5D\x29\x7D\x29\x2C\x32\x4B\x28\x61\x24\x63\x5B\x32\x4C\x5D\x29\x2C\x24\x28\x61\x24\x63\x5B\x36\x4B\x5D\x29\x5B\x61\x24\x63\x5B\x35\x31\x5D\x5D\x28\x43\x28\x29\x7B\x4D\x20\x71\x3D\x24\x28\x56\x29\x3B\x24\x77\x5B\x61\x24\x63\x5B\x34\x39\x5D\x5D\x28\x61\x24\x63\x5B\x34\x32\x5D\x2C\x43\x28\x29\x7B\x24\x28\x56\x29\x5B\x61\x24\x63\x5B\x34\x35\x5D\x5D\x28\x29\x3E\x3D\x32\x4D\x3F\x71\x5B\x61\x24\x63\x5B\x33\x31\x5D\x5D\x28\x61\x24\x63\x5B\x31\x53\x5D\x29\x3A\x71\x5B\x61\x24\x63\x5B\x36\x36\x5D\x5D\x28\x61\x24\x63\x5B\x31\x53\x5D\x29\x2C\x71\x5B\x61\x24\x63\x5B\x34\x37\x5D\x5D\x28\x29\x5B\x61\x24\x63\x5B\x34\x36\x5D\x5D\x3E\x3D\x24\x28\x61\x24\x63\x5B\x36\x4C\x5D\x29\x5B\x61\x24\x63\x5B\x34\x37\x5D\x5D\x28\x29\x5B\x61\x24\x63\x5B\x34\x36\x5D\x5D\x2D\x33\x36\x3F\x71\x5B\x61\x24\x63\x5B\x33\x31\x5D\x5D\x28\x61\x24\x63\x5B\x34\x6C\x5D\x29\x3A\x71\x5B\x61\x24\x63\x5B\x36\x36\x5D\x5D\x28\x61\x24\x63\x5B\x34\x6C\x5D\x29\x7D\x29\x2C\x71\x5B\x61\x24\x63\x5B\x34\x39\x5D\x5D\x28\x61\x24\x63\x5B\x36\x39\x5D\x2C\x43\x28\x29\x7B\x24\x28\x61\x24\x63\x5B\x36\x4D\x5D\x29\x5B\x61\x24\x63\x5B\x36\x4E\x5D\x5D\x28\x7B\x38\x48\x3A\x30\x7D\x2C\x35\x48\x29\x7D\x29\x7D\x29\x7D\x29","\x7C","\x73\x70\x6C\x69\x74","\x7C\x7C\x7C\x7C\x7C\x7C\x7C\x7C\x7C\x7C\x5F\x7C\x7C\x5F\x30\x78\x33\x35\x32\x35\x7C\x7C\x5F\x30\x78\x35\x34\x62\x34\x7C\x78\x36\x35\x7C\x7C\x7C\x78\x37\x34\x7C\x78\x36\x31\x7C\x78\x36\x46\x7C\x78\x37\x33\x7C\x78\x37\x32\x7C\x78\x36\x39\x7C\x78\x36\x43\x7C\x78\x36\x45\x7C\x5F\x30\x78\x34\x32\x31\x39\x78\x32\x7C\x78\x32\x44\x7C\x78\x36\x33\x7C\x7C\x78\x36\x44\x7C\x78\x37\x30\x7C\x7C\x78\x32\x30\x7C\x5F\x30\x78\x34\x32\x31\x39\x78\x33\x7C\x78\x36\x32\x7C\x78\x36\x34\x7C\x78\x32\x32\x7C\x66\x75\x6E\x63\x74\x69\x6F\x6E\x7C\x78\x37\x35\x7C\x78\x32\x45\x7C\x5F\x30\x78\x34\x32\x31\x39\x78\x34\x7C\x78\x36\x38\x7C\x78\x36\x37\x7C\x5F\x30\x78\x34\x32\x31\x39\x78\x35\x7C\x78\x33\x44\x7C\x78\x32\x46\x7C\x78\x37\x39\x7C\x6C\x65\x74\x7C\x78\x33\x43\x7C\x78\x33\x45\x7C\x78\x37\x36\x7C\x5F\x30\x78\x34\x32\x31\x39\x78\x36\x7C\x78\x37\x37\x7C\x78\x36\x36\x7C\x78\x37\x38\x7C\x5F\x30\x78\x34\x32\x31\x39\x78\x39\x7C\x74\x68\x69\x73\x7C\x78\x36\x42\x7C\x5F\x30\x78\x34\x32\x31\x39\x78\x37\x7C\x31\x34\x34\x7C\x5F\x30\x78\x34\x32\x31\x39\x78\x38\x7C\x7C\x7C\x7C\x7C\x7C\x7C\x7C\x7C\x7C\x7C\x78\x33\x32\x7C\x78\x33\x41\x7C\x70\x62\x74\x7C\x72\x65\x74\x75\x72\x6E\x7C\x78\x33\x42\x7C\x78\x33\x30\x7C\x78\x33\x35\x7C\x5F\x30\x78\x34\x32\x31\x39\x78\x62\x7C\x78\x33\x31\x7C\x78\x32\x31\x7C\x78\x37\x41\x7C\x78\x33\x33\x7C\x31\x34\x32\x7C\x78\x34\x33\x7C\x78\x35\x34\x7C\x5F\x30\x78\x34\x32\x31\x39\x78\x63\x7C\x78\x33\x37\x7C\x5F\x30\x78\x34\x32\x31\x39\x78\x61\x7C\x5F\x30\x78\x34\x32\x31\x39\x78\x32\x37\x7C\x78\x32\x33\x7C\x78\x35\x33\x7C\x67\x65\x74\x41\x74\x74\x72\x7C\x78\x32\x43\x7C\x78\x37\x31\x7C\x78\x34\x43\x7C\x69\x66\x7C\x31\x37\x38\x7C\x78\x34\x35\x7C\x78\x37\x42\x7C\x31\x35\x38\x7C\x78\x37\x44\x7C\x31\x37\x30\x7C\x73\x68\x63\x7C\x78\x36\x41\x7C\x31\x34\x39\x7C\x78\x35\x36\x7C\x78\x35\x35\x7C\x78\x33\x38\x7C\x78\x32\x36\x7C\x78\x35\x46\x7C\x78\x33\x36\x7C\x78\x34\x32\x7C\x63\x6C\x73\x7C\x78\x34\x34\x7C\x32\x37\x35\x7C\x73\x65\x74\x54\x69\x6D\x65\x6F\x75\x74\x7C\x78\x33\x34\x7C\x78\x34\x36\x7C\x31\x33\x38\x7C\x78\x34\x31\x7C\x31\x39\x30\x7C\x5F\x30\x78\x34\x32\x31\x39\x78\x32\x36\x7C\x7C\x7C\x7C\x7C\x7C\x7C\x7C\x7C\x7C\x7C\x78\x35\x30\x7C\x78\x34\x42\x7C\x31\x30\x35\x7C\x78\x35\x39\x7C\x78\x34\x44\x7C\x31\x34\x38\x7C\x78\x33\x39\x7C\x31\x30\x39\x7C\x66\x6F\x72\x7C\x77\x69\x6E\x64\x6F\x77\x7C\x31\x30\x32\x7C\x78\x34\x41\x7C\x78\x34\x37\x7C\x78\x35\x37\x7C\x78\x34\x39\x7C\x78\x34\x38\x7C\x5F\x30\x78\x34\x32\x31\x39\x78\x32\x65\x7C\x74\x79\x70\x65\x7C\x32\x39\x31\x7C\x32\x30\x32\x7C\x31\x37\x37\x7C\x32\x33\x38\x7C\x78\x35\x32\x7C\x5F\x30\x78\x34\x32\x31\x39\x78\x32\x62\x7C\x78\x33\x46\x7C\x76\x61\x72\x7C\x39\x33\x7C\x31\x33\x33\x7C\x78\x32\x34\x7C\x31\x38\x32\x7C\x33\x30\x32\x7C\x31\x32\x34\x7C\x31\x33\x32\x7C\x31\x34\x31\x7C\x32\x35\x34\x7C\x78\x35\x41\x7C\x67\x65\x74\x53\x74\x69\x63\x6B\x79\x53\x69\x64\x65\x62\x61\x72\x7C\x32\x37\x37\x7C\x31\x30\x30\x7C\x32\x30\x33\x7C\x31\x33\x30\x7C\x32\x34\x33\x7C\x31\x33\x31\x7C\x31\x31\x39\x7C\x32\x34\x34\x7C\x32\x33\x37\x7C\x32\x35\x39\x7C\x32\x35\x38\x7C\x32\x35\x37\x7C\x6E\x61\x76\x53\x68\x6F\x72\x74\x63\x75\x74\x73\x7C\x32\x33\x35\x7C\x32\x34\x32\x7C\x7C\x7C\x7C\x7C\x7C\x7C\x7C\x7C\x7C\x7C\x63\x6C\x6F\x73\x65\x53\x65\x61\x72\x63\x68\x7C\x31\x33\x34\x7C\x32\x30\x38\x7C\x39\x31\x7C\x31\x38\x37\x7C\x6C\x6F\x63\x61\x6C\x53\x74\x6F\x72\x61\x67\x65\x7C\x31\x38\x36\x7C\x6D\x73\x67\x45\x72\x72\x6F\x72\x7C\x31\x35\x39\x7C\x5F\x30\x78\x34\x32\x31\x39\x78\x32\x64\x7C\x32\x30\x36\x7C\x62\x72\x65\x61\x6B\x7C\x31\x34\x36\x7C\x31\x31\x36\x7C\x31\x34\x35\x7C\x31\x34\x33\x7C\x31\x33\x35\x7C\x62\x65\x66\x6F\x72\x65\x4C\x6F\x61\x64\x65\x72\x7C\x32\x32\x37\x7C\x31\x39\x37\x7C\x31\x39\x38\x7C\x31\x34\x30\x7C\x67\x65\x74\x46\x65\x65\x64\x55\x72\x6C\x7C\x31\x32\x39\x7C\x31\x32\x38\x7C\x39\x30\x7C\x31\x32\x37\x7C\x6F\x70\x65\x6E\x53\x68\x61\x72\x65\x7C\x31\x33\x37\x7C\x31\x33\x36\x7C\x67\x65\x74\x53\x65\x61\x72\x63\x68\x7C\x63\x6C\x6F\x73\x65\x53\x68\x61\x72\x65\x7C\x75\x72\x6C\x7C\x32\x38\x32\x7C\x6E\x65\x77\x7C\x78\x32\x35\x7C\x32\x37\x34\x7C\x32\x38\x36\x7C\x39\x32\x7C\x6F\x70\x65\x6E\x53\x65\x61\x72\x63\x68\x7C\x63\x6C\x65\x61\x6E\x53\x65\x61\x72\x63\x68\x7C\x32\x38\x37\x7C\x32\x38\x33\x7C\x33\x31\x34\x7C\x31\x36\x34\x7C\x73\x75\x63\x63\x65\x73\x73\x7C\x33\x31\x38\x7C\x31\x36\x33\x7C\x64\x6F\x63\x75\x6D\x65\x6E\x74\x7C\x32\x39\x30\x7C\x32\x39\x36\x7C\x32\x39\x38\x7C\x7C\x7C\x7C\x7C\x7C\x7C\x7C\x7C\x7C\x7C\x33\x30\x35\x7C\x33\x30\x34\x7C\x33\x31\x35\x7C\x32\x39\x37\x7C\x78\x32\x39\x7C\x39\x38\x7C\x6E\x75\x6D\x7C\x78\x34\x46\x7C\x67\x65\x74\x50\x6F\x73\x74\x73\x7C\x31\x30\x36\x7C\x31\x31\x30\x7C\x33\x33\x38\x7C\x31\x30\x38\x7C\x78\x32\x38\x7C\x67\x65\x74\x52\x65\x63\x65\x6E\x74\x50\x6F\x73\x74\x73\x44\x61\x74\x61\x7C\x5F\x30\x78\x34\x32\x31\x39\x78\x32\x61\x7C\x31\x36\x37\x7C\x31\x36\x39\x7C\x31\x37\x31\x7C\x78\x35\x38\x7C\x31\x37\x35\x7C\x67\x65\x74\x50\x6F\x73\x74\x49\x44\x7C\x31\x37\x32\x7C\x31\x37\x33\x7C\x31\x37\x34\x7C\x5F\x30\x78\x34\x32\x31\x39\x78\x32\x63\x7C\x31\x36\x38\x7C\x6F\x6E\x53\x63\x72\x6F\x6C\x6C\x7C\x31\x35\x33\x7C\x31\x35\x37\x7C\x31\x36\x35\x7C\x31\x36\x36\x7C\x31\x36\x32\x7C\x31\x36\x31\x7C\x31\x36\x30\x7C\x67\x65\x74\x50\x6F\x73\x74\x43\x6F\x6E\x74\x65\x6E\x74\x7C\x78\x34\x45\x7C\x5F\x30\x78\x34\x32\x31\x39\x78\x32\x66\x7C\x78\x35\x31\x7C\x65\x6C\x73\x65\x7C\x31\x35\x34\x7C\x31\x35\x35\x7C\x31\x35\x36\x7C\x31\x31\x38\x7C\x31\x35\x30\x7C\x4A\x53\x4F\x4E\x7C\x31\x32\x35\x7C\x67\x65\x74\x50\x6F\x73\x74\x4C\x69\x6E\x6B\x7C\x67\x65\x74\x50\x6F\x73\x74\x54\x69\x74\x6C\x65\x7C\x67\x65\x74\x50\x6F\x73\x74\x54\x61\x67\x7C\x31\x30\x37\x7C\x67\x65\x74\x50\x6F\x73\x74\x41\x75\x74\x68\x6F\x72\x7C\x7C\x7C\x7C\x7C\x7C\x7C\x7C\x7C\x7C\x7C\x67\x65\x74\x50\x6F\x73\x74\x44\x61\x74\x65\x7C\x31\x32\x36\x7C\x31\x32\x33\x7C\x67\x65\x74\x50\x6F\x73\x74\x49\x6D\x61\x67\x65\x54\x79\x70\x65\x7C\x31\x31\x31\x7C\x31\x31\x32\x7C\x31\x31\x33\x7C\x31\x32\x32\x7C\x31\x31\x34\x7C\x31\x31\x35\x7C\x31\x32\x31\x7C\x31\x32\x30\x7C\x67\x65\x74\x50\x6F\x73\x74\x49\x6D\x61\x67\x65\x7C\x67\x65\x74\x50\x6F\x73\x74\x4D\x65\x74\x61\x7C\x31\x35\x32\x7C\x39\x34\x7C\x31\x35\x31\x7C\x31\x31\x37\x7C\x63\x61\x63\x68\x65\x7C\x64\x61\x74\x61\x54\x79\x70\x65\x7C\x61\x73\x79\x6E\x63\x7C\x4D\x61\x74\x68\x7C\x6E\x6F\x54\x68\x75\x6D\x62\x6E\x61\x69\x6C\x7C\x31\x34\x37\x7C\x63\x61\x73\x65\x7C\x31\x33\x39\x7C\x39\x35\x7C\x39\x36\x7C\x39\x37\x7C\x39\x39\x7C\x31\x30\x31\x7C\x31\x30\x33\x7C\x31\x30\x34\x7C\x35\x30\x30\x7C\x31\x39\x34\x7C\x31\x37\x36\x7C\x32\x38\x30\x7C\x32\x37\x31\x7C\x32\x37\x32\x7C\x32\x37\x33\x7C\x32\x37\x36\x7C\x32\x37\x39\x7C\x32\x38\x31\x7C\x31\x38\x31\x7C\x62\x65\x61\x75\x74\x69\x41\x76\x61\x74\x61\x72\x7C\x32\x38\x34\x7C\x32\x38\x35\x7C\x32\x38\x38\x7C\x32\x38\x39\x7C\x32\x39\x34\x7C\x32\x39\x32\x7C\x32\x39\x33\x7C\x7C\x7C\x7C\x7C\x7C\x7C\x7C\x7C\x7C\x7C\x32\x37\x30\x7C\x32\x36\x38\x7C\x32\x39\x35\x7C\x32\x36\x36\x7C\x32\x34\x39\x7C\x32\x35\x30\x7C\x32\x35\x31\x7C\x32\x35\x32\x7C\x32\x35\x35\x7C\x32\x35\x33\x7C\x32\x36\x30\x7C\x32\x36\x35\x7C\x32\x36\x39\x7C\x32\x36\x31\x7C\x32\x36\x32\x7C\x32\x36\x33\x7C\x32\x36\x34\x7C\x6C\x61\x62\x65\x6C\x7C\x32\x37\x38\x7C\x32\x36\x37\x7C\x33\x30\x37\x7C\x33\x30\x31\x7C\x32\x34\x37\x7C\x33\x33\x30\x7C\x33\x32\x33\x7C\x33\x32\x35\x7C\x33\x32\x34\x7C\x33\x32\x36\x7C\x33\x32\x37\x7C\x33\x32\x38\x7C\x33\x32\x39\x7C\x33\x33\x31\x7C\x33\x32\x32\x7C\x33\x33\x35\x7C\x33\x33\x33\x7C\x33\x33\x34\x7C\x33\x34\x31\x7C\x33\x33\x37\x7C\x33\x34\x30\x7C\x33\x33\x39\x7C\x33\x33\x32\x7C\x76\x69\x64\x65\x6F\x7C\x32\x39\x39\x7C\x33\x31\x30\x7C\x33\x30\x30\x7C\x33\x30\x36\x7C\x33\x30\x33\x7C\x33\x31\x32\x7C\x33\x30\x38\x7C\x33\x30\x39\x7C\x33\x31\x31\x7C\x33\x31\x33\x7C\x7C\x7C\x7C\x7C\x7C\x7C\x7C\x7C\x7C\x7C\x33\x32\x31\x7C\x62\x65\x66\x6F\x72\x65\x53\x65\x6E\x64\x7C\x33\x31\x37\x7C\x33\x31\x36\x7C\x33\x31\x39\x7C\x33\x32\x30\x7C\x33\x33\x36\x7C\x69\x6D\x61\x67\x65\x7C\x32\x34\x38\x7C\x78\x32\x37\x7C\x32\x30\x39\x7C\x31\x39\x36\x7C\x32\x33\x30\x7C\x32\x32\x39\x7C\x31\x38\x39\x7C\x32\x32\x36\x7C\x32\x32\x35\x7C\x32\x32\x34\x7C\x32\x32\x33\x7C\x32\x32\x32\x7C\x32\x33\x31\x7C\x32\x31\x38\x7C\x31\x38\x35\x7C\x32\x32\x31\x7C\x32\x33\x34\x7C\x32\x34\x36\x7C\x31\x38\x33\x7C\x31\x38\x34\x7C\x32\x32\x30\x7C\x32\x31\x39\x7C\x31\x39\x39\x7C\x31\x39\x35\x7C\x32\x30\x37\x7C\x31\x39\x33\x7C\x31\x39\x31\x7C\x31\x39\x32\x7C\x69\x6E\x7C\x32\x32\x38\x7C\x31\x38\x30\x7C\x32\x33\x39\x7C\x32\x30\x35\x7C\x32\x35\x36\x7C\x32\x31\x30\x7C\x32\x34\x30\x7C\x32\x34\x31\x7C\x31\x37\x39\x7C\x32\x33\x32\x7C\x32\x30\x34\x7C\x32\x31\x32\x7C\x32\x31\x31\x7C\x32\x34\x35\x7C\x32\x31\x35\x7C\x7C\x7C\x7C\x7C\x7C\x7C\x7C\x7C\x7C\x7C\x32\x30\x30\x7C\x32\x33\x33\x7C\x32\x31\x37\x7C\x32\x31\x36\x7C\x32\x30\x31\x7C\x32\x31\x34\x7C\x32\x31\x33\x7C\x32\x33\x36\x7C\x31\x38\x38\x7C\x70\x6F\x73\x74\x7C\x63\x6F\x6D\x70\x6C\x65\x74\x65\x7C\x74\x79\x70\x65\x6F\x66\x7C\x73\x65\x74\x49\x6E\x74\x65\x72\x76\x61\x6C\x7C\x65\x72\x72\x6F\x72\x7C\x68\x65\x61\x64\x6C\x69\x6E\x65\x7C\x69\x6E\x64\x65\x78\x7C\x55\x52\x4C\x7C\x49\x6D\x61\x67\x65\x7C\x55\x52\x4C\x53\x65\x61\x72\x63\x68\x50\x61\x72\x61\x6D\x73\x7C\x74\x61\x72\x67\x65\x74\x7C\x31\x65\x33\x7C\x6C\x69\x6E\x6B\x7C\x6E\x75\x6C\x6C\x7C\x53\x74\x72\x69\x6E\x67\x7C\x67\x65\x74\x50\x6F\x73\x74\x53\x75\x6D\x6D\x61\x72\x79\x7C\x6A\x51\x75\x65\x72\x79\x7C\x63\x6F\x6E\x73\x74\x7C\x73\x77\x69\x74\x63\x68\x7C\x75\x32\x30\x32\x36\x7C\x33\x65\x33\x7C\x61\x64\x64\x69\x74\x69\x6F\x6E\x61\x6C\x4D\x61\x72\x67\x69\x6E\x54\x6F\x70\x7C\x61\x64\x64\x69\x74\x69\x6F\x6E\x61\x6C\x4D\x61\x72\x67\x69\x6E\x42\x6F\x74\x74\x6F\x6D\x7C\x4E\x75\x6D\x62\x65\x72\x7C\x73\x63\x72\x6F\x6C\x6C\x54\x6F\x70\x7C\x69\x64\x7C\x63\x6F\x6E\x74\x61\x69\x6E\x65\x72\x53\x65\x6C\x65\x63\x74\x6F\x72\x7C\x6E\x61\x76\x69\x67\x61\x74\x6F\x72","","\x66\x72\x6F\x6D\x43\x68\x61\x72\x43\x6F\x64\x65","\x72\x65\x70\x6C\x61\x63\x65","\x5C\x77\x2B","\x5C\x62","\x67"];eval(function(_0xbe0ex1,_0xbe0ex2,_0xbe0ex3,_0xbe0ex4,_0xbe0ex5,_0xbe0ex6){_0xbe0ex5= function(_0xbe0ex3){return (_0xbe0ex3< _0xbe0ex2?_$_pbtJS[4]:_0xbe0ex5(parseInt(_0xbe0ex3/ _0xbe0ex2)))+ ((_0xbe0ex3= _0xbe0ex3% _0xbe0ex2)> 35?String[_$_pbtJS[5]](_0xbe0ex3+ 29):_0xbe0ex3.toString(36))};if(!_$_pbtJS[4][_$_pbtJS[6]](/^/,String)){while(_0xbe0ex3--){_0xbe0ex6[_0xbe0ex5(_0xbe0ex3)]= _0xbe0ex4[_0xbe0ex3]|| _0xbe0ex5(_0xbe0ex3)};_0xbe0ex4= [function(_0xbe0ex5){return _0xbe0ex6[_0xbe0ex5]}];_0xbe0ex5= function(){return _$_pbtJS[7]};_0xbe0ex3= 1};while(_0xbe0ex3--){if(_0xbe0ex4[_0xbe0ex3]){_0xbe0ex1= _0xbe0ex1[_$_pbtJS[6]]( new RegExp(_$_pbtJS[8]+ _0xbe0ex5(_0xbe0ex3)+ _$_pbtJS[8],_$_pbtJS[9]),_0xbe0ex4[_0xbe0ex3])}};return _0xbe0ex1}(_$_pbtJS[0],62,543,_$_pbtJS[3][_$_pbtJS[2]](_$_pbtJS[1]),0,{}));
//]]>
</b:tag>
</b:if>
<!-- Blogger Scripts -->
<b:if cond='data:isFeed'>
  <b:eval cond='data:isFeed' expr='&quot;&lt;!--&quot;'/>
</b:if>
</body>
</b:with>
</html>
