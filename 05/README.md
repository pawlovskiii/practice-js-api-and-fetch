> :star: *Jeśli będziesz mieć problem z rozwiązaniem tego zadania, poproś o pomoc na odpowiednim kanale na Slacku, tj. `#s1e09-js-api-and-fetch` (dotyczy [mentee](https://devmentor.pl/mentoring-javascript/) oraz posiadaczy [kursu JavaScript](https://devmentor.pl/p/javascript-for-beginners/)) lub na [dedykowanej grupie fb](https://www.facebook.com/groups/155234921740033). Pamiętaj, aby treść Twojego wpisu spełniała [odpowiednie kryteria](https://devmentor.pl/jak-prosic-o-pomoc/).*

&nbsp;

# `#05` JavaScript: API oraz FETCH


W tym zadaniu będziesz potrzebować narzędzia [JSON Server](https://github.com/typicode/json-server), które uruchomi lokalne API na podstawie pliku `data.json`.

W pliku tym znajdują się już dane, które zostaną załadowane do HTML-a za pomocą kodu napisanego w `app.js` zaraz po uruchomieniu lokalnego API.

JSON Server można uruchomić w terminalu przy pomocy komendy: `json-server ./data.json --watch`.

Twoim zadaniem jest napisanie obsługi formularza, tak aby można było dodawać nowe dane do naszego lokalnego API.

Przypominam, że należy:
* wykorzystać odpowiednią metodę (`POST`),
* na podstawie wysłanych przez formularz danych utworzyć obiekt, który trzeba zamienić na format JSON (`JSON.stringify()`),
* przekazanć odpowiedni nagłówek (`'Content-Type': 'application/json'`).

Po każdorazowym dodaniu użytkownika zaktualizuj widok przy pomocy funkcji `loadUsers()`. Trzeba ją uruchomić w odpowiednim momencie, np. w `finally()`.

 **Uwaga!** Podczas tworzenia rozwiązań wykorzystujących API, możesz się spotkać z problemem dotyczącym [CORS](https://sekurak.pl/czym-jest-cors-cross-origin-resource-sharing-i-jak-wplywa-na-bezpieczenstwo/). Jeśli on wystąpi, to nie będziesz mógł pobrać danych z API. Wszystko zależy od konfiguracji przeglądarki i serwera. Problem zidentyfikujesz przez [odpowiedni komunikat w konsoli](https://www.google.com/search?q=cors+problem&source=lnms&tbm=isch). Możesz próbować wyłączyć to zabezpieczenie w przeglądarce przez [odpowiedni plugin](https://chrome.google.com/webstore/detail/moesif-orign-cors-changer/digfbfaphojjndkpccljibejjbppifbc) lub wykorzystując [pośrednika](https://jsonp.afeld.me/).
 Problem z CORS może być spowodowany również tym, że uruchamiasz plik przez protokół `file://`. Wówczas wystarczy, że uruchomisz plik `.html` przy pomocy rozszerzenia [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) do VSC.


&nbsp;

> :arrow_left: [*poprzednie zadanie*](./../04) | ~~*następne zadanie*~~ :arrow_right:

> :no_entry: *Jeśli nie posiadasz materiałów do tego zadania, znajdziesz je na stronie [devmentor.pl](https://devmentor.pl/p/js-basics/)*
