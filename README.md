### Forked [Youtube plus](https://github.com/ParticleCore/Particle "Youtube plus") by [ParticleCore](https://github.com/ParticleCore "ParticleCore") with some fixes
- Only for old youtube layout
- only JS implementation 
- something may not work
- basic functionality tested on chrome (tampermonkey)
-------------------

##### Permanently change youtube layout to old one 
> (until cookies will be renewed/deleted)

1. Open developer tool in browser by `Ctrl + Shift + i`
2. Paste and execute in console following code :
```
document.cookie = document.cookie.split(' ').filter(o=>o.indexOf('PREF=')!==-1)[0].replace(';','')+'&f5=30030&f6=8;domain=.youtube.com;path=/';
```
3. Hard reload youtube page by `Shift + reload button` or `Ctrl + F5`
