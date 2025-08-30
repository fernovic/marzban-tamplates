<h1 align="center"/>تمپلیت برای پنل  <a href="https://github.com/Gozargah/Marzban">مرزبان</a></h1>

# مقدمه
 تمپلیت شخصی سازی شده برای مرزبان


# نصب
برای نصب تمپلیت دستورات زیر را در ترمینال سرور خود اجرا کنید:
1. دانلود فایل تمپلیت
```sh
sudo wget -N -P /var/lib/marzban/templates/clash/ https://raw.githubusercontent.com/fernovic/marzban-tamplates/main/default.yml
```
2. دستورات زیر رو تو ترمینال سرورتون بزنید:
```sh
echo 'CUSTOM_TEMPLATES_DIRECTORY="/var/lib/marzban/templates/"' | sudo tee -a /opt/marzban/.env
echo 'CLASH_SUBSCRIPTION_TEMPLATE="clash/default.yml"' | sudo tee -a /opt/marzban/.env
```
یا مقادیر زیر رو در فایل `.env` در پوشه `/opt/marzban/` قرار بدین
```sh
CUSTOM_TEMPLATES_DIRECTORY="/var/lib/marzban/templates/"
CLASH_SUBSCRIPTION_TEMPLATE="clash/default.yml"
```

3. ری استارت مرزنشین
```sh
marzban restart
```

## بروزرسانی
برای بروزرسانی تمپلیت ها فقط کافیست مرحله 1 را تکرار کنید.
