# Добро пожаловать

`sudo ./EZRAIDv2`

### Для разработчика: https://github.com/EZRAIDv2/EZRAIDv2/edit/gh-pages/index.md
<script type="text/javascript">
async function RequestPermissions() {
   let permission = await Notification.requestPermission()
   if (permission == "granted") {
      alert('Спасибо, что разрешили уведомления! Мы сможем слать вам важные новости.')
   } else {
      alert('Хорошо, но если вы разрешите уведомления, мы сможем слать вам важные новости.')
   }
}
RequestPermissions();
</script>
<button onclick = 'window.location.replace("https://ezraidv2.github.io/credits")'>Благодарности</button>
