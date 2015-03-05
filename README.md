# module-conflict-detector

## INSTALLATION 

### A) Via Modman - Recommended (https://github.com/colinmollenhour/modman)

#### 1) Install Modman:

```
bash < <(wget -O - https://raw.github.com/colinmollenhour/modman/master/modman-installer)
```

or

```
bash < <(curl -s https://raw.github.com/colinmollenhour/modman/master/modman-installer)
source ~/.profile
```

#### 2) Allow symlinks for the templates directory (required for installation via Modman)

 - For newer Magento versions (1.5.1.0 & above) you just need enable 'Allow Symlinks' from System - Configuration / Advanced / Developer / Template Settings
 - For older Magento versions: http://www.tonigrigoriu.com/magento/magento-how-to-fix-template-path-errors-when-using-symlinks/

#### 3) Install module conflict detector module:
 
<pre>
cd [magento root folder]
modman init
modman clone https://github.com/juito/module-conflict-detector.git

</pre>

 - Make sure you've cleaned Magento's cache to enable the new module; hit refresh
 
#### How to update
I'm pretty lazy and I don't like to create Magento Connect packages. With modman you can effortlessly grab the latest changes from github.
<pre>
modman update module-conflict-detector
</pre>
 - Clean Magento's cache to make sure new changes will be enabled.

 - `Disable SQL Profiler` is not working, but `Enable SQL Profiler` works like a charm (or not)
