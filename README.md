
<div align="center">
 <img src="<a href="https://resimlink.com/O0PhV7D" title="ZeuS Olympus"><img src="https://r.resimlink.com/O0PhV7D.jpg" title="ZeuS Olympus" alt="ZeuS Olympus"></a>" 
  <h1>Olympus UserBot</h1>
</div>
<p align="center">
    Olympus UserBot, Telegram kullanmanızı kolaylaştıran bir bottur. Tamamen açık kaynaklı ve ücretsizdir.
    <br>
        <a href="https://github.com/iibrahimwt13/OlympusUserBot/blob/master/README.md#kurulum">Kurulum</a> |
        <a href="https://github.com/iibrahimwt13/OlympusUserBot/wiki/G%C3%BCncelleme">Güncelleme</a> |
        <a href="https://t.me/olympuss10">Telegram Kanalı</a>
    <br>
</p>

----
![Docker Pulls](https://img.shields.io/docker/pulls/fusuf/asenauserbot?style=flat-square) ![Docker Image Size (latest by date)](https://img.shields.io/docker/image-size/fusuf/asenauserbot?style=flat-square)
## Kurulum

[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy?template=https://github.com/iibrahimwt13/olympususer)

### String Alma Yöntemi
```Termux
git clone https://github.com/iibrahimwt13/olympususer.git
cd olympususer
pip install -r requirements.txt
python3 GenerateStringSession.py
```

## Örnek Plugin
```python
from userbot.events import register
from userbot.cmdhelp import CmdHelp # <-- Bunu ekleyin.

@register(outgoing=True, pattern="^.deneme")
async def deneme(event):
    await event.edit('Gerçekten deneme!')

Help = CmdHelp('deneme') # Bilgi ekleyeceğiz diyoruz.
Help.add_command('deneme', # Komut
    None, # Komut parametresi varsa yazın yoksa None yazın
    'Gerçekten deneme yapıyor!', # Komut açıklaması
    'deneme' # Örnek kullanım.
    )
Help.add_info('@Fusuf tarafından yapılmıştır.') # Bilgi ekleyebilirsiniz.
# Ya da uyarı --> Help.add_warning('KULLANMA!')
Help.add() # Ve Ekleyelim.
```

## Bilgilendirme
Herhangi bir istek & şikâyet & öneri varsa [destek grubuna](https://t.me/olympuss10) ulaşabilirsiniz.

```
    Userbottan dolayı; Telegram hesabınız yasaklanabilir.
    Bu bir açık kaynaklı projedir, yaptığınız her işlemden kendiniz sorumlusunuz. Kesinlikle Olympus yöneticileri sorumluluk kabul etmemektedir.
    Olympusu kurarak bu sorumlulukları kabul etmiş sayılırsınız.
```

