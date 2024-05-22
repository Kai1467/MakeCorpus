# 配信アーカイブから音声コーパスの作成

## 配信アーカイブの取得

### mac OS の場合

**youtube-dl**
youtube-dl：YoutubeやTwitchの動画をダウンロード出来るライブラリ
[youtube-dl -公式-](https://github.com/ytdl-org/youtube-dl/)  

#### Instal
`brew install youtube-dl`

#### How to Use
`youtube-dl 'URL' -x --audio-format wav`


#### Config File の設定
一部の設定はconfigファイルとして設定している。[【Mac】ターミナルで動画ダウンロード](https://mac-ra.com/terminal-youtube-dl/)  

##### 作成

~/.config/youtube-dl にディレクトリを作成。ココにconfigファイルを作成

```config
-o '~/Desktop/youtube/MIKO_youtube_%(upload_data)s.%(ext)s'
```
コレは配信日を取得しファイル名にしている。

## MakeCorpus


