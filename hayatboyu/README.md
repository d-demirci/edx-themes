Yaşar Üniversitesi Hayat Boyu Öğrenme Ortamı  (Open edX)
========
Sakarya Üniversitesi Open edX platformu için şablon çalışmasıdır.

Sizde Open edX için özel bir tema tasarlayabilirsiniz. Bunun için edX alt yapısına hakim olmanız gerekmektedir. Sakarya Üniversitesi için hazırlanmış olduğum şablonu dilerseniz sizde kullanabilirsiniz. Kurulum ile ilgili ayrıntılara aşağıdan ulaşabilirsiniz.

![Alt text](/hayatboyu.jpg?raw=true "Yaşar Üniversitesi Hayat Boyu Öğrenme Ortamı")

Şablon Hakkında
===============
Temayı yüklemek için aşağıdaki adımları izleyiniz.:
- Projeyi önce fork'layınız.
- Daha sonra /edx/app/edxapp  dizini altına "themes" isimli bir klasör oluşturup themes klasörünün içine gidiniz.
- git clone https://github.com/{username}/hayatboyu.git dosyaları theme klasörünün içine indiriyoruz.
- Css ve görselleri kendinize göre düzenleyin.
- Tema ismini değiştirmek için static/sass/ hayatboyu.scss adını tüm dosyalarda hayatboyu ifadesi geçen kısımları düzeltmelisiniz.
- Özel şablonu edx te aktif etmek için /edx/app/edxapp klasörü altında bulunan lms.env.json dosyasında öncelikle 'USE_CUSTOM_THEME' parametresini True yapıp, 'THEME_NAME' kısmına ise tema isminizi yazmalısınız.
- Open edX kurulu ve yapılandırması kompleks bir yapıda olmasına karşın çok kullanışlı bir öğrenme ortamı bize sunmaktadır.
- cd /edx/app/edxapp/edx-platform
- source /edx/app/edxapp/edxapp_env
- paver update_assets lms --settings=aws
- sudo /edx/bin/supervisorctl restart edxapp:
- sudo /edx/bin/supervisorctl restart edxapp_worker:
