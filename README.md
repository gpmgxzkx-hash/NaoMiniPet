# ナオのミニペット v0.5 Cloud Build

Androidの画面上に常駐するミニペット試作版です。

## 入っているもの
- 画面上を自動移動
- ドラッグ移動
- タップ反応とセリフ
- 長押しで休憩
- サイズ・透明度・速度設定
- 時間帯・低バッテリー時のセリフ
- Android 14+向け foreground service (specialUse)

## APK化
`.github/workflows/build-apk.yml` を同梱しています。
GitHub Actions の **Build Android APK** を実行すると `app-debug.apk` が成果物として生成されます。
このワークフローはクラウド側で JDK 17 / Android SDK 35 / Gradle 8.9 を用意するため、PCにAndroid Studioは不要です。

## 注意
端末への初回インストール時は、Android側で「不明なアプリのインストール」を許可する必要があります。
アプリ起動後は「他のアプリの上に表示」権限も必要です。
