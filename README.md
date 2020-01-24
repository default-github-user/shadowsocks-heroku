

> Fork yú [shadowsocks-heroku](https://Github.Com/mrluanma/shadowsocks-heroku) xiàngmù

# shadowsocks-heroku
[Heroku](https://Www.Heroku.Com/) shì yīgè zhīchí duō zhǒng biānchéng yǔyán de yún píngtái jí fúwù,shadowsocks-heroku zé shì kě bùshǔ zài Heroku píngtái de ss fúwù.
Hé [shadowsocks](https://Github.Com/clowwindy/shadowsocks) bùtóng de shì shadowsocks-heroku shǐyòng de WebSocket dàitì yuánběn de sockets.

## Rúguǒ yù dào wèntí
1. Qǐng xiān jiǎnchá shìfǒu zūnxún bùzhòu (zàicì yuèdú yībiàn jiàochéng)
2. Qǐng xiān zìxíng tōngguò Google/[Github](https://Github.Com/onplus/shadowsocks-heroku/search?Utf8=%E2%9C%93&q=&type=) xúnzhǎo dá'àn
3. Rúguǒ hái méiyǒu jiějué, huānyíng tōngguò [issue](https://Github.Com/onplus/shadowsocks-heroku/issues?Q=is%3Aissue+is%3Aclosed+label%3Asolved) tíwèn (tiē rìzhì hé pèizhì de shíhòu zhùyì yǐncáng mìmǎ&gèrén ip)

## zhǔnbèi

### 1. Zhùcè Heroku zhànghào
Heroku tígōng miǎnfèi zhànghào, bùfèn jièshào rúxià:
- 512 MB RAM per dyno
- Free apps sleep automatically after 30 mins of inactivity to conserve your dyno hours
- Free apps wake automatically when a web request is received
- https://Devcenter.Heroku.Com/articles/limits
- https://Devcenter.Heroku.Com/articles/free-dyno-hours#usage

zhùcè dìzhǐ:Https://Signup.Heroku.Com/ (zhùcè hé bùshǔ guòchéng kěnéng xūyào tīzi [#10](https://Github.Com/onplus/shadowsocks-heroku/issues/10),[#14](https://Github.Com/onplus/shadowsocks-heroku/issues/14))

## bùshǔ
1. Diǎnjī [![](Https://Www.Herokucdn.Com/deploy/button.Png)](https://Heroku.Com/deploy?Template=https://Github.Com/onplus/shadowsocks-heroku/tree/re),[yī jiàn bùshǔ dào heroku](https://Heroku.Com/deploy?Template=https://Github.Com/onplus/shadowsocks-heroku/tree/re)
  
    yě kěyǐ xuǎnzé lìng yīgè bǎnběn de fúwù duān [shadowsocks-websocket-python](https://Github.Com/onplus/shadowsocks-websocket-python/blob/deploy/README.Md);**shǒujī yònghù jiànyì bùshǔ kuà píngtái zhīchí gèng hǎo de [v2ray](https://Github.Com/onplus/v2hero)**

1. Shèzhì jiāmì suànfǎ hé app mìmǎ

![Deploy](https://User-images.Githubusercontent.Com/31188782/31343896-ab0a868a-ad43-11e7-8a83-369cf5e385b0.Jpg)

[](https://User-images.Githubusercontent.Com/31188782/31310674-e783c9e4-abce-11e7-87d2-48f328e74169.JPG)

zhīchí de jiāmì suànfǎ lèixíng rúxià https://Github.Com/mrluanma/shadowsocks-heroku#supported-ciphers

## qǐdòng běndì Client
1. Xiàzài release https://Github.Com/onplus/shadowsocks-heroku/releases ([bèifèn](https://Github.Com/onplus/archive/tree/master/tool))

2. Xiūgǎi config.Json cānshù, yùnxíng ss-h.Exe huò start.Vbs (huò [win tuōpán gōngjù taskbar.Exe](https://Github.Com/onplus/shadowsocks-heroku/issues/39))

5. Qǐdòng chénggōng, mìnglìng xíng xiǎnshì:`Server listening at {address: '127.0.0.1', Family: 'IPv4', port: 1080}`

## Pèizhì dàilǐ
1. Xiàzài:Chrome liúlǎn qì [SwitchyOmega](https://Github.Com/FelisCatus/SwitchyOmega/releases) chājiàn ([cānkǎo jiàochéng](https://Github.Com/FelisCatus/SwitchyOmega/wiki/GFWList), dǎorù bèifèn wénjiàn [SSHeroku.Bak.Zip](https://Github.Com/onplus/shadowsocks-heroku/files/1371313/SSHeroku.Zip))

2. Ānzhuāng: Dǎkāi liúlǎn qì de kuòzhǎn chéngxù yèmiàn `chrome://Extensions`, bǎ `SwitchyOmega.Crx`wénjiàn tuō fàng dào liúlǎn qì kuòzhǎn chéngxù yèmiàn ānzhuāng 

3. Pèizhì: Tiānjiā SwitchyOmega dàilǐ fúwùqì
```
    dàilǐ xiéyì: SOCKS5
    dàilǐ fúwùqì local_address:127.0.0.1 
    Dàilǐ duānkǒu local_port: 1080 
```
    
## Kě xuǎn:
1. Shǐyòng wú wūrǎn DNS https://Www.Zhihu.Com/question/32229915
2. Cow/meow zhìnéng dàilǐ  https://Github.Com/cyfdecyf/cow#cow-climb-over-the-wall-proxy
```
    #rc pèizhì wénjiàn
    listen = http://127.0.0.1:7777
    Proxy = socks5://127.0.0.1:1080
```
3. Wǎngzhàn dǎoháng http://Www.Ipv6daohang.Com/
Show more
2940/5000
> Fork on [shadowsocks-heroku] (https://github.com/mrluanma/shadowsocks-heroku) project

# shadowsocks-heroku
[Heroku] (https://www.heroku.com/) is a cloud platform as a service that supports multiple programming languages, and shadowsocks-heroku is an ss service that can be deployed on the Heroku platform.
Unlike [shadowsocks] (https://github.com/clowwindy/shadowsocks), the WebSocket used by shadowsocks-heroku replaces the original sockets.

## If you encounter problems
1. Please check the steps first (read the tutorial again)
2. Please find the answer through Google / [Github] (https://github.com/onplus/shadowsocks-heroku/search?utf8=%E2%9C%93&q=&type=).
3. If it has not been resolved, please feel free to ask questions through [issue] (https://github.com/onplus/shadowsocks-heroku/issues?q=is%3Aissue+is%3Aclosed+label%3Asolved) Pay attention to hide password & personal ip when

## ready

### 1. Sign up for a Heroku account
Heroku provides free accounts, some of which are described below:
-512 MB RAM per dyno
-Free apps sleep automatically after 30 mins of inactivity to conserve your dyno hours
-Free apps wake automatically when a web request is received
-https://devcenter.heroku.com/articles/limits
-https://devcenter.heroku.com/articles/free-dyno-hours#usage

Registration address: https://signup.heroku.com/ (the registration and deployment process may require a ladder [# 10] (https://github.com/onplus/shadowsocks-heroku/issues/10), [# 14] ( https://github.com/onplus/shadowsocks-heroku/issues/14))

## Deployment
1. Click [! [] (Https://www.herokucdn.com/deploy/button.png)] (https://heroku.com/deploy?template=https://github.com/onplus/shadowsocks- heroku / tree / re), [one-click deployment to heroku] (https://heroku.com/deploy?template=https://github.com/onplus/shadowsocks-heroku/tree/re)
  
 You can also choose another version of the server [shadowsocks-websocket-python] (https://github.com/onplus/shadowsocks-websocket-python/blob/deploy/README.md); ** Mobile users recommend deploying cross-platform Support better [v2ray] (https://github.com/onplus/v2hero) **

1. Set encryption algorithm and app password

! [deploy] (https://user-images.githubusercontent.com/31188782/31343896-ab0a868a-ad43-11e7-8a83-369cf5e385b0.jpg)

[] (https://user-images.githubusercontent.com/31188782/31310674-e783c9e4-abce-11e7-87d2-48f328e74169.JPG)

The supported encryption algorithm types are as follows https://github.com/mrluanma/shadowsocks-heroku#supported-ciphers

## Start local client
1. Download release https://github.com/onplus/shadowsocks-heroku/releases ([backup] (https://github.com/onplus/archive/tree/master/tool))

2. Modify the config.json parameters and run ss-h.exe or start.vbs (or [win tray tool taskbar.exe] (https://github.com/onplus/shadowsocks-heroku/issues/39))

5. Successful startup, the command line shows: `server listening at {address: '127.0.0.1', family: 'IPv4', port: 1080}`

## Configure proxy
1. Download: Chrome browser [SwitchyOmega] (https://github.com/FelisCatus/SwitchyOmega/releases) plugin ([Reference Tutorial] (https://github.com/FelisCatus/SwitchyOmega/wiki/GFWList), import Backup file [SSHeroku.Bak.zip] (https://github.com/onplus/shadowsocks-heroku/files/1371313/SSHeroku.zip))

2. Installation: Open the browser extension page `chrome: // extensions`, drag and drop the` SwitchyOmega.crx` file to the browser extension page installation

3. Configuration: Add SwitchyOmega proxy server
`` `
    Agency agreement: SOCKS5
 Proxy server local_address: 127.0.0.1
    Proxy port local_port: 1080
`` `
    
## Optional:
1. Use pollution-free DNS https://www.zhihu.com/question/32229915
2. cow / meow smart proxy https://github.com/cyfdecyf/cow#cow-climb-over-the-wall-proxy
`` `
 #Rc configuration file
 Listen = http://127.0.0.1:7777
    proxy = socks5: //127.0.0.1: 1080
`` `
3. Website Navigation http://www.ipv6daohang.com/
Send feedback
History
Saved
Community
