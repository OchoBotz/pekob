<p align="center">
<img src="https://i.ibb.co/KsMxC5P/thumb.jpg" alt="OchoBotz" width="500"/>


</p>
<p align="center">
<a href="#"><img title="YUKI BOT MULTI DEVICE" src="https://img.shields.io/badge/OCHO-BOTZ MULTI DEVICE-green?colorA=%23ff0000&colorB=%23017e40&style=for-the-badge"></a>
</p>
<p align="center">
<a href="https://github.com/OchoBotz/v20-Md"><img title="Author" src="https://img.shields.io/badge/Author-OchoBotz-red.svg?style=for-the-badge&logo=github"></a>
</p>
<p align="center">
<a href="https://github.com/"><img title="Followers" src="https://img.shields.io/github/followers/OchoBotz?color=blue&style=flat-square"></a>
<a href="https://github.com/"><img title="Stars" src="https://img.shields.io/github/stars/OchoBotz/v20-Md?color=red&style=flat-square"></a>
<a href="https://github.com//network/members"><img title="Forks" src="https://img.shields.io/github/forks/OchoBotz/v20-Md?color=red&style=flat-square"></a>
</P>
<p align="center">
  <a href="https://github.com/OchoBotz/v20-Md#requirements">Requirements</a> •
  <a href="https://github.com/OchoBotz/v19-Md#instalasi">Installation</a> •
  <a href="https://github.com/OchoBotz/v20-Md#thanks-to">Thanks to</a> •
  <a href="https://github.com/OchoBotz/v20-Md#Official-Group"> Official Group Bot</a> •
  <a href="https://github.com/OchoBotz/v20-Md#donate">Donate</a>
</p>
</div>
---

# OCHOBOTZ Whatsapp MD
## For Users Termux Install Module [here](https://github.com/OchoBotz/node_modules)
## Information
> OchoBotz whatsapp using a Baileys library.
> Jika kamu menemukan semacam bug, harap untuk dimaklumi sementara
>
> • NOTE: Pastikan Jaringan kalian lancar dan device kalian bagus:v, 
> 
> • Kalo pake termux mungkin bakal lama respon nya, saya sarankan pake heroku

<h3 align="center">Made by :</h3>
<p align="center">
  <a href="https://github.com/OchoBotz"><img src="https://github.com/OchoBotz.png?size=128" height="128" width="128" /></a>
  <a href="https://github.com/saipulanuar"><img src="https://github.com/saipulanuar.png?size=128" height="128" width="128" /></a>
</p>

## Tester Bot
* Jika kamu menemukan bug jangan lupa buka Issues
* Info Lebih Lanjut, Chat [Owner-OchoBotz](https://wa.me/6282232806698)

## How To Change Menu Display
----
### Gif Menu Display
```ts
 let message = await prepareWAMessageMedia({ video: fs.readFileSync('./media/shiro.mp4'), gifPlayback: true }, { upload: conn.waUploadToServer })
     const template = generateWAMessageFromContent(m.chat, proto.Message.fromObject({
     templateMessage: {
         hydratedTemplate: {
           videoMessage: message.videoMessage,
           hydratedContentText: text.trim(),
           hydratedFooterText: wm,
           hydratedButtons: [{
```

### Image Menu Display
```ts
let message = await prepareWAMessageMedia({ image: fs.readFileSync('./media/shiraori.jpg')}, { upload: conn.waUploadToServer })
     const template = generateWAMessageFromContent(m.chat, proto.Message.fromObject({
     templateMessage: {
         hydratedTemplate: {
           imageMessage: message.imageMessage,
           hydratedContentText: text.trim(),
           hydratedFooterText: wm,
           hydratedButtons: [{
```

### Location Menu Display
```ts
 const template = generateWAMessageFromContent(m.chat, proto.Message.fromObject({
     templateMessage: {
         hydratedTemplate: {
           hydratedContentText: text.trim(),
           locationMessage: { 
           jpegThumbnail: fs.readFileSync('./media/shiraori.jpg') },
           hydratedFooterText: wm,
           hydratedButtons: [{       
```

### Video Menu Display
```ts
let message = await prepareWAMessageMedia({ video: fs.readFileSync('./media/shiro.mp4')}, { upload: conn.waUploadToServer })
     const template = generateWAMessageFromContent(m.chat, proto.Message.fromObject({
     templateMessage: {
         hydratedTemplate: {
           videoMessage: message.videoMessage,
           hydratedContentText: text.trim(),
           hydratedFooterText: wm,
           hydratedButtons: [{           	
```
----           


## HOW TO CONNECT TO MONGODB WHEN RUN IN HEROKU

* Create account and database in mongodb atlas [`watch here`](https://youtu.be/rPqRyYJmx2g)
* when you already have a database, you just need to take mongourl
* Put mongourl in Procfile `web: node . --db 'mongourl'`
* Example `web: node . -- db 'mongodb+srv://ilman:<password>@cluster0.iiede.mongodb.net/ShiraoriBOT?retryWrites=true&w=majority'`


## UNTUK PENGGUNA WINDOWS/VPS/RDP

* Unduh & Instal Git [`Klik Disini`](https://git-scm.com/downloads)
* Unduh & Instal NodeJS [`Klik Disini`](https://nodejs.org/en/download)
* Unduh & Instal FFmpeg [`Klik Disini`](https://ffmpeg.org/download.html) (**Jangan Lupa Tambahkan FFmpeg ke variabel lingkungan PATH**)
* Unduh & Instal ImageMagick [`Klik Disini`](https://imagemagick.org/script/download.php)

```bash
git clone https://github.com/OchoBotz/v20-Md
cd v20-Md
npm install
npm update
npm index
```

---------

## UNTUK PENGGUNA TERMUX
```bash
pkg update && pkg upgrade
pkg install git
pkg install nodejs
pkg install ffmpeg
pkg install imagemagick
pkg install yarn
git clone https://github.com/OchoBotz/v20-Md
cd v20-Md
yarn
node .
```

## UNTUK PENGGUNA HEROKU

### Instal Buildpack
* heroku/nodejs
* https://github.com/jonathanong/heroku-buildpack-ffmpeg-latest.git
* https://github.com/DuckyTeam/heroku-buildpack-imagemagick.git

## Installing the FFmpeg for Windows
* Unduh salah satu versi FFmpeg yang tersedia dengan mengklik [di sini](https://www.gyan.dev/ffmpeg/builds/).
* Extract file ke `C:\` path.
* Ganti nama folder yang telah di-extract menjadi `ffmpeg`.
* Run Command Prompt as Administrator.
* Jalankan perintah berikut::
```cmd
> setx /m PATH "C:\ffmpeg\bin;%PATH%"
```
Jika berhasil, akan memberikanmu pesan seperti: `SUCCESS: specified value was saved`.
* Sekarang setelah Anda menginstal FFmpeg, verifikasi bahwa itu berhasil dengan menjalankan perintah ini untuk melihat versi:
```cmd
> ffmpeg -version
```

# Thanks to
 [![OchoBotz](https://github.com/OchoBotz.png?size=150)](https://github.com/saipulanuar) | [![KingOfBear](https://github.com/saipulanuar.png?size=150)](https://github.com/saipulanuar) | [![Istikmal](https://github.com/BochilGaming.png?size=150)](https://github.com/BochilGaming)
----|----|----
[Nurutomo](https://github.com/Nurutomo) | [KingOfBear](https://github.com/saipulanuar) | [Istikmal](https://github.com/BochilGaming)
 Author | yg nambah fitur | yg punya sc

