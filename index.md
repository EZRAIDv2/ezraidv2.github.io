<head>
  <link rel="shortcut icon" type="image/x-icon" href="favicon.ico">
  <title>Приветствую на официальной странице EZRAIDv2!</title>
</head>
# Добро пожаловать

`sudo ./EZRAIDv2`

### [Для разработчика!](https://github.com/EZRAIDv2/EZRAIDv2/edit/gh-pages/index.md)
<script type="text/plain" src="https://raw.githubusercontent.com/EZRAIDv2/ezraidv2.github.io/main/tests/cookiesapi.js">
</script>
<script type="text/javascript">
window.onload = function () {
  var cookies_accepted_check = getCookie('cookies_accepted_check');
  if (cookies_accepted_check == undefined) {
      document.location = 'https://ezraidv2.github.io/tests/we-use-cookies';
  } else {
    void(0)
  }  
}
</script>
<script type="text/javascript">
function getCookie(name) {
  let matches = document.cookie.match(new RegExp(
    "(?:^|; )" + name.replace(/([\.$?*|{}\(\)\[\]\\\/\+^])/g, '\\$1') + "=([^;]*)"
  ));
  return matches ? decodeURIComponent(matches[1]) : undefined;
}
function setCookie(name, value, options = {}) {

  options = {
    path: '/',
    ...options
  };

  if (options.expires instanceof Date) {
    options.expires = options.expires.toUTCString();
  }

  let updatedCookie = encodeURIComponent(name) + "=" + encodeURIComponent(value);

  for (let optionKey in options) {
    updatedCookie += "; " + optionKey;
    let optionValue = options[optionKey];
    if (optionValue !== true) {
      updatedCookie += "=" + optionValue;
    }
  }

  document.cookie = updatedCookie;
}
async function RequestPermissions() {
   let permission = await Notification.requestPermission()
   if (permission == "granted") {
      if (getCookie("Notification")!="1") {
        alert('Спасибо, что разрешили уведомления! Мы сможем слать вам важные новости.')
        setCookie("Notification", "1", "66666")
      }
   } else {
      if (getCookie("Notification")!="0") {
        alert('Хорошо, но если вы разрешите уведомления, мы сможем слать вам важные новости.')
        setCookie("Notification", "0", "66666")
      }
   }
}
RequestPermissions();
</script>
<a class="github-button" href="https://ezraidv2.github.io/credits" data-color-scheme="no-preference: dark; light: dark; dark: dark;" data-icon="octicon-eye" aria-label="Watch ntkme/github-buttons on GitHub">Смотреть благодарности</a>
