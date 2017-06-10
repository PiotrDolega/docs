# Webpack

System is equipped with predefined asset bundles, created with the webpack module bundler.

At this point, bundles contain JS files of application dependencies, such as external plugins, core js files and other external assets (such as css files and images).

All Bundles are developed to serve one given application view.

Bundles are named in a straightforward way - the name of the bundle suggests the application view that developer should use it on.
One exception from this rule is cache bundle (webpack.app_cache.js) that should be used in all application views, prior to given view bundle. Cache Bundle serves the puprose of speeding up the application - it contains all frequently used plugins across all views.  

Location of bundles in the system:
```bash
public/webpack/
```

---
 
List of existing Bundles: (CV stands for Complete View)

#### webpack.app_cache.js ( cache bundle)
+ jQuery
+ jQuery-UI 
+ pace.js
+ globalize
+ enquire.js
+ moment.js
+ noty
+ qTip2
+ swal 
+ match-height
+ hammer.js 
  - jquery adapter plugin
+ underscore.js
+ perfect-scrollbar
  - jquery adapter plugin
+ modernizr

#### webpack.CV_all.js ( Bundle that consists of all other CV Bundles - serves a testing purpose only) 
#### webpack.CV_brand_settings.js ( Brand Settings View, including Email Templates )
#### webpack.CV_comments.js ( Demo of Vue Comments Component )
#### webpack.CV_dashboard.js (Dashboard View, including gridstack and D3 library)
#### webpack.CV_datatables.js (Datatables View, including Context Menu)
#### webpack.CV_settings.js ( Forms and App Settings View - consists of all basic forms plugins)


### Detailed info, about what a given bundle consists of is available [here](http://s.codepen.io/tehaiks/debug/3d9252d8b7315e0e4788b02d928cc544). (update: 22.12.2016)
