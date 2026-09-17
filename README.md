# Заглушка «Кто точно знает»

Статичная страница по утверждённому изображению. Поле и кнопка являются частью изображения и не работают; адрес почты кликабелен. На телефоне боковые пустые поля изображения скрываются.

## Публикация

1. Создайте отдельный публичный репозиторий `ktotochno-placeholder`.
2. Загрузите содержимое архива в корень репозитория, без внешней папки. Файлы `index.html`, `placeholder.png` и `CNAME` должны лежать рядом.
3. Settings → Pages → Build and deployment → Source: Deploy from a branch → main → /(root) → Save.
4. В Custom domain укажите `ktotochno.ru` и сохраните до изменения DNS.
5. В Selectel добавьте четыре A-записи для корня ktotochno.ru с TTL 3600:
   - 185.199.108.153
   - 185.199.109.153
   - 185.199.110.153
   - 185.199.111.153
6. Для www добавьте CNAME на `matildalikho-cpu.github.io.`
7. Сохраните существующие MX, TXT, NS и SOA. Если есть прежние A/AAAA именно для веб-сайта, замените их, не оставляя конфликтующие адреса.
8. После успешной DNS-проверки в GitHub Pages включите Enforce HTTPS. Обновление DNS и выпуск сертификата могут занять до 24 часов.

Документация: https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/managing-a-custom-domain-for-your-github-pages-site
