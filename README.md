<img src="http://framework.zend.com/images/head-bottom-picture.png"
 alt="ZF2 Logo 1" title="ZF2 User Module" align="right" />


# User Module für ZF2

<img src="https://packages.zendframework.com/docs/latest/manual/en/_static/zf2_logo.png"
 alt="ZF2 Logo 0" title="ZF2 User Module" align="right" />

Dies wird ein UserModul für ZF2.

Bisher gibt es im Controoler nur folgende Aktionen:

  - Index (indexAction)
  - Anmelden (loginAction)
  - Registrieren (registerAction)

Von [Andreas Vogelbacher] für ein Semesterprojekt in der [ABB-TS] [1]:

# Version
0.0.1

> Achtung:

> Early beta

# Installation

(siehe auch https://github.com/avogelba/test2 für Application Modul)

1. Create a ZF2 Skeleton Application
e.g. with Netbeans

2. create VHOST in APache
```
<VirtualHost zf2.local:80>
	ServerName zf2.local
	DocumentRoot "c:/My Web Sites/zf2.local/public"
    	ErrorLog "logs/zf2.local.log"
    	CustomLog "logs/zf2.local.log" common
	SetEnv APPLICATION_ENV "development"
	<Directory "c:/My Web Sites/zf2.local/public">
		#DirectoryIndex index.php
		AllowOverride All
		#Order allow,deny
		#Allow from all
	    	Require all granted
	</Directory>
</VirtualHost>
```

3. add virtual address to hosts
e.g. c:\Windows\System32\drivers\etc\hosts
```
127.0.0.1					zf2.local
```

4. Restart apache

5. Open
http://yoursite.local
and enshure ZF2 is working
![Image](https://github.com/avogelba/test/blob/master/ZF2_skeleton.jpg?raw=true)

6. add following to6
config\application.config.php
```php
<?php
return array(
 ...
 //other modules 
 'Users',
), 
```

7. Open
http://yoursite.local/users
and hope User module works
![Image](https://github.com/avogelba/test/blob/master/users.jpg?raw=true)

###Note
Da habe ich doch gralatt englisch getippt bei Installation

##ToDo

Forms generieren ()
___


## ---- Tests -----


> Es kommen ein paar Markdown Tests um rauszufinde wie das Funktioniert:

## Mardown Tests

[Visit GitHub!](www.github.com)

:smile:

/play secret

```javascript
$(function(){
  $('div').html('I am a div.');
});
```

```php
public function registerAction()
    {
        $view = new ViewModel();
        $view->setTemplate('users/index/new-user');
        return $view;
    }
```
| **[Technical Docs] [techdocs]**     | **[Setup Guide] [setup]**     | **[Roadmap] [roadmap]**           | **[Contributing] [contributing]**           |
|-------------------------------------|-------------------------------|-----------------------------------|---------------------------------------------|
| [![i1] [techdocs-image]] [techdocs] | [![i2] [setup-image]] [setup] | [![i3] [roadmap-image]] [roadmap] | [![i4] [contributing-image]] [contributing] |


[Andreas Vogelbacher]:nixda@willkeinspam.com
[1]:http://abbts.ch

[techdocs-image]: https://d3i6fms1cm1j0i.cloudfront.net/github/images/techdocs.png
[setup-image]: https://d3i6fms1cm1j0i.cloudfront.net/github/images/setup.png
[roadmap-image]: https://d3i6fms1cm1j0i.cloudfront.net/github/images/roadmap.png
[contributing-image]: https://d3i6fms1cm1j0i.cloudfront.net/github/images/contributing.png

[techdocs]: http://framework.zend.com/manual/2.3/en/user-guide/overview.html
[setup]: https://github.com/avogelba/test
[roadmap]: https://github.com/avogelba/test
[contributing]: https://github.com/avogelba/test

